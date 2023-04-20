This repo is an Ansible playbook.

It helps me to manage my Raspberry Pi using my iPad.

TLDR; 

I connect to the Raspberry Pi, using Blink Shell  on my iPad, and run this playbook.

It sets up the necessary configuration for:

- local network to pi through USB-C connected to iPad (it creates and ad-hoc network)
- basic nginx configuration (wip)

## setup

create ssh key on host pc (or iPad Pro)

ssh to server

add ssh.pub to authorized_keys

reboot


## Develop and connect locally to your Raspberry Pi 4 from your iPad Pro M1+M2.

on your raspberry pi run the following

```
git clone https://github.com/christian-fei/ipad-pi-usb-setup.git
cd ipad-pi-usb-setup
```


## install deps

```bash
ansible-galaxy collection install community.docker
ansible-galaxy collection install community.general
ansible-galaxy install -r requirements.yml
```


---

install ansible on your pi

```
sudo apt update
sudo apt install ansible
```

run the playbook

```
ansible-playbook playbook.yml
```

reboot your pi

```
sudo reboot
```

enjoy!

---

**thanks to https://neoighodaro.com/posts/10-setting-up-raspberry-pi-to-work-with-your-ipad**

thanks to https://neoighodaro.com/posts/10-setting-up-raspberry-pi-to-work-with-your-ipad

#### Develop and connect locally to your Raspberry Pi 4 from your iPad Pro M1+M2.

on your raspberry pi run the following

```
git clone https://github.com/christian-fei/ipad-pi-usb-setup.git
cd ipad-pi-usb-setup
```

install ansible on your pi

```
sudo apt update
sudo apt install ansible
```

run the playbook

```
ansible-playbook playbook.yml
```

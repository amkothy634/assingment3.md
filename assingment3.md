# Assignment 3 – User Management and File System Access

## 1. Create user tupu
Command:
sudo adduser tupu

## 2. Create user lupu
Commands:
sudo groupadd lupu
sudo useradd -m -d /home/lupu -s /bin/bash -g lupu lupu
sudo passwd lupu

## 3. Create system user hupu
Command:
sudo useradd --system --shell /bin/false hupu

## 4. Add tupu and lupu to sudo group
Commands:
sudo usermod -aG sudo tupu
sudo usermod -aG sudo lupu

## 5. Create /opt/projekti shared directory
Commands:
sudo groupadd projekti
sudo usermod -aG projekti tupu
sudo usermod -aG projekti lupu
sudo mkdir /opt/projekti
sudo chown tupu:projekti /opt/projekti
sudo chmod 2770 /opt/projekti


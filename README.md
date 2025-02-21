# ubuntu-in-termux

## What's This?

This is a script that allows you to install Ubuntu in your termux application without a rooted device

## Updates

**• Updated to ubuntu 24.04**

## Important

**• If you get an error message that says "Fatal Kernel too old" you have to uncomment the line that reads "command+=" -k 4.14.81"" (remove the # that is located in front of the line) in the "startubuntu.sh" file**

### Installation steps

First of all enabled storage in termux using command `termux-setup-storage`

1. Update termux: `apt-get update && apt-get upgrade -y`
2. Install wget: `apt-get install wget -y`
3. Install proot: `apt-get install proot -y`
4. Install git: `apt-get install git -y`
5. Go to HOME folder: `cd ~`
6. Download script: `git clone https://github.com/ikrammf7/ubuntu-in-termux.git`
7. Go to script folder: `cd ubuntu-in-termux`
8. Give execution permission: `chmod +x ubuntu.sh`
9. Run the script: `./ubuntu.sh -y`
10. Now just start ubuntu: `./startubuntu.sh`

## Optional

### Adduser as sudoers/sudo

for user who do not exist yet `sudo adduser <username> sudo`
for existing user `sudo usermod -a -G sudo <username>`

### Install xrdp

[xrdp installer v1.5.3 by: c-nergy.be](https://c-nergy.be/blog/?p=20178)

### Linux System Monitoring Dashboard

**• gtop**

Installation steps

1. Update termux `apt update && apt upgrade -y`
2. Install Nodejs `apt install nodejs`
3. Install gtop `npm install gtop -g`
4. Run gtop `gtop`

### Linux System fetch

**• neofetch**

Installation steps

1. Update termux `apt update && apt upgrade -y`
2. Install neofetch `apt install neofetch`
3. Run neofetch `neofetch`

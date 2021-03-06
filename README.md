# Termux NetHunter Setup

This is a script by which you can install Kali nethunter (Kali Linux) in your termux application without rooted phone 

### Steps For Installation

1. Download script in **HOME** `curl -LO https://raw.githubusercontent.com/kimocoder/termux-nethunter/master/kalinethunter`

2. Give execution permission `chmod +x kalinethunter`

3. Run script `./kalinethunter`

### Usage 

1. Use command `startkali` to start nethunter. Default user is __kali__ and default password is also __kali__.

2. if you want to start nethunter as a root user then use command `startkali -r`.

### VNC Guide

1. To start a vnc session `vnc start`

2. To stop a vnc session `vnc stop`

3. To check status ( Display and port number) of vnc session `vnc status`

4. If user is __kali__ then by default `vnc start` will start vncserver with `DISPLAY=:2` & `PORT=5902` and for root user `DISPLAY=:1` & `PORT=5901`

### In Case Of SSL error: certificate verify failed

Rerun script with extra parameter `--insecure` or copy paste this command `./kalinethunter --insecure`

### setup LXDE 

Default __DESKTOP__ is _XFCE4_ but you can setup __LXDE__ also https://www.hax4us.com/2018/07/how-to-install-lxde-in-kali-nethunter.html?m=1


### Terminal development notes

Internal and external storage wiki:
https://wiki.termux.com/wiki/Internal_and_external_storage


### Prons by using Termux over Terminal Emulator
  * System V shared memory (shmget, shmat, shmdt and shmctl) emulation on Android using ashmem for use in Termux.

    https://github.com/termux/libandroid-shmem

  * libandroid-support:
    implementation of functionality missing in Bionic libc

  * Audio support through OpenSLES
  * Better access to GPU and OpenCL
  * Better handling of sessions




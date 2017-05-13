[![Build Status](https://travis-ci.org/insuusvenerati/dotfiles.svg?branch=master)](https://travis-ci.org/insuusvenerati/dotfiles)  [![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/insuusvenerati)

I prefer setting this up by installing Antergos and running the install script from a tty.

# Setting up base install with custom ArchISO
---
 ## 1. Download ArchISO with git preinstalled

[GDrive Link](https://drive.google.com/open?id=0B7FFEpe36_QnbUZKSDFWekVGU0E)

[Mega Link](https://mega.nz/#!d9tnxYpS!8GoN2_ygtaXuBWfLEqX-z2l3gh8s6tHeRMcXYNsGeaA)

  ## 2. Clone the repo recursively and run the Arch Anywhere script

```console
git clone --recursive https://github.com/insuusvenerati/dotfiles
cd dotfiles/arch-linux-anywhere
./arch-install
```

  ## 3. Run through the Arch Anywhere script to setup Arch

   > Choose options that fit your needs but keep in mind future scripts may overwrite your selections

  ![alt](http://i.imgur.com/4bK9HWn.png)

  ## 4. Run through scripts from @erikdubois
  > I have these because it installs a lot of extra software and aesthetic stuff

  > You'll want to start off at the script named 030-

  > Choose the driver from 030 that fits your hardware

  ```console
  cd dotfiles/Archi3/installation
  ./030-install-xorg-
  ```

  > Stop after 500- if you want to use my personal dotfiles

![alt](http://i.imgur.com/Xr6wFnq.png)

  ## 5. Using my dotfiles

  ```console
  cd ~/.dotfiles
  ./install
  ```
 ## 6. Setting up lightdm

 ```console
 sudo nano /etc/lightdm/lightdm.conf
 ```

In the section labeled [Seat:*] append lightdm-webkit2-greeter to  greeter-session=


![alt](http://i.imgur.com/Quz3BjJ.png)

Edit the webkit greeter with the material2 theme for example

```console
sudo nano /etc/lightdm/lightdm-webkit2-greeter.conf
```

![alt](http://i.imgur.com/U71lHJK.png)

## 7. Restart and enjoy

![alt](http://i.imgur.com/syKxRU2.png)

Credits:
@erikdubois
@deadhead420
Special thanks to @caarlos0 for the amazing shell tools
@anishathalye for creating the install script to setup the dotfiles
@ajlende


# Dwm Ricing Guide
In this guide, i'm gonna show you on how to ricing dwm with your liking. dwm is a simple dynamic window manager written in c programming language. i'ts part of [suckless.org](https://suckless.org/). it's famous for it's quality software with a focus on simplicity, clarity, and frugality.

## Chapter 1.0
in this guide, you have to know:
- some basic c programming
- a text editor
- a passion
- some effort
- internet
- some time

by using DWM, you aggree to the terms and condition that you're gonna sitting all day on your chair while applying some patch or configuring dwm bar's module to work. _(This is a jokes)_

## Chapter 1.1, Installation
you need some dependencies before installing dwm.
```bash
sudo apt install make gcc build-essential libfmt9 git wget vim curl # debian based
```
install dwm:
```bash
git clone https://git.suckless.org/dwm
cd dwm
make
sudo make install
```
install `st` and `dmenu`:
```bash
git clone https://git.suckless.org/st
cd st
make
sudo make install
```
```bash
git clone https://git.suckless.org/dmenu
cd dmenu
make
sudo make clean install
```
it's actually all the same for installing the from the suckless.org. 
***what is actually happened?*** Let's break it down!
- `make`, This is a command used to automate the process of building or compiling software. When you run `make`, it looks at a file called `Makefile` in the project directory. This file contains instructions on how to compile and build the software. Essentially, make is like a _helper that follows these instructions_.
- `sudo`, This stands for ***"SuperUser DO."*** It's a way to tell your system you want to run the command with admin (root) permissions. Some tasks, like installing software, require these higher privileges, so `sudo` ensures you have the right permissions.
- `make install`, After building the software with make, `make install` takes the compiled software and moves it to the correct system directories (like `/usr/local/bin` or `/usr/local/lib`). This is what actually installs the software on your system, making it ready to use.

So, when you run sudo make install, you are telling your system:
```text
"Build the software using the instructions in the Makefile (with make)
Once built, install it on my system (with make install), and
Do this with admin permissions (using sudo) to make sure everything is placed correctly."
```
## Chapter 1.2, Dwm
so, let's say that you're successfully installed all these essential softwarae for authentically using dwm so that you can post your ricing to _r/unixporn_, you may want for further configuration and making the dwm work with your liking, you have to edit the dwm source code, either on `config.def.h` or `dwm.c`.

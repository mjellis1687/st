# `st` - Simple Terminal

`st` is a simple terminal emulator for X which sucks less.

## Repository Setup

- Clone the repository
- Setup upstream remote:
	```bash
	git remote add upstream https://git.suckless.org/st
	git remote set-url --push upstream DISABLE
	git checkout -b upstream upstream/master
	```

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (st is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if necessary as root):
```bash
make clean install
```

## Running `st`

If you did not install st with make clean install, you must compile the st terminfo entry with the following command:
```bash
tic -sx st.info
```

See the man page for additional details.

## Patches

- [boxdraw](https://st.suckless.org/patches/boxdraw/) via [patch](https://st.suckless.org/patches/boxdraw/st-boxdraw_v2-0.8.5.diff): Custom rendering of lines/blocks/braille characters for gapless alignment
- 

### Additional Features

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

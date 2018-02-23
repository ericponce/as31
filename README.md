# as31
Adaptation of [as31 by Paul Stoffregen](https://www.pjrc.com/tech/8051/tools/as31-doc.html) for Mac OS X, modern versions of GTK+, and potentially linux (non gui)

## Requirements - Basic - Max OS X
* CommandLineTools
* bison

## Requirements - GUI - Mac OS X
* basic requirements
* GTK+2.0 (if compiling GUI)
* pkg-config

It is recommended that you install all of this using [homebrew](http://brew.sh)

## Requirements - Basic - Ubuntu 16.04 LTS
* build-essential
	* this includes commonly used developer tools
* bison

It is recommended to install all of this using [apt](https://help.ubuntu.com/community/AptGet/Howto)

## Installation (Non-GUI)
* Compile:
`make`
* Copy bin into your path

## Installation (GUI, Mac OSX)
* Modify your pkg-config path:
`export PKG_CONFIG_PATH=/usr/local/Cellar/gtk+/<your version>/include/:/opt/X11/lib/pkgconfig/`
* Compile:
`make gui`
* Copy bin into your path

## Verification
Run `make test`

## Sources
 * [as31 for Linux Based Systems by Paul Stoffregen](https://www.pjrc.com/tech/8051/tools/linux_compile.html)
 * [Bug #655487](https://www.mail-archive.com/debian-bugs-closed@lists.debian.org/msg350992.html)


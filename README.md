this is a fork off of a fork of the blackmagick repo which hasn't seen an update in ages and for which pre-built binaries are not present anywehre and for which the 'support' page on the website is permaunderconstruction.

anyhoo. the thing wouldn't build on my machine until i tweaked the makefiles.

binaries are in the /src dir

dfu-util -d 1d50:6018,1d50:6017 -s0x02000:leave -D src/blackmagic.bin 

should do the trick.

here's the og readme which you should probably ignore



Black Magic Probe
=================

[![Build Status](https://travis-ci.org/blacksphere/blackmagic.svg?branch=master)](https://travis-ci.org/blacksphere/blackmagic)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/blacksphere/blackmagic?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![Donate](https://img.shields.io/badge/paypal-donate-blue.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=N84QYNAM2JJQG)
[![Kickstarter](https://img.shields.io/badge/kickstarter-back%20us-14e16e.svg)](https://www.kickstarter.com/projects/esden/1bitsy-and-black-magic-probe-demystifying-arm-prog)

Firmware for the Black Magic Debug Probe.

The Black Magic Probe is a modern, in-application debugging tool for
embedded microprocessors. It allows you see what is going on 'inside' an
application running on an embedded microprocessor while it executes. It is
able to control and examine the state of the target microprocessor using a
JTAG or Serial Wire Debugging (SWD) port and on-chip debug logic provided
by the microprocessor. The probe connects to a host computer using a
standard USB interface. The user is able to control exactly what happens
using the GNU source level debugging software, GDB.

See online documentation at https://github.com/blacksphere/blackmagic/wiki

Binaries from the latest automated build are at http://builds.blacksphere.co.nz/blackmagic

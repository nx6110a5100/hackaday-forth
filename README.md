## Mecrisp-Stellaris Forth, Hackaday Edition

This is the version of Mecrisp-Stellaris that I'm using to go along with my article series on Hackaday.  Here you'll find the binaries and Forth code that you need to run the demos in the articles, as well as the framework that I used to generate them.  The idea is to make it easier for you to do the same for your own projects, and to give you a few bases from which you can easily spring off.

## Quick Start

If you're just interested in flashing a Forth into an STM32F103 board and running some demos, 

1. Go get [Texane]'s [stlink tools](https://github.com/texane/stlink).  Install.
2. Flash in `mecrisp-stellaris-hackaday-edition.bin` from the [ROMs](https://github.com/hexagon5un/hackaday-forth/tree/master/ROMS) directory.
3. Have a look in the [demos](https://github.com/hexagon5un/hackaday-forth/tree/master/demos) folder.  

## Demos

Want some example code that does X, Y, or Z?  Have a look in here, in JeeLab's [Embello libraries](http://embello.jeelabs.org/flib/), and in the [Mecrisp-Stellaris "common" directory](https://github.com/jeelabs/mecrisp-stellaris/tree/master/common).  If you want to go digging, and don't mind translating from other Forths, there is a lifetime's worth of ideas in [Forth Dimensions](http://www.forth.org/fd/contents.html).

So far, the demos here include: 

* blinky

* multitasking with blinky

I'll put more up as time passes.

Submit a pull request or send me an e-mail if you want us to add yours!  

## Custom ROMs

Everything is built on the basic Mecrisp-Stellaris build, and all of the extra(neous) code is pushed to the chip from include files in the `core` directory.  Basically, you can experiment with dropping some of the requirements, or just see what's behind the various versions by tweaking your own.  Mix and match!

Caveat Programmator!  The dependencies among Forth files isn't well laid out like it is in C or any other programming language you know.  This could be fixed any number of ways, but I just haven't gotten around to it.  I tried to make notes of some of the dependencies in the files themselves.  But, indeed, that's a lot of reading. 

If you have a good custom ROM setup, submit a pull request or shoot me an e-mail.



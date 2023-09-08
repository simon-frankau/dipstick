# dipstick

![A picture of some ICs with little paper labels on top, identifying
the pins.](./dipstick.jpg)

*dipstick* is a simple postscript file that you can modify to to
 generate stickers to pop onto DIP ICs.

## Why?

When breadboarding, it's something of a pain to keep having to refer
to pinouts or schematics to work out which wire connects to which pin
number (which you then have to count out).

Instead, you can print out some labels, cut them out and stick them
onto the back of the ICs, allowing you to breadboard away without
looking at the docs. It also makes debugging a lot easier, as it's
instantly obvious where to stick the probe.

This project is inspired by
http://hackaday.com/2013/03/15/script-makes-custom-pinout-labels-for-your-chips/
, but rather than printing the labels on a special label printer, it
uses standard printers.

## How?

Modify "dipstick.ps" to include the definitions for the chips you're
interested in, following the pattern used for the other chips. It can
handle both wide and narrow DIPs. At the end of the file, list the
chips that you want (repeating the name if you want multiple copies),
and the script should lay them out for you. If the sizing/spacing
isn't quite right for you, adjust the constants.

Make sure you print at 100% scale precisely, if you want everything to
line up.

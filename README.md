# Scorpion

This is the code for a Lego Mindstorms NXT 2.0 scorpion.

## Behaviour

The code is very simple. I was only interested in the sting mechanism
so this is the only behaviour this program implements (it has no
legs).

The UltraSound sensor should be plugged into input 1 and the sting's
motor into output A. At the moment, it assumes that the sting starts
in the closed position (I may add a setup step that pulls the sting in
first at some point).

## Construction

My scorpion is based on [a design found on
active-robots](http://www.active-robots.com/download/Build-Spike.pdf). I've
ditched much of the design, in particular the legs. Unfortunately,
these instructions require pieces that don't appear to come in the
default NXT 2.0 kit. My kit only contains two 15-length pieces, which
is less than the sting mechanism requires. I got around this by
scaling down the size of the sting by replacing 15-length pieces with
13, 13 with 11 and so on.

## Usage

You'll need to build a suitable machine out of the Mindstorms kit. You
can then connect it to your computer using a USB cable.

If you haven't done so already, get set up with the following steps:

* [Set up the NXC platform](http://nxc.ruby4kids.com/Downhome/Topic1)
* [Configure USB (Linux)](http://bricxcc.sourceforge.net/nbc/doc/nxtlinux.txt)

Then, with the nbc command set up and on your path, run the following
from the `scorpion` directory.

    nbc -d scorpion.nxc

This will compile the program and send it to the connected NXT device.

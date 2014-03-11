zotac-xbmc-link
===============

A link between a Zotac AD10/AD11 (Philips/NXP) remote control and XBMC


Some random facts I learned spelunking through the XBMC code:

* When sending Button events, "R1" really means "remote with named buttons" and "R2" really means "RCA code remote". The documentation has these as "Xbox Remote" and "Xbox Universal Remote" which is confusing.
* The Wiki page for the EventServer really isn't all that useful. You need to read the C++ header file and the ButtonTranslator.cpp file from the source code to understand what to do.
* There's not a lot of error checking or reporting in the network/EventClient.cpp file in XBMC, so if you get something wrong, it will just be silent.


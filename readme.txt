
Version: 2016-09-21

This folder contains...

* 8983 groundnet.xml files (parking locations for > 8400 airports)
with AI taxi routes for  1400 airports.
(made with aptdat2sqlite.py && sqlite2xml.py)
including 88 "legacy" groundnets that were made with TaxiDraw

* jetways.xml files for 259 airports.
(made with dsf2stg.py )

Make sure you have enabled AI-> Jetway Settings -> Enable animated jetways

I suggest to put this Airports folder into a custom scenery folder. (next to it's Objects folder)


WARNING:
* use at your own risk!
* make a backup of your existing Airports folder
* this package does not contain ils,twr,threshold files!
* at some airports you will see duplicate jetways: shared objects form the stg file and the AI jetways from this package.
* the jetways will not fit exactly to the buildings
* at some airports you'll see jetways but no buildings because nobody made the terminal buildings yet.
* the numbers on the jetways are not the gate numbers - they help to identify a jetway in the xml file

https://github.com/mherweg/d-laser-fgtools
http://wiki.flightgear.org/User:Laserman

http://wiki.flightgear.org/index.php?title=Howto:Animated_jetways

included in this package:
http://wiki.flightgear.org/Ground_networks_from_apt.dat

also included in this package:
http://wiki.flightgear.org/Airports_with_ground_networks


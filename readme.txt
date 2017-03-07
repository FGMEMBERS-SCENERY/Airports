new Version: 2016-12-25
https://github.com/mherweg/Airports

only on github, not yet in Terrasync




source: /xp11/Resources/default scenery/default apt dat/Earth nav data/apt.dat (February 2017)
number of airports with parking locations: 9335
number of AI ground networks: 1722

source: /xp11/Custom Scenery/Global Airports/Earth nav data/apt.dat (February 2017)
number of airports with parking locations: 3764
number of AI ground networks: 1672



This folder contains...

* ICAO.groundnet.xml files 
with AI taxi routes.
(made with aptdat2sqlite.py && sqlite2xml.py)
including a few groundnets that were hand-made with TaxiDraw

* jetways.xml files
(made with dsf2stg.py )

Make sure you have enabled AI-> Jetway Settings -> Enable animated jetways
In some versions of FlightGear the AI Jetways are broken, you'll see a Error message about "runtime-jetways"

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
(the 2 lists on the wiki are not always up to date)

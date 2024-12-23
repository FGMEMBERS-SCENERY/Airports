To install airport parking, after unzipping the files, remove "master" from Airports-Master so your airport files are in the file named Airports. This is important as it is the only way flightgear will recognize it. Create a folder someplace on your system (not in any FG files or folders), name it whatever you want, so you will know what it is. 
example (Airport Parking)
 Then create a file system like this:
					Airport Parking\
					       Airports\
					  airport files (1 to 0 and a to z) 

These are the parking files. Then open flightgear, and in add-ons\additional scenery folders, select add, and direct it to the file named Airport Parking, it must be done this way or it will not work.





new Version: 2017-03

local "push" repo:  i3:~/d-laser-fgtools/Airports
remote repo: https://github.com/mherweg/Airports

only on github, not yet in Terrasync


source 1: /xp11/Resources/default scenery/default apt dat/Earth nav data/apt.dat (February 2017)
total number of airports (without heliports & seaports): 28110
number of airports with parking locations: 9335
number of AI ground networks: 1722

source 2: /xp11/Custom Scenery/Global Airports/Earth nav data/apt.dat (February 2017)
total number of airports (without heliports & seaports): 3971
number of airports with parking locations: 3764
number of AI ground networks: 1672
... I think those are updates to the "big" apt.dat


This folder contains...

* ICAO.groundnet.xml files 
with AI taxi routes.
(made with aptdat2sqlite.py && sqlite2xml.py)
including a few groundnets that were hand-made with TaxiDraw

* ICAO.jetways.xml files
(made with dsf2stg.py )

Make sure you have enabled AI-> Jetway Settings -> Enable animated jetways
In some versions of FlightGear the AI Jetways are broken, you'll see a Error message about "runtime-jetways"
This can easily be fixed in jetways.nas

I suggest to put this Airports folder into a custom scenery folder. (next to it's Objects folder)

PATH-TO/myscenery/
					/Objects
					/Airports
					/Models
         
         
         
fgfs --fg-scenery PATH-TO/myscenery



WARNING:
* use at your own risk!
* do not overwrite your existing Airports folder
* this package does not contain ils,twr,threshold files - you have them already.
* at some airports you will see duplicate jetways: shared objects form the stg file and the AI jetways from this package.
* the jetways will not fit exactly to the buildings
* at some airports you'll see jetways but no buildings because nobody made the terminal buildings yet.
* the numbers on the jetways are not the gate numbers - they help to identify a jetway in the xml file


most of the groundnets were converted from apt.dat with: aptdat2sqlite.py && sqlite2xml.py
the jetway xml files were converted from .dsf files (gateway scenery packages) with dsf2stg.py
see:
https://github.com/mherweg/d-laser-fgtools
http://wiki.flightgear.org/User:Laserman
http://wiki.flightgear.org/index.php?title=Howto:Animated_jetways

http://wiki.flightgear.org/Ground_networks_from_apt.dat
http://wiki.flightgear.org/Airports_with_ground_networks
(the 2 lists on the wiki are not always up to date)



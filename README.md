TODO: some updates need here. Also to clarify exact role of this repository.


# TripleA Maps Project

* Map Making: https://github.com/triplea-maps/Project/tree/master/MapMakingTools
* Admin Setup: https://github.com/triplea-maps/Project/tree/master/bin
* Game engine: http://github.com/triplea-game/triplea


## How to play a map pre-release
Three ways:
1. If the map is officially part of the maps project, then look for the releases section of the map, and then look for the zip file download link. Example:
* https://github.com/triplea-maps/world_war_ii_g40_balanced/
* https://github.com/triplea-maps/world_war_ii_g40_balanced/releases

2. You can also go to the main page of the map, and click "clone or download", and save the map repo as a zip. Then extract the contents of that zip into the triplea 'downloadedMaps' folder (you can set this path from within the game via the settings window)

3. You can do a 'git' clone of the map repo directly to 'downloadedMaps'


## How to Report a Problem with a Map

* In-game:
  * Click the downloads maps button to open the downloads map window
  * select the 'installed' tab, find the map ands select it
  * click the 'submit feedback' button
* Alternatively, find the map here:http://github.com/triplea-maps
  * Click through and then look for the "issues" link, and then click "new"

* Filling out the issues form:
  * Describe the problem, be specific

* Game bugs should be reported with the game engine: http://github.com/triplea-game/triplea/issues/new

# Map Maintenance


* Download (clone) all of the map repos: https://github.com/triplea-maps/Project/blob/master/bin/clone_all.sh

## Useful commands:

```
## search for text
grep -r "search_text"

## search for text and only display the names of the files that match
grep -lr "search_text"


## search XML files, and for each one search for text. 
## This is a much faster version than 'grep -r' which goes over image and binary files
## The "-H" forces the file name in grep. "-h" will suppress. The forced file name is to mimic
## the behavior of 'grep -r' via using the find command.
find . -name "*xml" | xargs grep -H "search_text"
```

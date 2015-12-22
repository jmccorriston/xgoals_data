#This repository contains all play-by-play shot data from the 2007-08 season through the 2014-15 season. It is the data used to produce the statistics at www.fourthlineheroes.com.

##Roadmap:

accuracies/ - The league average shot accuracies at each distance for different game states

goalie_results/, player_results/, team_results/ - Results from the expected goals experiments explained at www.fourthlineheroes.com

play-by-play/ - Shot attempt (excluding blocked shots) and faceoff data for each season. Eventually I want to separate these into 1 game per file, but the game ID at the in the first column can be used to identify different games for now.

times/ - Time on ice for at even strength or on special teams for each player in each season.

id_mappings/ - Several JSON dictionaries that store unique integer IDs for each player and the mappings between these IDs and various forms of player strings that exist in the play-by-play data. The strings in the play-by-play data are different for each of a) the shooter on a given shot event, b) the goal scorer and assisters when a goal is scored, and c) who was on the ice for each event. Additionally, player names are inconsistent from year to year (e.g. Ovechking changes back and forth between Alex and Alexander). These IDs offer a unique way to identify a player that is robust to these differences.
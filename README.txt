Readme for DCS Multiplayer Bombing Range / Jet Golf

This script allows for up to 30 people to play in multiplayer. It has the following features

1. Live scoring - every bomb dropped is scored by distance to target and direction from bullseye, e.g. 23m @ 3 o'clock. The direction is in relation to the aircraft's attack heading at the point of release. This message goes to all players in real time. 
2. Players can view their bombing history via the F10 radio menu
3. Players can view all players summarised results, also via the F10 radio menu. 
4. Like golf, fewer points are better. Your points are total distance for all munitions dropped across the round. Least points wins. 
5. Results can be cleared via F10 if you want to start over. 
6. Works for all munitions except cannon. Note, if you drop more than one per hole, it'll count BOTH which isn't great for your totals. 

There are a few limitations:
1. Due to the way F10 radio menu triggers work, I haven't found a way to record which player / aircraft selected the option, so scorecards viewed this way go to the whole aircraft group, not just the initiating aircraft. Scorecards shown are of the first aircraft to spawn into the group only, for the same reason. On this basis, I recommend setting up groups of one aircraft only. 
2. If using in single player mode, when first spawning in the F10 menu won't appear. Hop back in the jet or select a different aircraft to then see it, or set your aircraft start time in mission editor to at least 3 seconds after mission start time. 
3. Only first 20 bomb drops are displayed in the scorecard. 
4. Munitions that create other munitions (like clusters) will not give good results. 
5. Scores any drop within 1000m of a target. I have not tested what happens for two targets closer than 1000m together, so suggest you either mod the rangescript to be a smaller radius, or set targets further apart than this. Or take your chances, it might be fine!

Two fully built missiona is included, and you can just use these straight away. These are:
1. Bombing range on Caucasus.
2. Jet Golf on Nevada.

Both are loaded with the MIST and rangescript scripts, and kneeboards. Both .miz files should be ready to run straight out of the box. 

I would say these have been reasonably well tested, within the scope of the test missions built. I can't say for sure it'll always work for all maps and circumstances. 

To set up your own range:
1. Add circular trigger zones and name them 'Hole01, Hole02, etc.' If you want to change the target names, update and reload the lua script. 
2. Add a once off trigger at time more than 1s to load MIST. 
3. Add a similar trigger at time more than 2s to load the range script.
4. Optionally, add a smoke marker script that creates smoke markers on your trigger zones (we found it helps to be able to see the targets from a distance, especially for aircraft that don't have stored waypoints). Script should repeat every five minutes as that's how long markers last. 
5. Add any targets you like. Make them immortal or set a script to respawn them if destroyed. 
6. Add your aircraft groups and waypoints. Recommed group start times at least 3s after mission start time. 

This has been a fun project to make, and I hope you enjoy it!


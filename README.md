# cs2config
cs2 config with QOL features such as adjustable sens, dynamic follow recoil, scrollwheel jump lockout, and lots of funny colors

|\IMPORTANT\|
if u plan to use this make sure to check for conflicts with your existing binds. alternatively, save a backup of your existing binds by pulling them from C:\Program Files (x86)\Steam\userdata\$$your_steam_id\730\local\cfg
ive done my best to keep all the binds at the top, but there is 1 major exception. 

by default, desubtick jump will be bound to mwheel up and normal jump will be mwheel down. if you wish to not have scroll wheel jump, be sure to remove ALL instance of the following line:
bind mwheeldown +jump; bind mwheelup +jump_
these binds are also made in alias +resetscroll as part of the mwheel jump lockout. be sure to remove them if you do not want scroll wheel jump.

this is not the most user friendly config in the world, as it is just my personal config. ive done my best to make it simple to use with a quick tutorial when the config is printed in console.  


make sure you start the cfg with 
|\main features\|
adjustable sens: by pressing N, you can toggle between 3 sensitivities. you can change these in the config under sens(1/2/3)int. here, you can also change the hud color for each sensitivity. 

dynamic follow recoil: vanilla follow recoil slowly falls back down to center, following the recoil's recovery. i find this a bit awkward to aim on, so dynamic follow recoil immediately snaps back to center once you're done shooting. 
by pressing J, you can toggle between the 3 follow recoil modes. you will have to double tap to confirm, this is for your safety. it has saved me 1 time so far. you can adjust the colors for each mode in the config, under mode(1/2/3)clr

give commmands: you have the option to download as well givecommands.cfg, this is a cfg for easily dropping yourself guns thru console. instead of typing out "give weapon_ak47", you can just type ak47. i used ai to make the list, so some names are a bit off. theyre based on the internal names, so stuff like m4a4 might be m4a1 or some other oddities. i will eventually make this list more thorough, i used to have a better version of this i hand made but sadly it is lost to time. 

scrollwheel jump lockout: you ever shot at someone and fat fingered your mheel down, getting you killed? me too, this solves it. when you press m1, your mwheel will be unbound. when you press space, it will be rebound to jump. 

left hand knife: you can press K to swap your knife into your left/right hand. by default, your "knife key" is set to 3. you will have to manually add a right/left hand bind to each of your other slots, if you want them to be different. i prefer knife left and everything else right, but you do you. you can use shr/shl to do this with a lot less typing, eg "bind 1 slot1; shr". 

funny colors: while messing with the config, you will see the hud changing colors. it also changes colors on a loop, assuming you also downloaded hudanim.cfg. it switches between the color for your chosen follow recoil mode and chosen sens. the blinking will pause while shooting, and resume once you unlock your scrollwheel by jumping. you can disable this functionality entirely and have it perma blinking by editing the alias +pls and removing "alias animtest ; atv;"

|\aliases to be aware of\|
dallas/chicago: instantly connects to respective WaSe dm server
simp: quick setup for show impacts, default impact time is sv_showimpacts_time 0.7
mpresp: a bind i made specifically for training_aim_csgo/cs2, enables respawns for both teams, knife pickups, and gives you a 2nd knife (on TAcs2 when u swap sides it takes away ur knife)
+jump_: desubtick jump
aimbotz: loads up aim_botz
cfg: reloads the cfg. very helpful when making edits. 
shr/shl: shorthands for switchhandsleft and switchhandsright. you will thank me if you setup left hand knife


|\todo list\|
better organize things
make helpcfg actually helpful
add binds to swap directly between recoil modes, maybe even slot specific. you can kinda already do this by binding like "slot1; sprt11", but id like to make a more user friendly way to do this. 
make more map aliases (they r a lil annoying now)
make more easily configureable 
clean up trash/leftover commands from previous stuff i may have been experiementing with
clean up alias names, make things more readable, rename the hudanim stuff from "animtest" xd

# NastyPS2Script

PS2 aint there it sud be regarding to cheats prevention, and now that alot of new players have gotten into it. There sud be more awerness regarding this matter!
Some days ago there was a stream which discussed "Casual to competitive", i think the game aint ready to take that step yet. Theres are things that needs to be adressed before thinking about real competitive gameplay. Well in the meantime, competivtive could be hold on a server with monitoring. doing it to all server is to soon.
Theres no "police" yet.

Also what about ps4? Its harder to cheat on that platform than on pc, due to its platform.

Anyway below is a script i made to make things alot easier in the game, to be honest ive been using it when my kd has been looking bad. But i want everyone to know how easy it is to cheat in the game.
No 3rd party detection, makes it easy having a script running in the background. PS. i havent shared this script with anyone yet, only people with link will see this. Dont wanna ruin the game, so i want you to know how some of the basic cheats work and how to easy detect them.



The only file available to look at here is the config, due to me not wanting to destroy the game.

*{                                                               
  "AutoSpot": true,  
  "WhenToSpot": "Auto", //Random, OnFire, Auto  
  "LosingShield": false, //Detect shield precent? 
  "LosingHealth": true, //Detect health precent?  
  "ShieldPercent": "5%", //On what shield percent to perform action                                                             
  "ShieldAction": "ToggelAbility", //Perform action on preset percent; ToggelAbility will use your abilty(medic will use heal abil, heavy overshield and infli invis)                                                                                              
  "HealthPercent": "90%", //On what health percent to perform action                                                          
  "HealthAction": "ToggelAbility", //Perform action on preset percent; ToggelAbility will use your abilty(medic will use heal abil, heavy overshield and infli invis)                                                                   
  "AimBot": false, //tells it self  
  "AimAt": "Stomach", //where script sud target; Stomach, Fot, Head, solid body  
  "Terminate": "Never" //When the script sud auto close  
}*

You can simply decide what you wanna use. everything of these parameters are 3rd party.
Like spotting i making the script send keyboard inputs, LosingShield and Health is just video feed from screen where a lib named opencv detect how much blue or green there are in the selected cordinates on screen.
Aim is using opencv to grab image files from a folder and try to find a place where it match. if the image match will make the mouse move to center of folder image.

Heres a small example on how to autospot.
This script only shows the spotting method:

![Spotted](http://wiad0api.tk/Delete%20in%202%20months/SkjermbildePS2.PNG)

But you dont even need that, simply just having a while loop which press 'q' works to, however its messing up if you wanna type in chat.

![Spotted2](http://wiad0api.tk/Delete%20in%202%20months/se.PNG)

As simple as 4 lines will make it so you dont have to click a button ever. Is this how we want the game?



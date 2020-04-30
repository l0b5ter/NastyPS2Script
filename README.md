# NastyPS2Script

PS2 aint there it sud be regarding to cheats prevention, and now that alot of new players have gotten into it. There sud be more awerness regarding this matter!
There was this stream which discussed "Casual to competitive", i think the game aint ready to take that step yet. Theres are things that needs to be adressed before thinking about real competitive gameplay. Well in the meantime, competitive could be hold on a server with monitoring. Doing it to all server is to soon.
Theres no "police" yet.

Also what about ps4? Its harder to cheat on that platform than on pc, due to its platform.

Anyway below is a script i made to make things alot easier in the game, to be honest ive been using it when my kd has been looking bad. But i want everyone to know how easy it is to cheat in the game.
No 3rd party detection, makes it easy having a script running in the background. PS. 'i havent shared this script with anyone yet', only people with link will see this. Dont wanna ruin the game, so i want you to know how some of the basic cheats work and how to easy detect them.



The only file available to look at here is the config, due to me not wanting to destroy the game.

*{                                                               
  "AutoSpot": true,  
  "Spot": "Auto", //Random, OnFire, Auto  
  "LosingShield": false, //Detect shield precent?                                                                     
  "LosingHealth": true, //Detect health precent?  
  "ShieldPercent": "3.3", //On what shield percent to perform action                                                             
  "ShieldAction": "q", //Perform action on preset percent;                                                                              
  "HealthPercent": "1.5", //On what health percent to perform action                                                          
  "HealthAction": "å", //Perform action on preset percent;                                                                
  "AimBot": false, //tells it self  
  "AimAt": "Stomach", //where script sud target; Stomach, Fot, Head, solid body  
  "Terminate": "Never" //When the script sud auto close  
}*

You can simply decide what you wanna use. everything of these parameters are 3rd party.
Like spotting i making the script send keyboard inputs, LosingShield and Health is just video feed from screen where a lib named opencv detect how much blue or green there are in the selected cordinates on screen.
Aim is using opencv to grab image files from a folder and try to find a place where it match. if the image match will make the mouse move to center of folder image.

Heres a small example on how to autospot.
This script only shows the spotting method:

![Spotted](http://wiad0api.tk/Delete%20in%202%20months/ps2spots.PNG)

But you dont even need that, simply just having a while loop which press 'q' works to, however its messing up if you wanna type in chat.

![Spotted2](http://wiad0api.tk/Delete%20in%202%20months/se.PNG)

As simple as 4 lines will make it so you dont have to click a button ever.




Oki down the the Shield/health part, below is a simple script using the opencv lib. 

![OpenCV](http://wiad0api.tk/Delete%20in%202%20months/OpenCV1.PNG)

Basicly it takes a screenshot of the screen every ms, and see if any of them matches any of the pics in the images folder. Do i need to tell more? I dont think so, dont want people to ruin the game. However you can ask me and i may answer^^
its a landmark file named "shape_predictor_68_landmarks.DAT" which contains datapoints on different shapes, so here its used the draw literal lines around the shield and health bar to get a more clear view of the image.



Ooooof, now we've come to the must discussed part......... This is the aimbot!

![Aim](http://wiad0api.tk/Delete%20in%202%20months/aim1.PNG)

The difference from stomach, fot, head or solid body is not so much in the code. thats just different landmarks and use another detector file.
Here it uses the landmark file again, to get the points around the "faces". The new awesome thing here is the detector file, this file contains jsut some helmets in black/white format. So it basicly first finds the center of the screen, then search for helmets in the screenshot. After that it uses the landmarks to draw a circle around head/helmet, and lastly it will find the center of the head/helmet and move the mouse to that position. Btw i wont share the 2 files!!!!!!!
Helmet file is made by me, so good luck finding it^^


Everything above is written by lobster/loster31345, and i dont stand responsibility for any of it missuse. This was just to let people know that the security in the game is pretty lacking, hopefully you will see this and find a way to improve the game.

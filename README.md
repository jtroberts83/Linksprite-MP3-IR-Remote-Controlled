# Linksprite-MP3-IR-Remote-Controlled
Modified LinkSprite MP3 Sheild code which allows control via any IR remote

On the Player.cpp file there is a function called translateIR() which you will need to update the 0x######### values with your remotes code

To find out what the codes are for your remotes buttons you need to upload this sketch to your Arduino Uno
Then within your Arduino IDE you need to go to the Tools menu and then open the Serial Monitor.
Then push the buttons on your remote that you want to use to control the MP3 playback and you will see your remote codes in the 
Serial Monitor window but the codes wont start with 0x but you just need to append 0x in front of it in the code. like this

 case 0xFFA857:   where the FFA857 was the volume up button code from my remote

I hooked up the IR reciever to Arduino pin 8 as many of the others are used by the Shield.

***The IR Remote and Reciever I am using is this one:  http://www.amazon.com/gp/product/B00KKROUSG?keywords=Arduino%20IR%20Receiver&qid=1457657541&ref_=sr_1_7&sr=8-7

but pretty much any remote should work.

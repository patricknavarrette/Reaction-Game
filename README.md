## Reaction-Game

These are step by step instructions to create your own reaction game using a Raspberry Pi and a breadboard. The game has an LED that lights up at random times as well as two switches, each switch intended to be controlled by a player. When the LED light is turned on, each player should try to press their button as fast as possible, whichever player hits their button first wins the game.

To create this game you will need:
- Raspberry Pi
- Breadboard
- Two male-to-male jumper cables
- Four male-to-female jumper cables
- LED light of any color
- Two push button switches 

Here is a schematic that indicates how I will wire the breadboard to my Raspberry Pi:
![Pic5](/images/pic5.PNG) <br/>

**WARNING!** You could permanently damage your Pi, so read carefully:
- Turn off your Pi when connecting cables to the GPIO ports.
- Use a resistor, the LED will consumer as much voltage as it can. This may damage your Pi.
- Do not bend the GPIO pins.
- Ground yourself electrically before proceeding.

**Step 1** <br/><br/>
Firstly I connected my LED light. You can see the configuration of the wires from the picture below.
![Pic1](/images/pic1.jpg)
I placed a resistor that lines up with the cathode of the LED light, preventing the LED light from drawing a dangerous amount of power from the Raspberry Pi. I placed the male-to-female jumper cable to align with the anode of the LED light, I have that cable connected to GPIO 17 on the Raspberry Pi.
<br/>

**Step 2** <br/><br/>
Then I connected my first push button on the breadboard, you can see the wiring in the picture below.
![Pic2](/images/pic2.jpg)
The first push button is connected to GPIO 2 on the raspberry Pi.
<br/>

**Step 3** <br/><br/>
Then I connected my second push button on the breadboard, you can see the wiring in the picture below.
![Pic3](/images/pic3.jpg)
The second push button is connected to GPIO 3 on the raspberry Pi. All of the components are now wired in the Raspberry Pi, seen from a different angle below.
![Pic4](/images/pic4.jpg)<br/>
<br/>

**Step 4** <br/><br/>
Now we must write the code for the reaction game. The code that I used can be found at [code](maincode). To create an executable python program, you can open a terminal on your linux machine and use the nano text editor. To create a file using nano you can type in the terminal "nano filenamehere.py" .py indicates it is a python file. For instance, for this reaction game I named the file reaction, so to create the file the command would be "nano reaction.py". After that command is entered, the nano text editor will launch and you will be editing the file under whatever name you decide. Then, you can copy and paste the [code](maincode) and exit and save the document. It will now be executable. You can see the file I created as well as what the nano text editor looks like in the screenshots below. <br/>
![Pic6](/images/pic6.PNG)
![Pic7](/images/pic7.PNG)<br/>
<br/>

**Step 5** <br/><br/>
Now that we have the code written and the wiring done, we can execute the program and play the game. To execute a python file from the linux terminal, you just type "python filenamhere.py" which will execute the program. You can see the syntax I used to in the screenshot below.
![Pic8](/images/pic8.PNG)<br/>
<br/>

**Conclusion**<br/><br/>
Your reaction game should now be complete if you follow all these steps. You can see in the video that included below how the game should look when it is completely assembled and functioning properly. <br/>
[Reaction Game](https://www.youtube.com/watch?v=IVRWWWZRkvQ)

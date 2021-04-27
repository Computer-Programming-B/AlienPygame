Alien Pygame
===========
One of Python's great strengths is the number of useful libraries (like Turtle graphics) that are available. In this assignment we will use Pygame Zero, a game making library, to make a simple alien game. We will be working through [this introduction to Pygame Zero](https://pygame-zero.readthedocs.io/en/stable/introduction.html).

Suggested steps to get started:
---------------------------------
1. It will be easiest to do this assignment on replit. If you prefer to work on your Windows PC using IDLE, see [the instructions below](#installing-pygame-on-a-windows-pc-running-idle), but be warned that installing Pygame will require using the command prompt. 
2. Start by forking [this replit](https://replit.com/@MrSimonLowell/AlienPygameBase). "Forking" means making a copy to your replit account. Click the blue Fork button.   
![](ForkButton.PNG)   
3. Run the program. You should see the following output:   
![](StartProgram.gif)    
4. Now we'll make the alien do something when we click on it. Add the following function to your program   
```python
def on_mouse_down(pos):
    if alien.collidepoint(pos):
        print("Eek!")
    else:
        print("You missed me!")
``` 
5. Now when you attempt to click on the alien you should see the results in the console
6. The console is a great place to check if something is working, but we don't want to use the console for our finished game. Now we'll change the picture and add a sound if we clicked on the alien
7. Modify `on_mouse_down` so that we change images and play a sound if we clicked on the alien   
```python
def on_mouse_down(pos):
    if alien.collidepoint(pos):
        sounds.eep.play()
        alien.image = 'alien_hurt'
    else:
        print("You missed me!")
```
8. *More to come!*

Extensions
----------------------------------------------
Feel free to modify the game any way you like. You can add your own art work and other features. Your alien game doesn't have to work or look like any other. Have fun and be creative!

Installing Pygame on a Windows PC running IDLE
----------------------------------------------
1. Installing Pygame on a Windows PC that uses IDLE is not straightforward. It requires using the command prompt to install the Pygame Zero library. If you are comfortable with the command prompt, you will need to navigate to the `Scripts` folder where you installed Python 3. On my system I could navigate to the scripts folder with the command `cd \Program Files\Python39\Scripts`.
2. Now type the command `pip install pgzero`. This is what it looked like after I typed the command to install Pygame Zero:   
   ![](InstallingPgzeroWindows.PNG)
4. Pygame and Pygame Zero are now succesfully installed!
5. Now, go to [this replit](https://replit.com/@MrSimonLowell/AlienPygameBase), click the three vertical dots, and choose *Download as zip*   
![](DownloadAsZip.PNG)   
6. Extract the downloaded folder to the folder where you store your other Python programs.
7. Open `main.py` from the extracted folder in IDLE. You should now be able to run the program. If IDLE was open during the Pygame Zero installation, you will need to close IDLE and reopen it before you can start coding.  

Samples of Student work
-----------------------
*none yet!*

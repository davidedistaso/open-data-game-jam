

Platformer
==========

Your team must have 2 coders, 1 artist, and 1 sound designer

The tutorial will show you how to make this: [Link to the Construct 3 project file](/tutorials/project_files/platformer.c3p)

![](/images/image2.png)
======================

You will make a simple platformer game (think Super Mario) in Construct 3.

Coders
------

1.  One coder should go to [https://editor.construct.net/](https://editor.construct.net/), the other one should read this tutorial and consult the documentation (Google search, Construct 3 Docs, ChatGPT, etc.)
2.  Close the guided tour popup, then click on the “NEW” button
3.  In the popup, leave all options to default and click “CREATE”
4.  Wait for the artist and the sound designer to upload the assets to Miro or to a shared folder
5.  Download the assets to your laptop, unzip them if necessary.
6.  Start from the background. Drag and drop the image into the Construct 3 editor and adjust its size so that it is inside the dashed lines

![](/images/image16.png)

7.  Repeat the process for the main character, platforms, enemies, and coins.
8.  Bonus tip! Remove unwanted backgrounds by double clicking on the object, selecting the bucket tool, adjusting the tolerance to 50 or more, setting the Alpha color value to 0, and then clicking on the background.

![](/images/image14.png)![](/images/image17.png)

9.  Add the “Platform” behavior to your main character

![](/images/image22.png)

10.  Add the “Solid” behavior to your platform
11.  Test the game by clicking the play button. You should be able to jump and move on the platforms using the spacebar and arrow keys. But nothing happens if you collide with an enemy or catch a coin.
12.  In the top bar select “Event sheet 1”. In the event sheet, you can specify conditions which trigger actions. For example, when the player presses spacebar (condition), play a sound (action).
13.  Right click on an empty space and select “add global variable”. Create a new variable called “score” with type “Number”

![](/images/image3.png)

14.  Click on “Add event”, then select your main character and add the event “On collision with another object”.
15.  Next your new event, click on “Add action”, then select the coin object and select the action“Destroy”. ![](/images/image10.png)
16.  Add one more layout called Game Over with a Text object showing the “Game Over” text. This is the screen that your players will see when the main character dies.
17.  Using the same process shown before, add the actions shown in the screenshot below.
18.  Make you sure you add audio actions for each event (collision with enemy, game over, etc.)
19.  Test your game. Coins should disappear when your character collects them, the score should be updated, and a sound should play.

![](/images/image15.png)

Artist
------

Based on the art style that you brainstormed, and on the references you picked on Miro, draw a background, main character, enemies, platforms, and coins. Recommended: you can make your own drawings on a piece of paper and then scan it with your phone.

![](/images/image13.png)

![](/images/image20.png)Upload the assets to your shared Miro, or to a file sharing service like Google Drive, so that the Coder can access them.

Sound designer
--------------

No game is complete without sounds! In the platformer you are making, you will need these sounds:

*   A soundtrack (playing in a loop)
*   Coin collected
*   Game over
*   Jump
*   Walking/running

You have a few options for your sound design:

*   Record your own sounds using a sequencer such as
*   [https://musiclab.chromeexperiments.com/Song-Maker/](https://musiclab.chromeexperiments.com/Song-Maker/)
*   [https://sfbgames.itch.io/chiptone](https://sfbgames.itch.io/chiptone)
*   [https://terrycavanagh.itch.io/bosca-ceoil](https://terrycavanagh.itch.io/bosca-ceoil) (Windows & Linux)
*   GarageBand (iOS and macOS)
*   Make some noise and record it using your phone’s microphone!

Keep in mind the aesthetic of the game that you brainstormed earlier.

Once you have your 4 sounds and one soundtrack, upload it to a file sharing service like Google Drive, so that the Coders can download them.
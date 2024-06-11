Visual novel
============

Your team must have 1 coder, 1 artist, 1 writer, 1 sound designer

The tutorial will show you how to make this: [Link to the Construct 3 project file](/tutorials/project_files/visual-novel.c3p)

![](/images/image4.png)

Coder
-----
One of the quickest ways of making a visual novel in Construct 3 is to create a base layout and duplicate it for every line of the text. In the duplicates, you will customize the text, character, music, etc. The base layout will have a text box, a background, a character, and two buttons (so the player can make a choice). Each button will have an instance variable called GoToLayout containing the name of the layout that should be loaded when the button is pressed. When the player presses the button, we simply load the layout with the name contained in GoToLayout.

1.  Go to [https://editor.construct.net/](https://editor.construct.net/&sa=D&source=editors&ust=1718112108926851&usg=AOvVaw0exkp_QTtoCzmHO7dg_MiY)
2.  Close the guided tour popup, then click on the “NEW” button
3.  In the popup, leave all options to default and click “CREATE”
4.  Select the Layout tab
5.  Right click on an empty space
6.  Click “Insert new object”
7.  Click on “Text”
8.  Using the same process to create objects, create two Buttons, and one Audio object
9.  Change the buttons’ text in the properties section on the bottom left. Write “Option A” in the first button and “Option B” in the second button
10.  For each button, create an instance variable called GoToLayout
11.  Select Option A button and write Layout 2 in the GoToLayout  variable. This means that when the button is clicked, Layout 2 should be loaded
12.  Duplicate Layout 1 and call your duplicate Layout 2
13.  Select Event Sheet 1

![](/images/image6.png)

![](/images/image7.png)

![](/images/image19.png)

![](/images/image24.png)

![](/images/image1.png)

14.  Finally, set up the rest of the events as shown below. Text preceded by // is a code comment explaining what the code does. Before you can implement the Audio actions, you need to create an Audio object. A single Audio object can play multiple sounds.

![](/images/image9.png)

15.  Test that the logic is working by clicking on the play button
16.  Wait for the artists, the sound designer, and writers to upload the assets to Miro or to a shared folder
17.  Download the assets to your laptop, unzip them if necessary.
18.  Import your assets by dragging and dropping them into the Construct 3 window.
19.  Bonus tip! Remove unwanted backgrounds by double clicking on the object, selecting the bucket tool, adjusting the tolerance to 50 or more, setting the Alpha color value to 0, and then clicking on the background.

![](/images/image14.png)

Writers
-------

It’s up to you to decide how to brainstorm your story. Once you have an idea about your dialogue, make a spreadsheet like this, and share it with the Coder, who will implement it into the game.

| # | Text                  | Characters | Background | Soundtrack | Options                                                     |
|---|-----------------------|------------|------------|------------|-------------------------------------------------------------|
| 1 | Hi, my name is Fox    | Fox        | Park       | Park       | Nice to meet you -> Line 2 Do we know each other? -> Line 4 |
| 2 | Nice to meet you too! | Fox        | Park       | Park       |                                                             |

Arists
--------------

Based on the art style that you brainstormed, the references you picked on Miro, and the story that you’re telling in the game,  draw the following elements:

*   Character(s)
*   Text box
*   Background(s)

Recommended: you can make your own drawings on a piece of paper and then scan it with your phone. You can also use a drawing app on a tablet or laptop.

![](/images/image23.png)

Sound designer
--------------

You have a few option for your sound design:

*   Record your own sounds using a sequencer such as

*   [https://musiclab.chromeexperiments.com/Song-Maker/](https://musiclab.chromeexperiments.com/Song-Maker/)
*   [https://sfbgames.itch.io/chiptone](https://sfbgames.itch.io/chiptone)
*   [https://terrycavanagh.itch.io/bosca-ceoil](https://terrycavanagh.itch.io/bosca-ceoil) (Windows & Linux)
*   GarageBand (iOS and macOS)

*   Make some noise and record it using your phone’s microphone!

Keep in mind the aesthetic of the game that you brainstormed earlier.

Start by making the following sounds:

*   A chill soundtrack
*   A tense soundtrack
*   Character speaking noises
*   Button pressed sound

Once you have your sounds, upload them  to a file sharing service like Google Drive, so that the Coders can download them.
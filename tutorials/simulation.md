

Simulation game
===============

Your team will 2 coders, 1 artist, 1 sound designer

The tutorial will show you how to make this: [Link to the Construct 3 project file](/tutorials/project_files/simulation.c3p)

This tutorial will show you how to make a simple game where you run an egg stand. You can buy more hen to get more eggs, see how much money you make, and how many customers show up.

Link to the final project in Construct 3:

![](/images/image5.png)

Coders
------

1.  One coder should go to [https://editor.construct.net/](https://editor.construct.net/), the other one should read this tutorial and consult the documentation (Google search, Construct 3 Docs, ChatGPT, etc.).
2.  Make sure you are on the Layout screen.
3.  To create an object, right click on an empty space and select “Insert new object”.
4.  Create one button and set its text to “Buy Hen” in the properties pane on the bottom left. Set the name of this object to BuyHenButton. Do not confuse the name of the object (under object type properties)  with its text (under properties). The name is used by the developers to refer to the object, the text is what is shown to the players.
5.  Now create four Text objects and set their names to MoneyText, EggsText, CustomersText, abd HensText
6.  Create one Sprite object called HenSprite. When you create a Sprite object, the cursor becomes a cross (+), click anywhere on the layout to place your new Sprite. After you click, the image editor automatically opens so you can draw your sprite. For now, just fill it with a solid color and then close the editor.
7.  In the project pane (top right), inside the folder “Object types” you should see your new sprite. Drag and drop it into the layout 5 times, so that we have a total of 6 instances of HenSprite. It is the same object, but instantiated 6 times. Different instances of the same object share some properties (the drawing), but not others (like the visibility). This means we can show or hide different instances, which will come in handy.
8.  Now that we created all our objects, let’s switch to the EventSheet. In the event sheet, you can specify conditions which trigger actions. For example, when the player presses spacebar (condition), play a sound (action). We can also specify variables to store information and retrieve it later.
9.  You can create variables by right clicking an empty space and selecting “Add global variable”. Let’s create 7 variables: HensAmount, MoneyAmount, EggsAmount, CustomersAmount, EggPrice, HenBuyPrice, HenMaintenanceCost
10.  Now let’s add our first event and actions! Every second we want all the customers to each buy one egg, and then get removed.
11.  Click on AddEvent, then select System, then Every X seconds (use the search bar to find it quickly). Set a 1 second interval. Every second this event will be triggered.
12.  Next to our new event, click on Add action, select system, select “Add to”, then select the MoneyAmount variable and write EggPrice in the value field.
13.  We also need to remove customers once they have made their purchase. Click on Add action, System, Subtract from, select CustomersAmount and write 1 in the value field. Repeat the same process to subtract 1 from the EggsAmount variable. Your event should now look like this:![](/images/image11.png)
14.  But this doesn’t work…we need all customers to each buy one egg! Let’s create a loop. Right click the empty space under your first condition (every 1.0 seconds), select Add -> Add another condition. Select System -> For , leave everything as it is but set CustomersAmount as the End index![](/images/image8.png)![](/images/image12.png)
15.  Add two more conditions to ensure that the customer amount and eggs amount are greater than 0. Now, this event will trigger every second and for every customer in CustomerAmount.
16.  You now know to set up events with multiple conditions and actions, good job! Set up the rest of the events as shown below.

![](/images/image21.png)

Artist
------

Based on the art style that you brainstormed, and the references you picked on Miro  draw the following elements:

*   Background
*   Icons for items to purchase/sell

Recommended: you can make your own drawings on a piece of paper and then scan it with your phone. You can also use a drawing app on a tablet or laptop.

Use Miro or a file sharing service like Google Drive to share your assets with the coders.

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

*   Soundtrack
*   Purchase button pressed
*   Sell button pressed
*   Game over (bankruptcy)

Once you have your sounds,, upload them  to a file sharing service like Google Drive, so that the Coders can download them.
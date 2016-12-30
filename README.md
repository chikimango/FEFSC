# FEFSC
Fire Emblem Fates: Support Coder

A JavaFX program that assists in coding supports for Fire Emblem 3ds games

# How to Compile

> 1. Download IntelliJ Idea
> 2. Create a new JavaFX project called FESC
> 3. Extract the master into the project file and overwrite all files
> 4. Go to *Build -> Build Artifacts* and build FESC as a JavaFX output

# How to Use
The program is relatively straightforward even if you don't have previous knowledge on how to code supports, but I'll be explaining how FESC works below in case anyone needs help. For reference, [here's](http://pastebin.com/0g7jf3i3) a guide on coding supports.


### Character Options:
![Imgur](http://i.imgur.com/3pRe2YW.png)

This is where you choose the names of the two characters who **appear first** in the support. Character 1 will appear on the left of the screen and character 2 will appear on the right. How to handle adding, removing, or replacing characters from the support will be explained in the Effects Options.


### Dialogue Input:
![Imgur](http://i.imgur.com/jqoGkWr.png)

For this all you have to do is write in (or paste) the first line of dialogue from your support into the text box.
**Make sure you do not exceed the box's proportions.** It will allow you to exceed two lines, but only two lines fit in the actual dialogue box from the game (and FEITS). The proportions of the box are the same as the proportions of the game's.

What "Add "\n" if the text wraps" means is that if your dialogue is over one row, then you need to type in "\n" at the beginning of the second row like so:

![Imgur](http://i.imgur.com/s2yeJEl.png)

This is to indicate a newline and is best done after you've finished typing all of your dialogue. If your dialogue goes over the box's proportions after adding the "\n" don't worry, the "\n" will dissapear in-game and in FEITS. What matters is if your dialogue alone goes over the proportions. 

If you don't add the "\n" this is how it'll look in FEITS and in-game:

![Imgur](http://i.imgur.com/zKAkTQ9.png)


### First Line Button & Song Options
![Imgur](http://i.imgur.com/MhsfyVI.png)

**The "first line" button should only be selected if you are on the first line of your support. You only select it once when creating your entire support.** This button will add code to make the game initiallize the characters on the screen and what music is playing. **Again, it is very important that you press this at the beginning of your support or else the support will not work correctly in-game OR in FEITS.**

I think the song options are pretty self-explanatory, you just choose which song you want to play in your support in-game. You can choose none if you'd like, and there are play/pause buttons on the right to sample the songs.


### Character Speaking Buttons & The "Appears Alone" Button
![Imgur](http://i.imgur.com/YVvXkAX.png)

There's not much to expain here, just select which character is saying the dialogue you wrote.

For the Appears Alone Button: This button will only be selectable when you've selected the First Line Button or when you've chosen the "Fade to Black" effect option. You only press this button if the speaking character appears alone during those two instances. **You'll need to initallize the other character in Effects Options _when they first appear_ by selecting "Character 1/2 Appears".**


### Displayed Emotion & Portrait Viewer
![Imgur](http://i.imgur.com/SerRt6h.png)

Not much to explain, here you choose what portrait will display for the speaking character. If the character is blushing or sweating you just select the blush/sweat buttons. You can select both if you want to.

You can view the portraits of the character if you've selected the 1st character or 2nd character buttons by clicking "View Portrait". That will open up this window:

![Imgur](http://i.imgur.com/6LLuY5Z.png?1)

Which displays either the 1st or 2nd character depending on which button you have selected in the character options and the emotion you've selected for them. 
Note: The "Same as Previous Emotion" option is for if you're using the same facial expression (including the blush/sweat) for multiple lines of dialogue. You don't have to use this option if you don't want to, it's just there for your convenience.


### Effects Options & Sound Effects
![Imgur](http://i.imgur.com/FVU9eS8.png)

For the effects options it's important that you remember this: **all of these options will happen _before_ your current dialogue appears. It is important to keep note of this for every option, because if you select an effect at the wrong time it could completely mess up the sequence of events for your support.** 

Options in Effects:

*None (Default)*: Does nothing.

*Screen Fades to Black*: Does what the name implies.

*Character 1 Appears*: Character 1 gets initialized or re-initialized.

*Character 2 Appears*: Same as above except for character 2.

*Character 1 Left*: Note the past tense. This makes character 1 dissapear, if you want them to reapear use "Character 1 Appears".

*Character 2 Left*: Same as above except for character 2.

*Chara 1 Replaced by New Chara*: Character 1 is replaced by a third character that you'll be able to choose.

*Chara 2 Replaced by New Chara*: Same as above except for character 2

*Charas 1 & 2 Replaced by New Charas*: Both characters 1 and 2 are replaced by a third and fourth character.

*Chara 1 Appears & New Chara Appears*: This will initialize or re-initialize character 1, and replace character 2 with a new character.

*Chara 2 Appears & New Chara Appears*: Same as above except for character 2.



The sound effects work like the regular effects do; they all play before any dialogue is spoken. If you choose an effect and want a sound effect to play as well, you can select whether you want the sound to play before the effect or after it. 

If you select "Chara 1/2 Replaced by New Chara" in the Effects options, you'll have the option of selecting the "Damage & Body Fall" sound effect, which is meant for when an enemy is killed and dissapears right away without saying anything. The damage sound effect plays first, then the effect, and then the body fall sound. 

### "Add Line" Button & Support Output
![Imgur](http://i.imgur.com/QoeWozt.png)

When you're finished choosing the options for the dialogue you've inputted, click the "Add Line" button. The program will take your dialogue and code it appropriately. The coded dialogue will be placed into the the area below the button. 
Once you've finished adding all of your lines of dialogue, just copy the finished support and put it into FEITS to see it. 
Be aware though: Even if the support works in FEITS it may not work correctly in the actual game. 

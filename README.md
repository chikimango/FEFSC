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
![Imgur](http://i.imgur.com/MBHa0p7.png)

For this all you have to do is write in (or paste) the first line of dialogue from your support into the text box.
**Make sure you do not exceed the box's proportions.** It will allow you to exceed two lines, but only two lines fit in the actual dialogue box from the game (and FEITS). The proportions of the box are the same as the proportions of the game's.

What "Add "\n" if the text wraps" means is that if your dialogue is over one row, then you need to type in "\n" at the beginning of the second row like so:

![Imgur](http://i.imgur.com/s2yeJEl.png)

This is to indicate a newline and is best done after you've finished typing all of your dialogue. If your dialogue goes over the box's proportions after adding the "\n" don't worry, the "\n" will dissapear in-game and in FEITS. What matters is if your dialogue alone goes over the proportions. 

If you don't add the "\n" this is how it'll look in FEITS and in-game:

![Imgur](http://i.imgur.com/zKAkTQ9.png)


### First Line Button & Song Options
![Imgur](http://i.imgur.com/MhsfyVI.png)

There isn't much to explain here, but it is important. **The "first line" button should only be selected if you are on the first line of your support. You only select it once when creating your entire support.** This button will add code to make the game initiallize the characters on the screen and what music is playing. **Again, it is very important that you press this at the beginning of your support or else the support will not work correctly in-game OR in FEITS.**

I think the song choices is pretty self-explanatory, you just choose which song you want to play in your support in-game. You can choose none if you'd like, and there are play/pause buttons on the right to sample the songs.


### Character Speaking Buttons & The "Appears Alone" Button
![Imgur](http://i.imgur.com/obgejEW.png)

There's not much to expain here, just select which character is saying the dialogue you wrote.

For the Appears Alone Button: This button will only be selectable when you've selected the First Line Button or when you've chosen the "Fade to Black" effect option, which I'll explain later. You only press this button if the speaking character appears alone during those two instances. **You'll need to initallize the other character in Effects Options _when they first appear_ by selecting "Character 1/2 Appears".**


### Displayed Emotion & Portrait Viewer
![Imgur](http://i.imgur.com/SerRt6h.png)

Not much to explain, here you choose what portrait will display for the speaking character. If the character is blushing or sweating you just select the blush/sweat buttons. You can select both if you want to.

You can view the portraits of the character if you've selected the 1st character or 2nd character buttons by clicking "View Portrait". That will open up this window:

![Imgur](http://i.imgur.com/6LLuY5Z.png?1)

Which as you can see, displays either the 1st or 2nd character you've chosen in the character options and the emotion you've selected for them. 
Note: The "Same as Previous Emotion" option is for if you're using the same facial expression (including the blush/sweat) for multiple lines of dialogue. You don't have to use this option if you don't want to, it's just there for your convenience.


### Effects Options & Sound Effects
![Imgur](http://i.imgur.com/GAP3foc.png)

Explaining the effects is going to get lengthy, so first I'll explain the sound effects.
There's an option in Effects for adding sound effects. When you select that option the Sound Effects box will be enabled. Just choose which one you'd like. There's no way to play the options, but I think the names are pretty self-explanatory as to what you should expect. 

Now for Effects, here are all the options for the first box.

> Default Line: Does nothing.

> Screen Fades to Black

> Character 1 Appears: This is really only used if character 2 was initiallized alone.

> Character 2 Appears: Same as above except for character 1.

> Character 1 Left: Note the past tense. This makes character 1 dissapear from view.

> Character 2 Left: Same as above except for character 2.

> Add Sound Effect


The second box has two options.

> No other Effect: Does nothing

> New Character Appears

> Add Sound Effect


First of all, **all of these options will happen _before_ your current dialogue appears. It is important to keep note of this for every option, because if you select an effect at the wrong time it could completely mess up the sequence of events for your support.** 
To elaborate, I said to keep note the past tense in "Character 1 Left". So, let's say you want character 1 to leave after they say "Goodbye". After they leave you want character 2 to say "Wait". You should not choose the effect option when you're on the line "Goodbye", you want to select it when character 2 says "Wait", because the effect will happen before character 2 says anything. That's why it's in past tense.

For the option "Character 1/2 appears", it's a bit different. Because the character is being initialized, you'll want to select it when the appearing character first says something. For example: Character 1 is alone and they say "Hello" then character 2 appears and says "Hello" as well. Since the effect happens before the character speaks, you're going to want to select the effect option when character 2 says "Hello." because if you select it when character 1 speaks, character 2 will appear prematurely.

**Note: If you chose "Character 1/2 Left" and want them to reappear later, you have to choose "Character 1/2 Appears".**

On "Screen Fades to Black": This will reinitialize all the characters, so if you want to add a new character or switch characters **do it when you select this option.** Remember, the screen will fade to black BEFORE the dialogue appears. Don't select it too early.

For adding/switching characters anytime: When you want to switch in a new character you need to first choose the option "Character 1/2 Left" in the first option box, and then choose "New Character Appears" in the second box. This will make a third character box appear. Choose the new character there, the characters will switch places accordingly. If you ever want the old character to reappear, just do the same exact thing except choose the old character in the third character box.

And that's it for effects.

### "Add Line" Button & Support Output
![Imgur](http://i.imgur.com/QoeWozt.png)

When you're finished choosing the options for the dialogue you've inputted, click the "Add Line" button. The program will take your dialogue and code it appropriately. The coded dialogue will be placed into the the area below the button. 
Once you've finished adding all of your lines of dialogue, just copy the finished support and put it into FEITS to see it. 
Be aware though: Even if the support works in FEITS it may not work correctly in the actual game. 

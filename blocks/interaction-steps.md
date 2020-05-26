# Interaction steps

## Speak Block

### Overview
The Speak block allows you to output speech and audio for the user. With the Speak block, you can have your assistant talk to the user in a variety of voices, as well as play audio files.

<img src="https://i.imgur.com/eAXfWMP.png" alt="img" style="zoom:80%;" />

### Speak block basics

To output speech, drag in a Speak block and click on it. On the far left panel, you'll see a text box where you can enter text to output to the user.


You can type anything!

<img src="https://i.imgur.com/sInuhYe.png" alt="img" style="zoom:50%;" />

### Using different voices

With the Speak block, you may use several different voices - categorized by accent region. When you drag in and click on a Speak block, you can type in the text you would like to output, and then choose the voice you would like to be used.


### Multiple Voices in One Speak Block
Within one Speak block you can say several things in different voices. Below, you can see output in two sentences - each in a different voice by adding another section. 


### Using Variables in the Speak Block
You can use variables within your speak blocks to personalize the user's skill experience, or convey dynamic information such as the answer to a calculation, or an API response. 

To use a variable in the Speak block, hit the right facing curly brace button '{' which will pop the drop-down list for available variables to use in your speak block. 


You can use multiple variables in a single Speak block.

### Playing Audio Files
Using the Speak block you can have play short audio files for the user. To do this, within the Speak block hit "Audio".



When you do this, you'll create a new section for an Audio file which will be played in order with your Speak block sequence, or at random if you have that option toggled. 
Here, you can upload an audio file to be hosted on Voiceflow, or, you can link to a file you are hosting on your location. 

Once you have added a file you will see the length of the file, and be able to preview the sound. You are able to traverse through your audio file by clicking on different parts of the audio player.

<img src="https://i.imgur.com/prUJMzb.png" alt="img" style="zoom:50%;" />


### Alexa specific limitations:

Files for the Speak block can only be up to 240 seconds if uploading to Alexa, and will be played at a reduced sound quality due to Alexa technical restrictions.

When using the speak block, if you were to use back to back blocks with audio uploaded, the audio time within them is added. This is because all blocks will process concurrently until the user is faced with user input (i.e. choice block, interaction block, etc.) The limit applies to the total, until there is user input, then this limit resets.
For example: using two back to back speak blocks with 2 mins and 3 mins wouldn't work, because that would total five mins. But using speak/choice/speak would, because the time is 'reset' after user input.


### Outputting Random Speech
You can output a random 'section' from within your speak block. For example, if you were to have two different greetings, or two different sound effects, you can output a random one to play, rather than play all the sections in sequence as a normal Speak block does.

To do this, hit the three dot button and select "Randomize Outputs". To reset to sequential outputting, hit the three dot button and select "Unrandomize Outputs".



### Change the Vocalization of Your Text with SSML Tags
To output different sounding speech, you may use SSML tags within you Speak block. SSML is a special format created to modify how voice assistants talk.

We have an in-depth tutorial on using SSML tags here.

## Choice Block

### Related articles

- Intents and Slots

### What Are Choice Blocks?

Choice blocks allow you to ask users to make a choice from a pre-defined list of choices. If the user says one of the choices listed in the choice block, it will follow that choice's path. If the user says something that isn't one of the listed choices, the user will follow the ELSE path.



<img src="https://i.imgur.com/wLosZqO.png" alt="img" style="zoom:50%;" />



### Adding Choices

To add choices, drag the choice block out from your block menu onto the canvas. You will automatically have a single choice ready. Select an intent from the drop down list to complete your choice block. 



<img src="https://i.imgur.com/W2dxMRF.png" alt="img" style="zoom:50%;" />



To add more choices to your choice block, hit the "Add Path" button and select and intent. You should see there are now multiple paths on the choice block, one for every path that you have defined.





<img src="https://i.imgur.com/HUI6JL6.png" alt="img" style="zoom:50%;" />



ELSE Port

If the user responds with something that is NOT one of the listed choice options, then the ELSE block port will be activated. For example, if the user was to say "Zebra" as a response choice block asking the user for a "Yes" or "No" answer, it would trigger the ELSE path. This is because "Zebra" is not close enough to "Yes," "No," or any of their synonyms to trigger either path.



Using ELSE As An Error Handler

You can use the ELSE on a Choice block as an "Error Handler". The Error Handler will repeat the available options back to the user, and ask them to choose again. This allows you to ensure they are always choosing from the available options on the list.



<img src="https://i.imgur.com/riGC5jE.png" alt="img" style="zoom:80%;" />


### **No Reply Response**

If Alexa fails to map whatever the user says to any intent defined in your skill, the No Reply Response occurs. For instance if the user says nothing, gibberish, or *words that aren't part of any intent*, it does not map to an intent. A reprompt needs to be defined with the last outgoing message and the Voiceflow service receives no information when a reprompt happens.

We send out each choice with the default reprompt of the last spoken thing. So if you have a speak block "What color do you like?" followed by a choice block, and Alexa fails to map to an intent, it will simply repeat "What color do you like?"

However, Voiceflow allows you to define custom No Reply Response if you don't want it to repeat the same thing. This can be done on any choice or capture block.

![img](https://cdn.zappy.app/3338a4aa21d08c5812a917125adee5cd.png)

![img](https://cdn.zappy.app/5d68320e17c50f63053b733d68fb94a9.png)

No Reply Response only occur twice and will exit the skill if it still doesn't understand the third time.

## Intent Block

### What Are Intent Blocks?

Intent blocks allow you to add shortcuts within your project. With Intent blocks, a user can say an intent at any point within the skill (or outside the skill) and "jump" to that point in the project.

For example, you could add an intent for 'Home' which allows the user to always return to a home menu using the Intent block. Or, you could use a Intent Block to jump to a new place in an interactive story ⏤ the use cases are endless.

### How Intent Blocks Work

![img](https://i.imgur.com/EKWwRiL.png)


Intent blocks only have one outbound port because they do not take an input to be activated. The Intent block is constantly listening for it's keyword or key phrase to activate the block. To setup an Intent block:

### How intent blocks know what to look for

Intent blocks need to be filled with an Intent. Your Intent block will be listening at all times for a users input that matches the intent that is specified.

Intents must be chosen in the drop down menu.

![img](https://i.imgur.com/yObEE40.png)

### Jumping around inside a project
Intent blocks allow you jump to specific points inside a project without having to be connected by lines to other blocks. This allows you to jump to an intent block at any point in your project.

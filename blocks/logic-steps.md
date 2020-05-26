# Logic steps

## **If Block**

### What is an IF block?



The IF block acts as a check to see if a value has met certain conditions or not. If it meets a condition, the skill will execute down the corresponding path.



![img](https://i.imgur.com/FEPJQsF.png)





### IF block example



The IF block can be used to make comparisons of things like numbers or words. You can use it to see how many sessions a user has. If it is a users first time in an app, their session can be checked if it is equal to 1 and they are sent down one path. If they have more than 1 session, they can be sent down another path.



<img src="https://i.imgur.com/btVJVPl.png" alt="img" style="zoom:50%;" />

![img](https://downloads.intercomcdn.com/i/o/109611856/b299beb2e125ac2b8fd9c739/Screen+Shot+2019-03-18+at+5.00.17+PM.png



### Maximum number of options

Within the IF block you can create conditions. These conditions are numbered and will be evaluated in numerical order. You can create up to 20 different conditions within a single IF block.





Each IF statement you add has a number beside it which corresponds to the number on the IF block. The '1' Statement corresponds with the '1' port on the IF block.



![img](https://downloads.intercomcdn.com/i/o/109612987/ac31208c72571bfc4a294180/Screen+Shot+2019-03-18+at+5.06.08+PM.png)



If the condition we put in the #1 Statement is evaluated as true then the IF block will take the user down that path. If statement #1 is not true, then statement #2 will be evaluated next and so on. If there is no match after running through al the conditions then the user will be taken down the ELSE path.



### Adding paths

To add paths, hit the add If statement button and create a new condition to compare against.

<img src="https://i.imgur.com/JXTm7SS.png" alt="img" style="zoom:50%;" />

## **Set block**

### About the Set block

The Set block is used to set and change the value of variables. You can set variable values to numbers, or words. 

The Set block can have its value set through entering a value, or performing an equation. You can set multiple variables within one Set block.



### Using the Set block

Variables are automatically set to the value '0' on creation. When a Set block is activated, the variable it is setting will be changed.

We can use the Set block to change the value of a variable. Below are several examples.

Example 1 We increase the value of a user's {score} variable when they choose the correct answer in our quiz game. In this case we are setting a variables value to its current value, plus one. 

![img](https://i.imgur.com/qC3FM6v.png)

Example 2 We multiply two user inputted numbers together to perform a multiplication function for them, and store the answer in a new variable called answer. In this case we are setting a variable to the value of other variables multiplied together.

![img](https://i.imgur.com/qRiF6I2.png)

### Setting multiple variables at once

You can set multiple variables at once by clicking on the "add variable set" button.

![img](https://i.imgur.com/e6yLNtz.png)

You can set as many variables as you'd like within a single Set block. Set blocks start from the top variable Set and work downwards. Meaning you can override previous variable sets within the same Set block.

## **Capture Block**

### What the Capture Block Does

The Capture block allows you to capture the user's response into a variable. Once this response is stored in the variable, you can use this value throughout the rest of the skill. 

- i.e. You can ask the user what their name is using a Speak block, then follow that up with a capture block to capture the user's name into a name variable. You could then use the user's name throughout the rest of the project. this is a gchange to demonstrate github.

![img](https://i.imgur.com/51vqxXZ.png)



### How to use the capture block 



The capture block takes in users input and saves it to a variable. The type of input must be defined by selecting the Slot type. 

You must also store what the user says into a variable. Variables can be selected from the "Select Variable" drop down. 

<img src="https://i.imgur.com/Quw8vEV.png" alt="img" style="zoom:50%;" />



A completed capture block looks like the following:

<img src="https://i.imgur.com/V3Do8nY.png" alt="img" style="zoom:50%;" />

### No Response

If the user does not respond, a response can be given to prompt them to be asked again. Hit the three dot menu and select "No Reply Response"

There are two types of input for this response:

1. Text to speech

<img src="https://i.imgur.com/QUOtviH.png" alt="img" style="zoom:50%;" />

2. Audio

<img src="https://i.imgur.com/BcaCQNY.png" alt="img" style="zoom:50%;" />

Similar to every other audio upload in Voiceflow, you can upload your own file or link to an audio file URL hosted on the internet from services like Dropbox or Google Drive.

## **Random Block**

### What is the Random block?

The random block allows you to randomize where the user is taken in your flow.

You can setup multiple paths and when the Random block is activated, the user will head down a random path. The Random block does not say anything to the user and will simply choose a random path.

![Imgur](https://imgur.com/g5FJzva.png)

Above, the user would be sent to a random option of the 3 available paths.

### Adding random options

To add random options, click 'add random option'. 

![Imgur](https://i.imgur.com/iX34fup.png)

To remove a path, click the 'remove path' button. If all the paths are not connected to an option, there is a chance that the random option will hit an option without a connection, and end the skill as result.

### No duplicates - don't go down the same path twice

The no duplicates option makes the user not go down the same path twice if the same random block is activated multiple times. 

![img](https://i.imgur.com/YG8T61X.png)

For example, if there are 3 random options, the no duplicates option will not activate the same path twice in a row until all of the options have been taken. Once all the options have been hit, the Random block will reset.

## **Exit Block**

### What the Exit Block Does

The name is self-explanatory, but when executed, the Exit block will exit the skill. The skill will end immediately without any text playing. Its use is very convenient to **leave the skill from a flow** (by default, the flow will return to the last place from which it was used).

<img src="https://i.imgur.com/ECM6kym.png" alt="img" style="zoom:50%;" />


### When the exit block is not needed

The exit block is not needed to exit your skill everytime. The exit block will only ever be needed when you want to force an exit from within a flow. Exit blocks are not needed on the HOME flow to exit your skill.



### Using the exit block

To use the exit block, add it to the end of a flow and connect it to the last block in the flow where you want to exit the skill

![img](https://i.imgur.com/KHpO49I.png)

## **Flow Block**

### What are flows?



A flow is a set of blocks in Voiceflow organized within a single canvas. When you are working on Voiceflow, everything you can see on the canvas is all stored within a single flow. 



Flows can contain other flows, allowing you to stack them and organize thousands of Voiceflow blocks into easy, manageable sections that you can duplicate and reuse.

Flow blocks work like a file system for your projects - you can see this on the left by clicking the flows tab or hitting the Flows hotkey (CMD + > on Mac and Ctrl + > on Windows)

![img](https://i.imgur.com/lCdCmxm.png)



### Flow diagram

Once a flow has been entered, you are shown a version of the start block that carries on from where the flow block beggins. This block acts similary to the standard start block in the ROOT flow but will not be the starting point of the project, only for the specific flow that it is in.

![img](https://i.imgur.com/doEKJSL.png)



### The ROOT flow



The ROOT flow is the main flow for your project. When you start a new project, you will see the ROOT flow as the only flow. You cannot change the name of the flow, or delete this flow. Every flow used will be a sub-flow of the ROOT flow.



There are three settings for each flow block:



- **Rename:** change the name of your flow

- **Duplicate:** duplicate the flow

- **Delete:** delete the flow



1. **Editing flow names** You can edit every flow name except for the ROOT. When you do this, you cannot rename a flow to a name that is already taken. 

2. **Copying flows** When copying flows you will copy just the single flow. For example, if you are copying a flow that has a flow within it, you will only be able to copy one layer at a time. Doing so will produce an exact duplicate of the flow you had copied.

3. **Deleting a flow** When you delete a flow you are deleting it permanently. It is highly recommended you do not delete flows unless you 100% are sure of doing so.



### Flows Menu



![img](https://i.imgur.com/X8CWBhz.png)



The Flows menu has a list of flows as well as a search bar at the bottom that allows you to search through your flows.

**Reusing flows**



You can reuse flows by dragging a new flow block onto the canvas and rather than hitting the 'create new flow' button, you can select from the list of existing flows. You can do this by clicking on your newly placed flow block, and on the right menu you'll see the bar to 'select existing flow'.



![img](https://downloads.intercomcdn.com/i/o/110239689/5a9a905604340395ec69fe80/image.png)



By doing this you'll be able to reuse the flow. If the other flow was in the 'other flows' menu, you will see this flow be taken out of that menu, and placed back into the flow tree according to where you placed your flow block.



### Creating flows



Within the flow block, you can hit the button create flow to create a new flow within your flow tree. If you do not create the flow within the flow block, the flow will not exist in your flow tree and will lead to a dead-end block for the user.



Once you hit 'Create New Flow', you will be brought into a new canvas where you'll only have a start block. From here you can build your new flow.



Once you create the flow, you will see your new flow active on the left flow bar showing your flow diagram. The active flow you are on is always highlighted in blue.



![img](https://downloads.intercomcdn.com/i/o/110239839/ec4f81add1252cb5c30df76f/image.png)



### Local variables in flows



![img](https://i.imgur.com/9AKANpZ.png)

![img](https://i.imgur.com/E8dBXgn.png)

Flows have their own variables called local variables. For example, if you were to have two different flows called 'A' and 'B', each flow would have its own unique set of local variables. This means that you can have variables with the same name, such as {score} in two different flows without them colliding.



Local variables are different than global variables which are accessible throughout your project and will collide between flows



### Sharing local variables between flows



If you want to have local variables shared across flows, you can do so by using the variable mapping feature on the settings bar (right bar when you click on a block) of each block.



Each flow block, except the ROOT flow, can have input, and output variables. Flow blocks can have both, either, or no variable inputs and outputs.



- **Input variables:** local variables being passed into that flow from the flow above it in the flow tree diagram

- **Output variables:** local variables that are passed out of the flow diagram, back into the flow above it in the tree diagram. 

## **Code Block**

### Code Block Overview

The code block accepts a popular programming language known as **JavaScript**. If you don't know how to code, that's alright! Thankfully, there's lots of resources we can use to integrate this block into our skill's logic. 

![img](https://downloads.intercomcdn.com/i/o/109208313/0c2cfde1732a1a448196de06/Screen+Shot+2019-03-15+at+5.09.20+PM.png)

### JavaScript Resources

- [W3Schools](https://www.w3schools.com/js/) - good for learning JS syntax and supported functions
- [Stack Overflow](https://stackoverflow.com/) - good for finding answers to specific questions (must specify that you're using JS in your search).

### Beginner's Example

To store a random number from 0 - 100 in the {random_num} variable put this in your Code block:



```
random_num = Math.floor(Math.random() * 101); 
```

Declare 'random_num' as a variable on Voiceflow. Connect the Code block to a Speak block that states "The random number is {random_num}" and run your project on the Voiceflow test tool. 

![img](https://downloads.intercomcdn.com/i/o/109211439/1b1cf3d2e6f352c8efb1885f/Screen+Shot+2019-03-15+at+5.31.05+PM.png)

I copied this code from [here](https://www.w3schools.com/js/js_random.asp). Easy stuff, right? 

### Advanced Example

To get the current date in (yyyy/mm/dd) format put this in your code block:



```
var today = new Date();
var dd = today.getDate();
var mm = today.getMonth()+1; //January is 0!
var yyyy = today.getFullYear();

if(dd<10) {
    dd = '0'+ dd
} 

if(mm < 10) {
    mm = '0'+ mm
} 

var todaysDate = yyyy + '-' + mm + '-' + dd;
```

Declare 'todaysDate' as a variable on Voiceflow. Connect the Code block to a Speak block that states "The current date is {todaysDate}" and run your project on the Voiceflow test tool. 

![img](https://downloads.intercomcdn.com/i/o/109212317/df18448ad436350ac3687076/Screen+Shot+2019-03-15+at+5.38.39+PM.png)

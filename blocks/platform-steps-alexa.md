# Platform steps (Alexa)

## Stream Block

### What is the Stream block

 The stream block allows you to stream audio files longer than 90 seconds at a higher quality than the audio block. The stream block supports the following file types:

- MP3
- AAC/MP4
- HLS/M4U

You can learn more about the kinds of audio [files supported by Alexa skills here](https://learn.voiceflow.com/build-alexa-skills-without-coding/alexa-skill-audio-files).



![img](https://i.imgur.com/cv3p2Jd.png)

### Stream block vs Audio block

The stream block works very differently than the [Audio block](https://learn.voiceflow.com/build-alexa-skills-without-coding/basic-blocks-tutorials/audio-blocks). Unlike the audio block, when a user hits your stream block - the user is **actually leaving your skill**. This functionality was built-in by Amazon. The user only returns to your skill if they say one of the Stream block's keyword functions. The accepted functions are below:

- Alexa, Pause
- Alexa, Next
- Alexa, Previous

Unless the user says one of these keywords while still streaming audio from the Stream block, your skill will be officially over. This is why it is suggested you use Audio blocks for almost all cases unless impossible. With Audio blocks, the user is still within your skill, and can access Command blocks and other in-skill features.

### Adding audio

To add audio files into the Stream block, you need to add a link to the audio that you want to stream. You can either paste the direct link into the text box or you can save it in a variable and use the variable directly in the textbox. **You must use an https url because it is a requirement to pass the certification of your skill with Alexa.**



![img](https://i.imgur.com/Z56UDCj.png)

### Loop audio by default

When you enable 'Loop audio', you are looping the audio files within the Stream block until the user either stops the skill, or, if you have Audio player functions enabled, asks for an audio player function. This means that the audio will continue to loop until the skill is stopped, or the user asks 'Alexa, next/previous/stop/pause'.



### Audio player functions

 The stream blocks functions can be activated at any time when using the Stream block. For the user to activate a function, they must say the wake word followed by the function they desire (e.g 'Alexa, next').

With Voiceflow, you can determine what happens next when the user says one of the pre-defined Stream block functions by using the next and previous outputs of the block.

When the user is in a Stream block and uses any of the pre-defined functions, they will be routed through the corresponding port. As an example, if the user says 'Alexa, next' while in your stream block - you can use a speak block and connect it to the next port, then have Alexa say the name of the next song before going into another stream block. That looks like this:

![img](https://i.imgur.com/GowDurC.png)


## User Info Block

### What is the User Info block?


The User Info block allows you to retrieve information from a users account and save it into a variable for use in your project. You can retrieve information like the users name, email, location of their device and other informaiton without having to ask the user. This information is pulled directly from the users Amazon account or Alexa device.

![img](https://i.imgur.com/VlbJJrd.png)



### How to use the User info block



The user info block allows you to retrieve one or multiple pieces of information at a time. To add more than one retrieval, click the "Add Request button"

![img](https://i.imgur.com/WwEjpAz.png)



### Supported Information types

Currently, the supportted types of information that you can pull are:



- User email

- User Name

- User Phone Number

- Location

- Whether "Reminders" are enabled

- Whether "Alexa lists" can be read from

- Whether "Alexa lists" can be written to

- Wehther "Notifications" are enabled

- Whether "Skill Personalization" is enabled

![img](https://i.imgur.com/HNj0CXD.gif)

### Check user's permission to set reminders


To start you will need the **User Info Block** to check if the user has authorized reminders permission for your skill. Then, choose **Reminders** from User Info Type.


![img](https://i.imgur.com/AVElTsT.png)


On the User Info's **No Access port**, which means the user has not granted reminders permission yet, link a **Speak block** to explain why you're using the **Reminder block** in your skill and to give the user more informations on how to authorize the skill in the **Alexa app** or on [**alexa.amazon.com**](http://alexa.amazon.com/)

![Imgur](https://i.imgur.com/WblXrnc.png)


![img](https://i.imgur.com/jHj9Zl8.png)

In the following example, I'm using the **reminder_text** variable as the reminder text in the **Reminder block** and I've set the reminder time to notify the user in **one minute**. As for the text, you can also use variables for the Hours, Minutes and Seconds fields.

![img](https://i.imgur.com/0MV3OZR.png)

Add the **Permission block** just after the **Speak block** to end this path. Then, select **reminders** for Permissions Request.

![Imgur](https://i.imgur.com/Xk3tHWQ.png)

You can then link the **Reminder block** on the remaining port of the **User Info block**, which means the user has permitted your skill to set reminders.

![Imgur](https://i.imgur.com/uqCBpt6.png)

### Set a reminder as timer

In the following example, I'm using the **reminder_text** variable as the reminder text in the **Reminder block** and I've set the reminder time to notify the user in **one minute**. As for the text, you can also use variables for the Hours, Minutes and Seconds fields.

![Imgur](https://i.imgur.com/qDGxrhd.png)


After **uploading** your skill to **Alexa**, like your future users, you must allow access to the reminder from the **Alexa app** or [alexa.amazon.com](http://alexa.amazon.com/).

![Imgur](https://i.imgur.com/Nv8ZYQt.png)

Here, I'm using [alexa.amazon.com](http://alexa.amazon.com/) to authorize the skill to access the Reminder.

Click on **Update Permissions**

![img](https://downloads.intercomcdn.com/i/o/124670838/ecb97127757a7a046415278b/Image+2019-05-30+at+3.07.32+PM.png)

Go to **SETTINGS**

![img](https://downloads.intercomcdn.com/i/o/124665726/baff71e4f38031367e5d9139/image.png)

And click on **MANAGE PERMISSIONS**

![img](https://downloads.intercomcdn.com/i/o/124665880/f8eaf5a5a9d6ec7101e2cf1b/image.png)

**Enable** the Reminders and hit the **SAVE PERMISSIONS** button.

![img](https://downloads.intercomcdn.com/i/o/124666239/cb1fbbf7a6b8788b95edfe12/image.png)

![img](https://downloads.intercomcdn.com/i/o/124666138/e7b858496a3b1bea0efe9736/Screen+Recording+2019-05-30+at+03.09+PM.gif)

In another way, you can manage permission on your Alexa app. Permission Block will send a card to Alexa app, which leads the users to allow your skill to access to reminders. You can see a card in home screen of Alexa app or Activity menu.

These are the samples of a card in home screen and in Activity menu. Tap on **Manage** on a home card, or **UPDATE PERMISSIONS** on a card in Activity.

![Imgur](https://i.imgur.com/vh9kg7W.png)

![Imgur](https://i.imgur.com/rLWbzsa.png)

Check the box for reminders and tap on **SAVE PERMISSIONS**.

![Imgur](https://i.imgur.com/xapflHk.png)

Well done, you can now test your skill on a device or from the Alexa application (reminders are not available in the simulator).

### Scheduled Reminder for one-time-only

If you set reminders for one-time-only on the specific date and time, choose **scheduled** and set date and time.

![Imgur](https://i.imgur.com/OG5R85r.png)

Basically, you don't need to set the specific timezone. **User Timezone** will uses the timezone of the user's device.

### Scheduled Reminder for Recurring

Voiceflow also lets you set up automatic reminders to let you send recurring reminders to your users by enabling **Reccurence**. These reminders can be sent daily or weekly on a specific day.

![Imgur](https://i.imgur.com/ANm0T7Y.png)

### Daily

In order to set a reminder to run everyday at a specified time, choose **Daily** and fill in time (in the screenshot below, it is set to 12:00 PM). You don't need to fill in date.

![img](https://i.imgur.com/trl5QpW.png)


Then, set your reminder message and you are good to go with daily recurring messages!

### Weekly

In order to set a reminder to occur weekly, select the **Weekly** and the day you would like your reminder to occur on. In the below screenshot, a reminder is scheduled for every Monday at 12:00 PM Eastern Standard time.


![img](https://i.imgur.com/9JB0Uls.png)

## Card Block


### What the Card Block Does

The card block sends users a card with information to their Alexa app on their phone. All users with an Alexa enabled device will have the Alexa app installed. This block allows you to send both text and images to the users mobile app.

![img](https://i.imgur.com/Ecp4dIm.png)



The card block allows you send to send two typs of cards:

- Simple cards
- Standard cards

### Simple cards

![img](https://i.imgur.com/NzuSyrE.png)



Simple cards allow you to send users a card to their phone with some text. You have the ability to set a `Title` and a `Card Text` for the card that you are sending. It will show up on the users Alexa app looking like the card below.



![img](https://i.imgur.com/5MiPFKl.jpg)

### Standard cards

![img](https://i.imgur.com/QUhXXA3.png)



Standard cards allow for the same functionality as a Simple card but allow you to add an image as well.

Standard cards will show up on the users Alexa app and look like the image below

![img](https://i.imgur.com/Yuxce9g.jpg)

## Reminder block



![img](https://i.imgur.com/HNj0CXD.gif)

### Check user's permission to set reminders


To start you will need the **User Info Block** to check if the user has authorized reminders permission for your skill. Then, choose **Reminders** from User Info Type.


![img](https://i.imgur.com/AVElTsT.png)


On the User Info's **No Access port**, which means the user has not granted reminders permission yet, link a **Speak block** to explain why you're using the **Reminder block** in your skill and to give the user more informations on how to authorize the skill in the **Alexa app** or on [**alexa.amazon.com**](http://alexa.amazon.com/)

![Imgur](https://i.imgur.com/WblXrnc.png)


![img](https://i.imgur.com/jHj9Zl8.png)

In the following example, I'm using the **reminder_text** variable as the reminder text in the **Reminder block** and I've set the reminder time to notify the user in **one minute**. As for the text, you can also use variables for the Hours, Minutes and Seconds fields.

![img](https://i.imgur.com/0MV3OZR.png)

Add the **Permission block** just after the **Speak block** to end this path. Then, select **reminders** for Permissions Request.

![Imgur](https://i.imgur.com/Xk3tHWQ.png)

You can then link the **Reminder block** on the remaining port of the **User Info block**, which means the user has permitted your skill to set reminders.

![Imgur](https://i.imgur.com/uqCBpt6.png)

### Set a reminder as timer

In the following example, I'm using the **reminder_text** variable as the reminder text in the **Reminder block** and I've set the reminder time to notify the user in **one minute**. As for the text, you can also use variables for the Hours, Minutes and Seconds fields.

![Imgur](https://i.imgur.com/qDGxrhd.png)


After **uploading** your skill to **Alexa**, like your future users, you must allow access to the reminder from the **Alexa app** or [alexa.amazon.com](http://alexa.amazon.com/).

![Imgur](https://i.imgur.com/Nv8ZYQt.png)

Here, I'm using [alexa.amazon.com](http://alexa.amazon.com/) to authorize the skill to access the Reminder.

Click on **Update Permissions**

![img](https://downloads.intercomcdn.com/i/o/124670838/ecb97127757a7a046415278b/Image+2019-05-30+at+3.07.32+PM.png)

Go to **SETTINGS**

![img](https://downloads.intercomcdn.com/i/o/124665726/baff71e4f38031367e5d9139/image.png)

And click on **MANAGE PERMISSIONS**

![img](https://downloads.intercomcdn.com/i/o/124665880/f8eaf5a5a9d6ec7101e2cf1b/image.png)

**Enable** the Reminders and hit the **SAVE PERMISSIONS** button.

![img](https://downloads.intercomcdn.com/i/o/124666239/cb1fbbf7a6b8788b95edfe12/image.png)

![img](https://downloads.intercomcdn.com/i/o/124666138/e7b858496a3b1bea0efe9736/Screen+Recording+2019-05-30+at+03.09+PM.gif)

In another way, you can manage permission on your Alexa app. Permission Block will send a card to Alexa app, which leads the users to allow your skill to access to reminders. You can see a card in home screen of Alexa app or Activity menu.

These are the samples of a card in home screen and in Activity menu. Tap on **Manage** on a home card, or **UPDATE PERMISSIONS** on a card in Activity.

![Imgur](https://i.imgur.com/vh9kg7W.png)

![Imgur](https://i.imgur.com/rLWbzsa.png)

Check the box for reminders and tap on **SAVE PERMISSIONS**.

![Imgur](https://i.imgur.com/xapflHk.png)

Well done, you can now test your skill on a device or from the Alexa application (reminders are not available in the simulator).

### Scheduled Reminder for one-time-only

If you set reminders for one-time-only on the specific date and time, choose **scheduled** and set date and time.

![Imgur](https://i.imgur.com/OG5R85r.png)

Basically, you don't need to set the specific timezone. **User Timezone** will uses the timezone of the user's device.

### Scheduled Reminder for Recurring

Voiceflow also lets you set up automatic reminders to let you send recurring reminders to your users by enabling **Reccurence**. These reminders can be sent daily or weekly on a specific day.

![Imgur](https://i.imgur.com/ANm0T7Y.png)

### Daily

In order to set a reminder to run everyday at a specified time, choose **Daily** and fill in time (in the screenshot below, it is set to 12:00 PM). You don't need to fill in date.

![img](https://i.imgur.com/trl5QpW.png)


Then, set your reminder message and you are good to go with daily recurring messages!

### Weekly

In order to set a reminder to occur weekly, select the **Weekly** and the day you would like your reminder to occur on. In the below screenshot, a reminder is scheduled for every Monday at 12:00 PM Eastern Standard time.


![img](https://i.imgur.com/9JB0Uls.png)


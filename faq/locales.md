# Locales

What are locales and why are they important?

Locales define region and language specific features, built in to both Alexa Skills and Google Actions. Locales can be restrictive in that many features are only available to certain countries or languages.

**Resources**

- [Alexa: Locales Landing Page](https://developer.amazon.com/alexa-skills-kit/locales)
- [Alexa: Slot Type Reference](https://developer.amazon.com/docs/custom-skills/slot-type-reference.html)
- [Google System Entities](https://cloud.google.com/dialogflow-enterprise/docs/reference/system-entities)

**Enabling Locales in Voiceflow**

When you create a project, you'll be prompted to choose which locales you'd like to use before beginning. These locales relate to Alexa.

Google allows you first to select languages supported by your skill, then to choose which countries to enable the Action for. Your Actions will work for people in every country who speak a language your Actions support. All settings for Google are done after [uploading your project](https://learn.voiceflow.com/en/articles/2705386-uploading-your-project-to-google-assistant) to Google Assistant.

![img](https://cdn.zappy.app/24419fa3b69b79a0c509253f8a7564a0.png)

Once your skill has been created, you can navigate to the Publish tab in Voiceflow, and scroll down to Locales to edit your choices.


Alexa Skill  

![img](https://cdn.zappy.app/a81d2917b556de9dd8db8c186be9c08b.png)


Google Action  

![img](https://cdn.zappy.app/f8dd39ebb389a37240e10441ed2b6d95.png)

## Updating Locales outside of Voiceflow

Any edits you make within Voiceflow will be saved when publishing, but you can also edit languages (and countries, for Google) outside of Voiceflow.

For Alexa, head to [ADC](https://developer.amazon.com/alexa/console/ask), select your skill, then navigate to the Distribution tab. You'll see a Skill Preview menu on the left hand side, detailing which settings are done for each locale selected.

For Google, head to your [Console](http://console.actions.google.com/), select your action, and you'll see a menu on the left hand side. Under Deploy, choose Location Targeting.

**Common Errors**

- US_First_Name Slot will only work for US, CA, and UK English
- GB_First_Name Slot will only work for US, CA, UK, and DE
- Language support: you can only select languages that you've supported within your skill.
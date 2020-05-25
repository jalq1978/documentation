# New releases 🔥

Everything new in Voiceflow, all in one place.

# **April 14th, 2020 Release**

## **Canvas Design Experience:** 

We want to empower our users to understand the context and direction of their work as best they can. With this goal in mind, we implemented an improved design process and meaningful block visuals that showcase the contents of your conversations directly on the canvas. This makes it easier to see and manage different branches of conversation from a bird's eye view.  With our latest release, spend less time searching for content and more time scaling your projects. You can also expect plenty of UX improvements, a revamped toolbar and better modal accessibility. All of these changes represent a big step towards a faster, more comprehensive design process in our tool. ***To view a more comprehensive run-down of these changes,** [**view our changlog here**](https://www.notion.so/voiceflow/Voiceflow-Changelog-8bd07e4c1e4f45d8ac119938c5b5b172)**.** 

## Our goals for this release are:

1. **Let your canvas tell the story of your conversation**  - editor content now viewable on the canvas
2. **Increase speed and organization** - simplifying the use of combined blocks with a new merging system, allowing for custom color coding & faster linking
3. **Bake in conversational best practices** - allow you to represent your project as 'turn cards'
4. **Design a system that can be used across all current and future channels** - ensure our system scales across conversational channels beyond Alexa and Google

## Why these changes?

Although our canvas is great for visualizing the flow of your voice experience, it lacks context when it comes to individual blocks. Previously, a block's information was housed in its accompanying editor, which meant a user had to click open each modal in order to access that information. This also limited the use of Voiceflow as a tool for stakeholder feedback. With the absence of contextual cues on the canvas, it was difficult for stakeholders to understand and evaluate projects at a high-level - especially when viewing them at a glance. 



# **February 4th, 2020 Release** 

**Important Functional Changes:**

- **Interaction** block is now the **Choice** block, what was previously the **Choice** block is now **Choice Old** and can be accessed from the spotlight (spacebar) search. [Video update](https://www.loom.com/share/f6f2b24626e94de68588487e10121e56)
- The new **Choice** block introduces a more robust intent builder that accommodates slots and dialogue management. [Video Update](https://www.loom.com/share/b0885f6d04884d7787e366db01e49f02)
- **Display** blocks have been temporarily disabled for further maintenance. All existing display blocks will still function as they did previously when uploaded to ADC - however you won't be able to edit them until maintenance is complete.
- Slots are now located on the left bar under the "Variables Tab" - slots can now have colors. [Video Update](https://www.loom.com/share/abb0f816e2a445a19710904e93a45076)
- Access all your Intents on the left bar under the "Variables Tab", there is now a new Intent Management Modal. [Video Update](https://www.loom.com/share/be5b6401beb64983a137799a19248869)
- Slots are now also classified as variables, anywhere that you can use a variable you can use a slot as well. [Video Update](https://www.loom.com/share/9ec929a27bd74ea4ab395be5b6e03822)
- **Interaction**, **Intent** and **Command** blocks no longer provide the option to map slots to variables for an Intent. Previous mappings will continue working but it is recommended to update your project to directly use the slot instead of the mapped variable. Voiceflow now automatically assigns slots and they can be used anywhere else in the project.

**Global Changes to All Editors**

1. New drag step to re-arrange. [Video Update](https://www.loom.com/share/a01406e4c00d4de0970ab961a2be05c2)
2. New drag step to trash.
3. Updated header section style with a bug fix to input lag when updating the block name.
4. Updated footer sections with 'how it works' popover menu (content being updated on an ongoing basis with new written and video tutorials planned for release).

**Speak Editor**

1. Embedded SSML Editor. [Video Update](https://www.loom.com/share/dadb61ef9d18469f8d384f98a71a254e)
2. Play text to speech.
3. Listening to audio upload. [Video Update](https://www.loom.com/share/954ae54165f34c71b43093fe0febb12b)
4. Randomization of outputs has been moved to the ellipsis button in the footer section of the editor.

**Choice Editor**

[Side by side comparison video (old vs new)](https://www.loom.com/share/e3fc74393e4e49a8bbdc93bd5c214ad7)

1. Ability to name intents from the choice block.
2. New intent builder workflow.
3. New slot builder workflow. [Video Update](https://www.loom.com/share/738564567372482f930490095445a63b)
4. Add slots to utterances using '{'.
5. Color coded slot tags.
6. No Reply Response option has been moved to the ellipsis button in the footer section of the editor.

**Dialogue Management:**

[Full walkthrough video](https://www.loom.com/share/b0885f6d04884d7787e366db01e49f02)

1. Implementing a standardized dialogue management interface that adheres to conversational design best practice.
2. Allow for dynamic conversations that are flexible, multi-layered, and natural.
3. Allow users to build faster, and in a more methodical manner.

**Other Changes:**

**Set Editor**

1. Ability to create variables directly from the variable dropdown.

**IF Editor**

1. Ability to create variables directly from all variable dropdowns.

**Capture Editor**

1. Ability to create variables directly from the 'capture input to' dropdown.

**Random Editor**

1. New popover menu description for 'No duplicates' option.

**Stream Editor**

1. 'Visual' section added to collapsable section with additional options.
2. Custom pause option moved to footer inside the ellipsis button.
3. Removed ability to upload audio hosted on Vocieflow (all existing uploaded audio is still hosted).

**Integrations Editor**

1. UI cleanup.
2. New in-depth content 'how it works' popover.
3. Google Sheets and Zapier editors remain in previous condition.

**Flow Editor**

1. Ability to create or add a flow from the same dropdown.
2. UI cleanup.
3. Variable mapping moved to ellipsis button in section footer.
4. New variable mapping UX.
5. New content in 'What are flows' popover.

**Code Editor**

1. Minor UI bug fixes.
2. Expand to fullscreen now inside the ellipsis menu in the section footer.

**Exit Editor**

1. New content in 'how it works' popover.
2. Minor UI updates.

**Card Editor**

1. New content in 'how it works' popover.
2. UI updates.

**Display Editor (Under maintenance currently)**

1. Separated 'Splash' and 'Advanced' display types.
2. New Splash screen section with the ability to upload images to be shown on Alexa instead of having to upload JSON files.
3. Advanced is where you can access Alexa's authoring tool and upload JSON files.
4. In browser preview for Splash and Advances display types.
5. UI overhaul.
6. Removed secondary screen to configure and edit JSON.

**Permissions Editors**

1. New multi-select dropdown to choose all permission types you'd like to request.
2. New content in 'How it works' popover.

**Account Linking (New Block)**

1. We've made account linking a standalone block.
2. Updated workflow for connecting your app to your third party service.
3. New content in 'How it works' section.
4. More info popovers for Scope and Domain tabs.

**User Info**

1. Updated UI.
2. Ability to create variables from mapping dropdown.
3. New content in 'How it works' section.

**Payment & Cancel Payment**

1. Updated UI where you can see all your products and their product image.
2. Ability to add up-sell message directly from the editor.
3. New collapsable section where we explain the 'requirements of an up-sell message'.
4. Ability to create variables from mapping dropdown.
5. Ability to unlink a product moved to the ellipsis button in the footer section.
6. New content in Cancel payment 'More info' popover.

**Why these changes?**

These new features introduce a slew of UX enhancements and a standardized dialogue management interface that adheres to conventional conversational practices. This serves to support the creation of truly conversational experiences while also streamlining our building process for our creators.

We believe these changes will inspire genuine conversational experiences while allowing users to build conversations in a faster, more methodical manner.

# **December 4th, 2019 Release**

**Real-time collaboration**

1. VF real-time collaboration allows project owners to invite both editor collaborators, and viewers to their project.
2. Editors have full collaborative permissions and can make changes to the project, while viewers can "view" the project but not make changes.
3. Allowing users to see each other's cursors, and edits, in real-time as they happen.

**Why real-time collaboration?**

Real-time Collaboration (RTC) is a foundational feature for VF which marks our commitment towards helping VUI designers not only work better with each other, but with their broader teams. RTC allows multiple people to be working on a single VF canvas at the same time. VF's RTC implementation aims to make the experience of working on a project as collaborative as possible by allowing users to see each other's cursors, and edits, in real-time as they happen.

**New pricing structure**

1. New **Basic Plan** offers unlimited projects, all core features and community support at $0/mo
2. New **Professional Plan** offers real-time collaboration, unlimited backups, up to 3 editors and priority support at $49/mo
3. New **Team Plan** offers up to 10 editors, unlimited viewers, dedicated support + everything available in the Pro plan at $249/mo
4. This updated pricing structure will be grandfathered in, and so existing paid users will remain at their current plan pricing.

**Why update the pricing structure?**

When talking with our users it became clear that individual makers wanted unlimited projects, and professional users wanted collaboration features and dedicated support. So following our user's advice, we've changed our pricing to allow free users to have unlimited projects, and paid users to have support. We've increased the prices to accommodate for the lessor number of Pro users there are relative to general makers.

# **Oct 30th, 2019 Release**

**Canvas Refactor**

After overhauling the previous rendering engine and implementing a more modular code base, the canvas is quicker and more responsive than ever before. This improved functionality will help our team build and seamlessly integrate new features and plugins in the future.

# **April 19th, 2019 Release**

**Collaboration**

1. The Dashboard has been turned into 'boards'. Each board acts as an individual workspace where you can add teammates. All existing projects have been moved to your 'personal' board.
2. Adding collaborators to a board can be done from the dashboard.

**Why collaboration?**

We built this feature due to demand from creators and businesses, along with our beliefs in the future of building voice interfaces. Building natural conversations is a tall task, and requires input from multiple team-members with different domain expertise. This new feature sets the stage for teams to collaboratively build better conversations with technology.

Future feature additions will include: live canvas collaboration, user testing, change-logs, and project handoff.

**Integrations (Google Sheets)**

1. Integrations block has replaced the API block. Custom API's can be accessed from within this block's content menu (right bar).
2. We're launching this feature with two options. Custom API (as previously offered) and Google Sheets. We have more integrations roadmapped and coming soon: Airtable, Sendgrid, Dashbot, Zapier and more. Let us know if you think there's an integration we absolutely need and are missing.
3. Google Sheets Tutorial

Winston, who led this feature, made a great tutorial video on using the new Google Sheets integration. Here it is!

[Google Sheet integration](https://youtu.be/O-XAAFRrA20)

**Why Integrations?**

Context within a conversational interface is critical for moving the conversation in the right direction, and getting a user to their goal intent. Connecting to existing services can supercharge your voice app to better deliver information to the user at the right time.

Let us know what you think of our Google Sheets integration. This will likely be the first of many, and we want your feedback.

# **April 13th, 2019 Release**

**Combine Block Updates**

1. Single blocks now have 'add' buttons located at the bottoms to add additional blocks to a grouping.

https://www.loom.com/share/735e2362640341d28c78fc8ac3189a86

1. All blocks within an grouping have in-ports and icons

https://www.loom.com/share/68a2144655234a25b832bc4b63e19186

1. You can move blocks around without unlinking ports

https://www.loom.com/share/95edc3ad9736405eb82e26b965444b33

1. Renaming got easier

https://www.loom.com/share/2d5b040324344eb8bf9ecd882ec9594e

1. Warning message when you're unable to combine blocks

https://www.loom.com/share/98342a204d934c099f13f0b7e450be9c

1. Dragging blocks in/out is still available

https://www.loom.com/share/bc5629dff0f0460398c13f8e4b017dee

**Why these changes?**

Interactions with Alexa and Google, while all different in content should follow some basic design principles. Most interactions should contain some form of output from Alexa and input from the user- which informs your skills/actions logic on how to proceed during the conversation. Combine blocks in Voiceflow make grouping these interactions easier, we hope to see people take advantage of this subtle but powerful change in how you design conversations on Voiceflow.

From the outside looking in, Voiceflow looks like flowcharting software to many. However, our power users understand that conversations built in Voiceflow often don't follow the lines you create. You can hop around based on intents, jump in and out of flows, and change context with ease. We believe grouping interactions with combine blocks creates a more organized way to do this, ultimately creating better conversations. We're excited to see how our users adapt to this change, and look forward to your feedback on how we can improve.

**Input Updates**

1. We've added icon's to specific drop-downs to distinguish the content you are selecting. This small change is meant to create platform consistency.
2. We've globally changed the colour of variable inputs to purple, while others will remain blue.
3. We've added a 'create variable' button to the bottom of all variable drop-downs. This is done to help you create a variable faster without having to manually navigate to the left bar.

**Other Changes**

1. We changed the colour of the Advanced sections blocks as user feedback indicated it was too similar to other sections.
2. We made the left bar expandable. This is making way for upcoming changes. Stay tuned
3. You may notice many other small changes to Voicieflow, some aesthetic enhancements and some UX tweaks. As always, please let us know what you think and we challenge you to improvise better solutions!
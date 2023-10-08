
# Navigating the Activity Designer



 
When you create or open an Activity the Activity Designer appears. The Activity Designer is the space which you can create and edit your automation tasks from. It contains all the tools necessary to automate even the most complex of processes. 

![Image](https://lh6.googleusercontent.com/8aJ1lPgtLl8M2602EAhlWMz4r6wDEhT66SZxPI4tmZyvude_XP54juZycywc-A386aU_hLV_yfRhT9nWpEkcFli-JwHNo8tM-CwiYL6lDQZLL2A4mcQu_sTIxOZD-hkd_ERKs25o) 

The screen shown in the above image is the Activity Designer of a brand new activity so it has no actions placed down; we'll cover actions later on.
Let's take a tour of the Activity Designer.

#### Action Panel

The left hand panel contains everything relating to the actions that you can use to automate a process.

![Image](https://lh6.googleusercontent.com/qCWG5aE-PX1DT3ofwRxrK_tQh9b-FIkepz18rjf05mtWjuQ5nPhOzJgwG6oe6e_FjRd_32KAjO2ctSeFqg202UJqLKlo2jVcXkLZWJaBcd5EMzcOQnJrcqexbwkxsT3tLXlAHwMi) 

On the far-left hand side you have a list of all of the actions available to use with your Bot and then directly to the right of that you have the action palette which is where you drag and place the actions you wish to use.
The actions run in the order that they are arranged from top to bottom. Once you place an action you can move it around by dragging it.
For example, the below shows an Activity that will first perform a mouse click at a certain position and then it will type "Hello world!"

![Image](https://lh5.googleusercontent.com/NVhvZFBE95RTncz9YDDugwng_U_-W6EUGHWHISrTLwZ04ExomiC0El584mszjRyrnGa2Dlw7HrzQGK9uNqlA4YuwtaLYqP8Fc9CFUijO22PcMMTniXb0S4-9v34QSYjsHFl4ZGy-) 


#### Bot Screen and Interaction

Moving further across to the right we can see the Bot's screen. This is a live view of what the Bot is currently doing but you can also interact directly with the Bot from this view without using any actions.

![Image](https://lh6.googleusercontent.com/AAO1BJrk8gf3p8tQpODfDO-G9a-fTxDn6bxceKMRHaIqygTVfAcDuMrNC8-emeLO8xckJvfRJWAq4plH2JxHXieP_fLdc0_dSqYtMSRnTp8jmf6o-vy3IRTNwH9UZm_wuOkRPaWA) 

You can control whether it is just a live view you are seeing of the Bot or whether you wish to be able to interact with it directly by toggling between the two view modes in the bar across the top of the Activity Designer

![Image](https://lh3.googleusercontent.com/wjH3RH8WkwCk3BoQLsT35AqdR9HOfeviearqho60Dmy_iMs2idpQcsSh8Hrl4XCUUglIW4IybTKH1UnNV1G4HM_A3HLYpnTv-3P9A_FnO5B8oN_-bEhc5TL3fLE6fbWjZidECMMa) 

Live view means the Bot is displaying it's screen but you cannot interact directly with it.
 
![Image](https://lh5.googleusercontent.com/MjsoIUtJnRy999M4KMWZbuSvfURW-0KfXKOA1hG9tXAMHo3kligLGr9Ba8t2qRNE2uDAxiM9RgEjEFqfq5p_Y299TdS4S0Ru4Hn1URWS-oTOczp7v8k3d3GGltyZby1vFAQs5Ib1) 

Interactive view means you are getting screen updates and you are able to interact directly with the Bot.
When you are in Live view there are extra capabilities which you can take advantage of.
If you hover over the Bot's screen when in live view you'll notice a menu icon in the top right hand corner as shown in the image below.
![activity designer 7-1](https://docs.toca.io/hs-fs/hubfs/activity%20designer%207-1.png?width=512&name=activity%20designer%207-1.png) 

Clicking on this menu allows you to perform a new set of complex interactions with the Bot without having to use any actions.

![Image](https://lh6.googleusercontent.com/8i7h2bfXH9T14MfrM4nef5h-JTp0BSG7h1RNeXImr3iy9zlzKdAhPLbsQoLfFOkfHUMD2RJ6aF-Ys0-XJnM5C9X6iPSznxbH3T_UmPTcvHvIdpJF6rWCI2kLXjg7wMZuwPXxqXs_) 

This menu allows you to:


- Upload a file from your local machine onto the Bot's desktop


- Download a file from the Bot onto your local machine


- Copy data from your machine onto the Bot's clipboard


- Get data currently in the Bot's clipboard onto your local clipboard

These are all very useful when you're in the process of starting an activity and you are in the scripting and testing stage.

#### Activity Console

At the bottom of the Activity Designer; underneath the Bot screen you have the Console and Watch List. The console is a real-time log of every action that the Bot has run/is running and the Watch List allows you to view Variables and their values as an activity is running, more on this later.

![Image](https://lh4.googleusercontent.com/GAgr2ELBpz3sXs53PEKRQT-qZBFaJfeLCyI26EsT9rMpaC8mnbJ38rIjBsOrI4mq1Ar5iROxGv8-Zj_WqGfvj6YInTTX5pmNZ1Uj9Ge8ujIFPq7LSfyKt6WSMoeniiSef_3bEINf) 

When you run your activity you can see items added to the console in real time and it will show you that each action ran, when they ran and whether they were successful or not.
You can get more information about how each action ran by expanding the action's entry in the console.

![Image](https://lh3.googleusercontent.com/afa4z1ty6L-UiU9jCFKBxxATW9KEeNKU6Rt0yGQ8ddNJJBLyestIS6HhKPAr1ESgCUHARAp6RyhJL456oUoFOJaKY1c_Oqma3mEGWd0shft5EmbkGcM_6CXr2RulqapPKxLyEhJl) 

This expanded view of the console for each action shows what results an action has returned. If an action has errored then the console will also include the reason for it failing.
The console is very useful for troubleshooting if something isn't working as you expected.

#### Notes

Occasionally your activity will be performing something so complex that it requires some form of documentation to make sense of it. Good documentation is an essential part of constructing a comprehensive automation project. This is especially important if you are handing a project over to someone who may not necessarily understand the business process that is being automated.
We recognise this and have note taking built into the Activity Designer. To add a note to your activity, simply click the note icon
![activity designer 11](https://docs.toca.io/hs-fs/hubfs/activity%20designer%2011.png?width=602&name=activity%20designer%2011.png) 

This will instantly create a new note for you to add to. Once you have added text to it the note is saved automatically and you can view it by hovering over the notes icon.

![Image](https://lh4.googleusercontent.com/5qxua3Q92TMhHbO8yIWRRm0AZZG_nwFwKgr7PKCiXduvd3va_Wlrv7Qw8CVNKNpbekcb_nE_Br2XkaVV017rQTHlSoOGrWlY9GMjAR67-_uXELeujYnbdqfGHYIF4eBWesR0vJDW) 


#### Saving an Activity

When you have made a change or update to an activity, it is important to remember to save your changes. There is the option to save in place which will update the existing Activity, or you can Save As which will let you save your changes as a new Activity.
To update your existing Activity, simply click Save which can be found in the top left hand corner of the Activity Designer.
![activity designer 13](https://docs.toca.io/hs-fs/hubfs/activity%20designer%2013.png?width=602&name=activity%20designer%2013.png) 

When it has successfully Saved it will update the text to the left of the Save button to say "Saved less than a minute ago" and it will disable the Save button until it detects something has changed.

![Image](https://lh3.googleusercontent.com/u-_SgXpQwu3Lk-17l36J0g5LlozI5DDmeripCuk8V7Y7xlBehbzk2bfqLU1H-fP4AhIqB9Kuemucwv7Xd1dUl41LYMXwnnV9znHwSDCt9M0XQvBEOuhqlVYrmD6vKExYKf84cunI) 

To save your changes as a different activity altogether then click the dropdown icon next to the save button.

![activity designer 15](https://docs.toca.io/hs-fs/hubfs/activity%20designer%2015.png?width=602&name=activity%20designer%2015.png) 

This will give you the option to Save As.

![Image](https://lh5.googleusercontent.com/CJq0KCf5I7TS-sIWhTd9QW2nHSkY1ouapmYmQhloAO4HVozbbamQLuiFWG6e2eZZ4hWmmiXSL0rXauWnypfn0xGE24_jv-byI2Lz5IhTNpoH9GnXuMtH21Mtru9i240TMQFpnzin) 

This will then present you with a pop up very similar to the one you saw when you created the original activity.

![Image](https://lh3.googleusercontent.com/1Tf9k4mf5MTsibBkN8PWmBpcaJW74kZ46WFMudW5mv7Qgp623dR9Cg7oEq46eVZ0S_XyCdIo-4Saw9WviYCGGXW59tApNLZtalgyhyrU69HIUM2kFp5nZ_o5EkrG2kn_3CkBtn6R) 

This allows you to specify a new name and description for the Activity you're saving it as.
The Save As functionality is very useful for versioning your Activity, so if you are about to make a large change to your Activity you can do so without overwriting the original one.
 

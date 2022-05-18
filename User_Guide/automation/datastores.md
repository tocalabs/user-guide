
# Creating and managing datastores



 
There are times when automating something that you need to store some values for the next time a Workflow runs; you need some way of persistently storing data. You could use files for this on the Bot where you write some values at the end of a workflow and then read the values again at the start of a workflow but this is not a practical solution. 
To make storing data easy we have Datastores.
Datastores are a storage container which you can throw almost anything into. They can store files, images, variables and they can even securely store passwords.
Let's take a closer look at Datastores and what they can do!

#### Create a Datastore

First, let's create a datastore. Each Automation project can have one or more Datastores inside it. This allows you to keep unrelated variables and data separate from each other and it keeps everything clearly organised.
Open up the project you want to create a Datastore in. At the top of the project page there is a button that says Add Datastore, click this button.

![Datastores 1](https://docs.toca.io/hs-fs/hubfs/Datastores%201.png?width=602&name=Datastores%201.png) 

This will bring up a window asking you to give the Datastore a name and a description, this is so that you can easily identify what the data stored inside the Datastore is for.

![Image](https://lh4.googleusercontent.com/bMzA4QtVIzylIaIwbF8KP_tvW2xHhD9oghsIRw03igm0WlgRaSMyGxJj9LoY_EMN8TQXooJicuAru9wDSQzcK5EHP219NNJYN4v7g1GfOIFp4VWqp76UZrQvnFH9cmf5C686WY0E) 

Once you have given your Datastore an appropriate name and description, click CREATE.

![Datastores 3](https://docs.toca.io/hs-fs/hubfs/Datastores%203.png?width=602&name=Datastores%203.png) 

This will open the Datastore which will present this page to you.

![Image](https://lh4.googleusercontent.com/48a1J5ApS6NgOUae_SKgn2r6KFJqeM8EBqiDyh6ACdqfP-rK9vpl9AoR0tZaBNIiR9V6i9FRDhrm4W1WLStY5SOTWejNOMANRUUwbxU92GAqWeL0ja6fsv6HiTK7gMw1P4c60J3P) 

From here you can manually add data to your datastore by clicking either the Add to Datastore button in the top left corner or you can press the ADD ITEM TO DATASTORE button in the middle.
In the next section we'll explore the ways you can add data to a Datastore.

#### Add data to a Datastore

There are two ways to add data to a Datastore: manually or through an Action in an Activity. You can add the following types of data to a datastore.


- Variables - These can be any type of variable such as text, number, coordinates, image etc.


- Passwords - This will encrypt your password and store it securely, you can use a password in the Paste Password Action.


- Files - You can store files of any extension in a datastore, they can be pulled down from a datastore to a bot using the Download File Action and a Bot can add a file to a Datastore by using the Upload  File Action.


- Identities - An identity allows you to link other accounts (Google, Microsoft etc) with Toca so you can take advantage of Actions such as Outlook Send Mail.

**Adding data manually.** You can manually add items to a datastore by opening the datastore and clicking on the Add to Datastore button.


![Datastores 5](https://docs.toca.io/hs-fs/hubfs/Datastores%205.png?width=602&name=Datastores%205.png) 

When you click this button, it displays a drop down list of what you can add to a Datastore.

![Datastores 6](https://docs.toca.io/hs-fs/hubfs/Datastores%206.png?width=404&name=Datastores%206.png) 

Select what type of item you want to add to your Datastore and click the relevant one. Follow the instructions for the type you want to add so for a file it will ask you to choose one from your local machine and for a variable it will ask what type of variable you want. The image shows a text variable being added.

![Image](https://lh3.googleusercontent.com/ry-F7q0DsSj_vvSpRU9KgV65_pQi8MUt-nwVMstgOYAW1Rpdw1zH1O_CIQZJn3t0WJ7No-yR9tvTz3nDYX4LEF4X85XeHZOneFVaRx7LRX_6GDKw3612jUZCApUsjHgL3LB6r6Mz) 

Click on Add when you are done and the new data will appear in your datastore.

![Image](https://lh4.googleusercontent.com/ObM95ouZlEG5BspPKbvTTeenfuh4MIMQPTWHpNS8_rTTUxd4LGRu6PLvn3Cr28obuymqioa1YQXi7HM6YgpGgiA9GL4gTXXQkW-dV4DL2LLjo7vfC9BAK4PPVdeQGKx0faH08KCV) 

When you click on the item you get a preview of the data it contains in the right-hand panel. 
To remove items from a datastore click the bin icon to the right of the item.

![Datastores 9](https://docs.toca.io/hs-fs/hubfs/Datastores%209.png?width=602&name=Datastores%209.png) 

To edit the item you have added, click the pencil icon.

![Datastores 10](https://docs.toca.io/hs-fs/hubfs/Datastores%2010.png?width=602&name=Datastores%2010.png) 

You have now successfully added an item to your datastore.
 
**Adding data using Actions.** The second way to add data to a Datastore is to do so by using Actions in an Activity. To add a variable or file to a Datastore from an Activity you can use the Set Datastore Variable Action which can be found in the Variable category of Actions.


![Datastores 11](https://docs.toca.io/hs-fs/hubfs/Datastores%2011.png?width=478&name=Datastores%2011.png) 

This Action allows you to write directly to a Datastore within the same project as the activity. 

![Image](https://lh5.googleusercontent.com/Cda-IcR4hKI6tyLrDy9hqraZddT7TiSglVs4yDfemvP6EVjwWFozQVRIv2cvZ5zFaX8hEqTBp7YEBnpb3w4WCwC4F0Sbz-Olb3S3vphvtb-rs7y_gH50fK4Hc9J6oaa10T7ho3p6) 

Select the Datastore you want to write to using the Datastore dropdown.

![Datastores 13](https://docs.toca.io/hs-fs/hubfs/Datastores%2013.png?width=301&name=Datastores%2013.png) 

Set the variable name you want to give the item, the variable type and the value.

![Image](https://lh6.googleusercontent.com/eOeF8oaO4xU14ylpGxJiqQfrOVhq-lguysZrgq7OFFfut7fRBziS_sAGGYp71iShDrUSBM5klkttF6pXjbPgZCK8Ac8dVaCTOwoAPbqhEK5h_bslcIHeZC1VBouzcUqfv2QA1GeY) 

Now when this Action runs it will add a variable to the datastore; if a variable with that name already exists then it will overwrite it with the new value.

#### Use data from a Datastore

Now that there is data in a Datastore, how do you use this data in an Activity? Much like using results from Actions and variables, we select a Datachip.
Open the Action you want to use your datastore data in and on the input which will use the datastore item press the Datachip button.

![Datastores 15](https://docs.toca.io/hs-fs/hubfs/Datastores%2015.png?width=325&name=Datastores%2015.png) 

This will drop the Action you are currently editing down to half height and expose the Action panel.

![Image](https://lh5.googleusercontent.com/7lO5oJGodVoiIMAMyemVO43FGz2BBQpR_ga9xTchVNeRHy5llxOfDBukvvG1ARciuU3MP2vWHDRtK_k9bfJhpyjukzrin-RfFo-w-6yrqWi4wVEFnhSx49wtv2qZR0_d61S_S_-H) 

Now select the Datastores tab.

![Datastores 17](https://docs.toca.io/hs-fs/hubfs/Datastores%2017.png?width=406&name=Datastores%2017.png) 

This will then show you a drop down list of all Datastores you have in the current project and it will also allow you to see all the variables you have in the selected datastore.

![Image](https://lh4.googleusercontent.com/9zaoKU1vBM_tMzo1DmJd7ACLn1CwW7t7FIQclL2969BRv0DFewCcH50YKpRTOKIH2EOGAmsrbbnxNp4c1e6chO8E2bxCyeT2pw8PWc2tkFNRN2m8VHAk5kC3hYVQaNwuzlwUowV8) 

Select the Datastore you want to use from the drop-down and then select the variable you want to use. 

![Image](https://lh6.googleusercontent.com/1tukVz5yhce6qt_keZPSjHIWIcWMmzjT2h1BV22isEULv67s7cZvoblqEp0m4MC-pj5J2xBYl7tvQ8GYnQNmpg9nnhvAQg1j2YkNFkFlgv8BXQRZ7wial9OWMXi5VRNR7BX_apJ7) 

You have now successfully used a Datastore variable in an Activity!
You'll notice that Datastore Datachips appear in blue and activity results and variables appear in green, this makes it easy to identify the origin of a Datachip at a single glance. They also have a slightly different icon on each Datachip and a Datastore icon alongside it to let you know where it has come from.

#### Edit a Datastore

Once you have created a Datastore, you may need to change its name and description if its purpose changes. To edit these properties of a Datastore open the project that contains the Datastore and scroll down the page until you find it. You cannot edit the Datastore from the quick access section at the top of a project.
 

![Image](https://lh4.googleusercontent.com/R3ENCov8fLetLZN9baAbL7wyHJKIpx5FJ8nmDTsf9BoKTPd4G8RV7rXMcR_Ke2Sg-I5eJ0PUSLgWmrsIXfd8w-V8vM7zA1VDfL2505EKcA_0kFAIlDTCMX029usXkMgmQxeZLxwb) 

Once you have found the Datastore, hover over it to reveal the Datastores menu.

![Datastores 21](https://docs.toca.io/hs-fs/hubfs/Datastores%2021.png?width=283&name=Datastores%2021.png) 

Click on the pencil icon to edit the name and description of the datastore.

![Image](https://lh4.googleusercontent.com/rSvjbYBe6AHfIlf3hCnRJMLlv_Z-qiG5zcUv2WBUUwH_IfAbjwMW8v7tSoqSQtb2tA0go7eEyiOp0WQrGqIEkvoxR6wzAM3j1u9b6ZrBKGsyVX2yk9xctipYnjokEL9NdhBmq9vd) 

Change the details as you need and then click UPDATE.

#### Remove a Datastore

To remove a Datastore, navigate to the project which contains the Datastore you want to remove and scroll down until you find the Datastore. You cannot remove a Datastore from the quick access section of the project page.

![Image](https://lh4.googleusercontent.com/R3ENCov8fLetLZN9baAbL7wyHJKIpx5FJ8nmDTsf9BoKTPd4G8RV7rXMcR_Ke2Sg-I5eJ0PUSLgWmrsIXfd8w-V8vM7zA1VDfL2505EKcA_0kFAIlDTCMX029usXkMgmQxeZLxwb) 

Hover over the Datastore to reveal the menu.

![Datastores 24](https://docs.toca.io/hs-fs/hubfs/Datastores%2024.png?width=283&name=Datastores%2024.png) 

Click the bin icon to permanently remove the Datastore. A popup will appear asking you to confirm your Actions as removing a Datastore is an irreversible process.

![Image](https://lh4.googleusercontent.com/cnHz3VOB8F_ZkHRR9TyKLUfeIOnOkO6TLP_v5FSQWcxRxl9UlfxVYTgSnjvgqqxApbC5eHSpF4wmBnEk-Out_b-IkFVfGBp9-ZvJwQwglzKfOrGqOBt-nwWIEeOVEaUZfdHFOjnt) 

Click YES to remove it and click NO to cancel.
 

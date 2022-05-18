
# Implementing Decisions and Parallel Execution



 
Some business processes have decision points in them which dictate which branch of a process to proceed down. Other processes require two or more activities to happen at once. The Workflow Designer includes the exclusive and parallel nodes to cover these requirements.

#### Execute Activities in Parallel

When a process requires you to execute two or more processes at the same time, the parallel node comes into play. It is worth noting that a Bot can only execute one activity at a time so the parallel node only really makes sense if you have two or more Bots assigned to your user. 
To use the parallel node identify the activities you wish to run at the same time and make sure each one has a different Bot assigned to it so they are actually capable of running in parallel.
Once you have done this, we can start building our parallel workflow. Create a Workflow and wait at the Workflow Designer screen.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.3.jpg?width=602&name=screenshot.3.jpg) 

As before, add a Start node and an End node to mark where our Workflow will begin and finish.

![screenshot.9](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.9.jpg?width=602&name=screenshot.9.jpg) 

Now, place a parallel node down after the start node and connect your start node to the parallel node.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/decisions%20and%20parallel/screenshot.3.jpg?width=602&name=screenshot.3.jpg) 

Now add in your activities to run in parallel after the parallel node and connect them both to the parallel node, *not* to each other.


![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/decisions%20and%20parallel/screenshot.4.jpg?width=602&name=screenshot.4.jpg) 

Place a parallel node after the activities and connect each activity to the new parallel node.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/decisions%20and%20parallel/screenshot.5.jpg?width=602&name=screenshot.5.jpg) 

Finally, connect the last parallel node to the End node.

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/decisions%20and%20parallel/screenshot.6.jpg?width=602&name=screenshot.6.jpg) 

Now this Workflow is ready to run. When it is run it will begin running both activities on their respective bots at the same time. When the last activity to finish between the parallel nodes has finished, only then will it move on and End the workflow.
Some things to note with parallel nodes in a Workflow:


- You must place both an opening and closing parallel, this is so the Workflow knows when to resume executing activities in series rather than parallel.


- Execution of the workflow will wait at the closing parallel node until all activities between the parallel nodes have been completed.


- If all activities between the parallel nodes are registered to run on the same bot then it will actually run the activities in series but there is no guaranteed order in which the activities will run.


#### Inputs, Outputs and Context

Before getting onto decision points at the Workflow level, we are going to revisit Activities as there is an important feature of activities to learn about which will help moving forward.
When a workflow is running, you may sometimes wish to use a variable from a previous activity inside the current activity. Equally, you may wish to use a variable from an activity to make a decision in a workflow. Let's take a look at Inputs and Outputs in Activities.
When you open the Activity Designer for an activity, you'll notice a tab on the action panel called "*Input &amp; Output*". 


![Decisions and Parallel Execution 7](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%207.png?width=602&name=Decisions%20and%20Parallel%20Execution%207.png) 

Click on this and you'll see a container for inputs and a container for outputs.

![Image](https://lh6.googleusercontent.com/UXe9kHlWQgzYf2Oc3qwqobWdDqMvjNvhLj1EK78uFiwdRGLUg8ZbEW_P6Zsu2SeSv4x64sf5QygcvUnuSBJs6yd0vp3s-bKCX-jfB8vUW45CCtvAdoMvFpsWwr5b2EGzGepeRWm4) 

**Inputs.** By adding inputs to an activity, you are telling the activity to expect to be started with some variables. Inputs can come from manually starting an activity and defining them, they can come from a previous activity in a Workflow or they can come from a Listener (more on those later).

**Outputs.** By adding outputs to an activity, you are saying that this current activity will return these variables when it is finished. These outputs can be used as inputs for the next activity in a Workflow or they can be used to make decisions in a Workflow.

Let's create a workflow that utilises both inputs and outputs. First, create an activity that will output some values.

![Image](https://lh5.googleusercontent.com/Ap5qHu1qMxT-_jtRlOMY8KGwxGnd4bLKNHuQ6ZMeN3NKfYejoSS1pslukF5qGPzo5BL9hzfvVcJSVh3wmIMOYtdZgSJNVho59rXv4rImtp2VRP_wRVvueRseWModVJgUlUIPamzW) 

The above screenshot shows an activity that creates a variable called counter and sets it's value to 0.
To make the activity output counter go to the Input &amp; Output tab and click ADD OUTPUT

![Decisions and Parallel Execution 10](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2010.png?width=413&name=Decisions%20and%20Parallel%20Execution%2010.png) 

You can select either an action result as an output or a variable, this example will use a variable rather than action result.

![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.1.jpg?width=602&name=screenshot.1.jpg) 

When you click the Add Output button it will slide out to the side and show all your variables you have as well as all the actions you have placed on the action palette. This is so that you can either select a variable or an action result.
Select the variable or result you wish to use as your output.

![screenshot.2](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.2.jpg?width=391&name=screenshot.2.jpg) 

Once you have selected the output(s) you want your activity to return you can save the activity and move onto the activity that will take the output(s) as input(s).
In your activity that accepts the inputs, go to the Input &amp; Output tab in the action panel and click Add Variable in the Input section.

![Decisions and Parallel Execution 13](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2013.png?width=380&name=Decisions%20and%20Parallel%20Execution%2013.png) 

This will trigger a drop-down list where you must select the type of input that the activity is to expect (e.g. number, text, coordinates, etc.). In the previous activity we are outputting a number, so the input for this activity will be a number too.

![Image](https://lh3.googleusercontent.com/MXpdf8rFXP4avK-qXCokoFc488dG_U3C8KvhY9y5qMycXW6VtCT5aA4bNJBEmxnh2v78e_cVdh1eXwnSgojfE_zksxBzzUv4ebZP2Dajok9u_fZOZJjgXYW8aJXvEo2P4WlJ1u73) 

Once you select the type of input you will be shown a name and a value field, the name is the name to give the input. If this input maps to a previous activities output then the names must match. For example, if your previous activity outputs a variable called *counter* then the input must be called *counter*. The value is the default value you can set to fall back on if an input with the given name is not available.



![Image](https://lh6.googleusercontent.com/V7S-lKxzoWOVp_N1MKnq81wvMklTv7XfRU2mMwR9B3MWImO6nrtD86H9Tl6bWPsM_5RsFsLgnVSbohvpGG0B5H9-vrONFJq6EYhckC-kCc2TBRjGoilgOXZ5iS6GMHnq3VeqqVqX) 

In the above screenshot, we have told the activity to expect an input called counter which has no default value so the input *must* be provided.

To use the input in the activity, we select it as if we were selecting an action result datachip or a variable datachip. Place down the action you wish to use the input in.

![Image](https://lh4.googleusercontent.com/M0kEToo6CDVfLtbH4xicjboTDEHpxUcZKnj8YFoBNezdevkcYx-HC27gavQaxMV1cI26XN_CXrQHyjLSWnquPr2oQhxQK6CsD3Irgy-YAGfRMhLiNBCu-GSPAMG4eX-OnyvK9vfD) 

The above shows an Equation action as we want to add 1 to the counter input. 
Press the datachip button.

![Decisions and Parallel Execution 17](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2017.png?width=369&name=Decisions%20and%20Parallel%20Execution%2017.png) 

Click on the Input &amp; Output tab at the top of the action panel.

![Decisions and Parallel Execution 18](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2018.png?width=332&name=Decisions%20and%20Parallel%20Execution%2018.png) 

This will show you all your inputs and now you can pick your input as you would a regular action result or variable.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.3.jpg?width=246&name=screenshot.3.jpg) 

In the below screenshot we are adding 1 to the counter input using the equation action.

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.4.jpg?width=280&name=screenshot.4.jpg) 

We can now test whether this will work by starting this current activity with inputs so we can test it before putting the workflow together.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.5.jpg?width=469&name=screenshot.5.jpg) 

As shown in the screenshot above, the Start Activity button has a little drop-down next to it. Press this button and select the option to *Start with Inputs.*


![Decisions and Parallel Execution 22](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2022.png?width=423&name=Decisions%20and%20Parallel%20Execution%2022.png) 

This will trigger a pop up to appear which lists the inputs you have defined and will give you the opportunity to set a value for the inputs before it runs the activity.

![Image](https://lh6.googleusercontent.com/poEdZNtfu4Nld6wzCusZ4mh0HBMciVgV3Yx18-CQ9Io8qYrusnxBZpW2w90UGpu_43w56dQnOaRUGPiU-H_AUdFdl3LniDCAoUMFYvuFxE3KnDe4G3tMQZvhYXpaC_Cg4tUcR1-J) 

Add the value for your input and press START ACTIVITY to run it. Check everything in the console is correct and now you can put the two activities together so that this activity with the inputs uses the output of the first activity.

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/inputs,%20outputs%20etc/screenshot.6.jpg?width=602&name=screenshot.6.jpg) 

Place down a start node followed by your activity that returns an output, connect that activity to the one expecting an input and then finally connect an end node. It should look similar to the screenshot above.
Your workflow is now ready to run and will transfer the outputs of the first activity and use them as the inputs to the second activity.
This is a useful pattern if your process relies on values being passed around throughout the workflow.
All outputs are always transferred to all following activities in a workflow so you are not just limited to using an activity\'s outputs in the activity that immediately follows. 
 

#### Add Decision Points

Now you have learned about inputs and outputs to activities, we can apply that knowledge to creating decision points in a Workflow. 
To add a decision point to a workflow you must have an activity that returns at least one output. Refer to the Inputs, Outputs and Context section to find out how to do this.
To make a decision in a workflow, you use the Exclusive node. The exclusive node allows you to connect to many activities or nodes and each connector can have a condition on. If a condition is met then the workflow will continue down that particular connector.
To use an exclusive node, start by placing the activity which outputs the variable you're going to use in the condition. 

![Image](https://lh3.googleusercontent.com/kZfAGlZPQFRkm-9YwVtkiujxc28Hrc5axbUjlagoQ53pLxsK1B1GZu73O0fL7aygvJ5CrZ4lWk7KfMlonRmy8wFgIUxa3ffDyqvV51mQOm5XKMm-p51Mfr3lrlydQ1ZtqGVmgy3h) 

In the above instance, there is an activity that will return true if it should get FTSE data 
and false if it should get NASDAQ data.

![Image](https://lh5.googleusercontent.com/StIJTZSExEQgmQEpCfgAz69TPmibYhNjAvyzFWn89mJKl-bMYH45QiPxAb9xiNYp20ZeWHGOEYA1gzux6eeGzuA-UNSGxeRd0yhkaqxsA7RXCDHGt-7k1QGnIr20Q91Ql9IIQGN5) 

Connect an exclusive node to your workflow.

![Image](https://lh3.googleusercontent.com/iYFKS2bFbORT89qqaHeuhR66gcu8i9No7G-EeVs1O6PUrxBJaTAFdZ8LVqJ19DG2tYT1ruNyRjvWOZMUmeUbFjxRXsvRHahP327chiEqQAuIB-j3UxAy9OvH2BgrNuGJ2RHgTs76) 

Follow the exclusive by the two or more different paths that could happen and connect everything up.
At the moment we have placed an exclusive in our Workflow but we haven't added any decision logic so let's do that.
Select the Exclusive node.

![Image](https://lh3.googleusercontent.com/rl8ddaDr4cfn3LoKnu0MiZ_KKX2YAinxxJZomhK4X7Uz6PlaleJ7o1a_pTGHNGZwhuYrmpNwlARzNP8i9F9ENOq1O81q3GVkGcwJDtgE3b7209WO5UzxELUdpMsCM31Adpywkim9) 

When you select an exclusive node it will show the properties panel on the right-hand side and it will have as many inputs as there are connectors leaving the exclusive. Here it shows two inputs for the exclusive as the exclusive connects to two activities: Get NASDAQ data and Get FTSE data.
As you click in each input field it highlights the connector that it corresponds to.

![Image](https://lh4.googleusercontent.com/XUeso0ioJI6a7bz7Uuvjz2Yr7iXvYs7a4AxWNPeTxx4eyqRPwdsHuqrGLUiVOW88opBBA5tmh4IlguIW3UZlTa-RnDuc49HLoAkcrSq0ulkPgtoUpYj4z_ORWXvwXgVMNr7rzxi1) 

Here we can see the top input field relates to the connector going to Get NASDAQ data and below it shows the second input field relates to the connector going to Get FTSE data.

![Image](https://lh6.googleusercontent.com/o5eCXiYXLI6-yZufXWu4VCNqH18MC6DMMeoj0LxhVAcmkO9FIBD4AwaMfm1NrnxJ5izdHy1p0QmzeoDCkXHCxZ7x_GSHNX0evtivmBOzG87fS_e1RVTIBrz8dORYYtS9ASutXJXf) 

To use an output from an activity that has come before an exclusive node, we can use the datachip button on each input.

![Decisions and Parallel Execution 31](https://docs.toca.io/hs-fs/hubfs/Decisions%20and%20Parallel%20Execution%2031.png?width=308&name=Decisions%20and%20Parallel%20Execution%2031.png) 

Click on this and then click on the activity that the output you want to use comes from.

![Image](https://lh6.googleusercontent.com/eAs8hbUXJTe-1XCszVaiPcHWAyiz49aPVYANXiH01Ea6p_zBGvKUQJ_mawRtqjGR_5ZjYKNVkXQgQFwlZH1eRSgbEKI-xUCja9JUNKL0gnlQI87R6vGqwVxi7Qthl7zXptv6ij_P) 

When you click on the activity it produces a container that shows all the outputs that activity produces. Here we are just interested in the output called *ftse.*

Add your conditions to each branch of the exclusive node and you should be left with something similar to what is shown in the below screenshot.

![Image](https://lh5.googleusercontent.com/tmwoBwsOOj9Mz8R7iqKR2Tol90U_LQCtxsHUaX6TjarqXuyIMq_yVEeLQz5DLrSgCQs1mTS0csCako0f093YwtC-5Uijopo9PI2TefCoYS8DMub6pBnLTDZeQm33Bxxei5fJRwfg) 

From this screenshot, we can see that the top connector has the condition *ftse == false* and the bottom connector of the exclusive has the condition *ftse == true.* 


We have just successfully added a decision point to a Workflow!
There are some additional things to note when it comes to exclusive nodes in a Workflow:


- The else keyword - If there is a connector that should be followed when none of the other conditions are met then you can simply just write the word else in the exclusive input. This is the equivalent of saying IF none of the conditions are met THEN do this.





- The activityFailed output - Every activity has an output called activityFailed which you can use in exclusives. If you have configured an activity to continue on failure in a Workflow then you can use this status output to decide what connectors to go down in a workflow. This is very useful for adding error handling steps to a workflow if an activity has failed.




#### Adding Loops

Exclusives are not limited to making one-off decisions; if configured correctly you can create loops with them as well.
The below screenshot shows a simple workflow that creates a variable called *counter* in the first activity then adds 1 to the counter variable in the next activity. The workflow then ends.


![Image](https://lh5.googleusercontent.com/YZAqv1pMQECnLy9AuJ7fvOaa7qiQPp6ei90esWp7yJN8j4V3ql3INFHgtp_NljzjvvkxuQ509u1WbR0UPXp86GX9IYrxHaCq0bhoyp49TtpA-xtupTE4qnK7WUll6JsYTQXT_L0g) 

What if you want this workflow to loop until the *counter* has a value of 10 and then finish?


![Image](https://lh6.googleusercontent.com/dDJlLoHH-6GTID46uHlw_4qRW9xIDBEYPF7rwSSc6nbjRAE6cjo1vwFmdILu1d5CujSzV8f2_il1gkjWnwinb9BPjatmuWZYaABpyCsKMYmBJwEDd8-b87VihJRiZp2DxpLchYz0) 

We just simply place an exclusive after the *Add 1 to counter* activity that has two conditions:



- If counter is equal to 10 then we proceed to the stop node



- If counter is less than 10 then we loop back to the Add 1 to counter activity



Assuming the value of *counter* starts at 0 then this will loop 9 times as the value of *counter* will then be 10 and it will finish the workflow.


The loop is a powerful Workflow pattern as it allows you to move loops from your activities to your workflow, meaning you can build more concise activities and do all the orchestration from your Workflow.
 

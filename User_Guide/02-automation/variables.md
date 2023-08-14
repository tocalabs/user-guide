
# Creating and understanding Variables



 
Actions return results which are unchangeable representations of a result at a point in time. What if you want to update a result?
Sometimes in an activity you'll want to store a value for later use and update this value throughout an activity. You may create a list and then wish to add items to the list later on in the Activity. This is where Variables come in. A variable is simply a container for a value which you can give a name to so you can reference the value easily. A variable can be overwritten and modified, unlike an action result.
 
It is **important** to note going forward that the Datachip for an action result will be green and will look as such:


![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.1.jpg?width=402&name=screenshot.1.jpg) 

Whereas the Datachip for a variable will be pink and will look as such:

![screenshot.2](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.2.jpg?width=405&name=screenshot.2.jpg) 

You can create a variable in two different ways. 
**Action Result to Variable.** Firstly, you can create a variable from an Action result. To do this, edit the action which has the result you want to make a variable from.


![Variables 1](https://docs.toca.io/hs-fs/hubfs/Variables%201.png?width=316&name=Variables%201.png) 

Each action has a Variables section at the bottom of it. If you expand this section it will show you the results which that action returns and from here you can create variables.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.3.jpg?width=288&name=screenshot.3.jpg) 

To create a variable, click one of the + in the bottom right corner; next to the output which you want to create a variable from. A pop up will appear asking you to choose a name for your new variable

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.4.jpg?width=295&name=screenshot.4.jpg) 

Then give your variable a name; you use the name to reference the variable when you use it in the future.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.5.jpg?width=301&name=screenshot.5.jpg) 

Then click 'Set Variable' and save your Action.
Your variable will now appear in the Variable palette in the Action panel.

![Variables 6](https://docs.toca.io/hs-fs/hubfs/Variables%206.png?width=414&name=Variables%206.png) 

Click on Variables as highlighted in the screenshot above to show the Variable palette.

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.6.jpg?width=407&name=screenshot.6.jpg) 

This will show you all the variables you have created in this Activity. 
 
**Set a Variable.** The second way of creating a variable is to use an Action that returns a variable rather than a result. There is only one action that does this and it is called Set Variable.


![Image](https://lh5.googleusercontent.com/59FJEmNtBvKgU5Db5_rJjUaEj87mpszBZrt7qQ4cZ7thM_tas5K9IhYgwOH-i5xDkjxlDz8vMxobON2inKia7SGiCp3A4fUUDZ1A5ygjZ66z2jD1u-FIT0KZOy8OBLylZNQLzrT6) 

The screenshot above shows a Set Variable action which creates a new variable with the name of *new_variable* to the text "Hello World!".

As you would expect, the Set Variable action automatically creates a variable from the action output and this can be seen by expanding the variable dropdown at the bottom of the action menu (shown below).

![screenshot.12](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.12.jpg?width=324&name=screenshot.12.jpg) 

If you visit the Variable palette now you can see the new variable created with the Set Variable action.

![screenshot.7](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.7.jpg?width=408&name=screenshot.7.jpg) 

 
To use a variable it is the same as using an action result but instead of selecting a datachip from an action, you select it from the variable palette. As normal you press the datachip button on the input you are editing.

![Variables 10](https://docs.toca.io/hs-fs/hubfs/Variables%2010.png?width=320&name=Variables%2010.png) 

Instead of clicking on an action, click the VARIABLES option.

![Variables 11](https://docs.toca.io/hs-fs/hubfs/Variables%2011.png?width=276&name=Variables%2011.png) 

This will show you all the variables you can select. 

![screenshot.8](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.8.jpg?width=296&name=screenshot.8.jpg) 

Click on the variable you wish to use.

![screenshot.9](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.9.jpg?width=298&name=screenshot.9.jpg) 

You have now selected a variable instead of an Action result.
Another way of using a variable is to focus the input field and type *$*. This will start suggesting variables to you and as you type it will narrow down the options to match what you type. You can then select the variable you want without leaving the action.


![screenshot.10](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.10.png?width=316&name=screenshot.10.png) 

Below the input field you will notice a checkbox titled "Update variable?". Ticking this box will update the variable you used as the input with the result of the action you have used the variable in.
In the example shown in the screenshots this will update the *new_variable* to go from "Hello World!" to "HELLO WORLD!".


![screenshot.11](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/screenshot.11.jpg?width=315&name=screenshot.11.jpg) 

 

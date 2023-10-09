
# Nested Actions explained



 
Some actions expect to have other actions "nested" underneath them, for example a Repeat action expects one or more actions nested underneath it and these actions represent the actions which will run each iteration of the Repeat action.
The screenshot below shows a Mouse Click action followed by a Keyboard Input action that will repeat 5 times and then the Delay action will run.

![Nesting actions 1](https://docs.toca.io/hs-fs/hubfs/Nesting%20actions%201.png?width=397&name=Nesting%20actions%201.png) 

The actions highlighted in red are the nested actions of the Repeat action, you can tell this as they are indented slightly to the right.
Actions that expect nested actions can be split into 3 different groups.


- Looping actions - Any action that loops will perform it's nested actions each loop (For Each, Repeat, Image Grid etc.).


- Conditional actions - An action that makes a decision will perform the nested actions if the condition is true but move on if not true (If Then, While).


- Structural - An action which uses nesting as a means to structure your activity into sub sections (Group).

To nest an action underneath another action, drag it underneath and slightly to the right of the parent action.
If you try running an action that was expecting actions to be nested underneath it but doesn't have any, then the action will fail.
 


# Nodes



 
 
To return to our example, let's introduce a 'click' event onto the workspace and subsequently add a 'trigger event listener' action to the right. Drag them both into the workspace from the left hand side.

![screenshot.17](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.17.jpg?width=535&name=screenshot.17.jpg) 

 
You will notice that once the 'click' event has been dragged onto the workspace, the icon is greyed out and you cannot drag another one across. This is because you cannot have more than one of each event per component i.e. it makes no sense to have more than one click event on a button because it can only be clicked once at any given time.

![screenshot.28](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.28.jpg?width=602&name=screenshot.28.jpg) 

 
Click on the 'click' event to select it. Then, from the highlighted arrow, drag towards the action to connect the two nodes.

![screenshot.18](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.18.jpg?width=602&name=screenshot.18.jpg) 

 
It is also noteworthy that whilst an event can link to many actions, actions **cannot** link back to an event. This will become clearer in subsequent articles when we explore how you can have multiple actions connected to a single event.


![screenshot.29](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.29.jpg?width=602&name=screenshot.29.jpg) 

 
Once the nodes have been connected, click the arrow to highlight it. This will bring up two fields on the right hand side; the one we are interesting in is labelled 'listener name'

![screenshot.19](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.19.jpg?width=602&name=screenshot.19.jpg) 

 
As you will remember from earlier, the event listener we are trying to call had a long randomised string as its default name. We renamed this event listener simply to 'Toggle', and so this is what we will input into the 'listener name' field.

![screenshot.20](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.20.jpg?width=602&name=screenshot.20.jpg) 

 
Click the save icon to save your work. Clicking elsewhere on the page (i.e. above the event viewer) before doing this can cause the event viewer window to collapse and your changes to be lost. 

![screenshot.21](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.21.jpg?width=602&name=screenshot.21.jpg) 

 
If we now look inside the explorer tab, we can see that the button component now has the event viewer icon next to it. Clicking this icon will open up the event viewer for this component.

![screenshot.24](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.24.jpg?width=602&name=screenshot.24.jpg) 

 
Finally, let's preview our app and see that it appears relatively empty except for our button component. 

![screenshot.22](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.22.jpg?width=602&name=screenshot.22.jpg) 

 
But, as per the in-page logic we defined, clicking this button triggers the event listener for the transition and reveals the card component. Clicking the button again hides it and so on and so forth.

![screenshot.23](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.23.jpg?width=602&name=screenshot.23.jpg) 

 
This concludes the first section of the example. Although simple, you should now be familiar with the core functionality of IPL including how to call event listeners. The proceeding articles around IPL will segue into a further example with more complicated use cases.
 

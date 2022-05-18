
# The Event Viewer (IPL cont.)



 
As aforementioned, the event viewer is our 2-dimensional grid workspace within IPL. Aesthetically, it is not dissimilar from the workflow designer and it also shares the same drag and drop functionality. Because it is true that each individual component can have its own events, it is also true that each component has its own event viewer.
 
If you click the button in the design view, you will notice a toolbar appears above it.

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.4.jpg?width=602&name=screenshot.4.jpg) 

 
The icon highlighted below is what we are interested in. Clicking this icon will bring up the event viewer from the bottom of the page. 

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.5.jpg?width=602&name=screenshot.5.jpg) 








Let\'s take a quick tour of the event viewer. Highlighted below is our workspace grid, where we drag and arrange the events and actions.

![screenshot.26](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.26.jpg?width=602&name=screenshot.26.jpg) 

 
Next we have 'component events'. As the name suggests, an event represents a singular point in time when a component is triggered and whatever is after it will run. The available events for the button component are as follows:


- Click - The event and subsequent actions are triggered when the button is clicked.


- Component mounted - The event and subsequent actions are triggered when the component is rendered on the page.


- Component unmounted - The event and subsequent actions are triggered when the component stops being rendered on the page.

 
The available events vary based on the component and what it does/ what the person who created it programmed it to do in the TDK.  Other possible events include:


- Change - The event and subsequent actions are triggered when the value in a text field, for example, changes.


- On Play - The event and subsequent actions are triggered when the video inside the Youtube component starts playing.


![screenshot.14](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.14.jpg?width=278&name=screenshot.14.jpg) 

 
Next, under the dropdown 'web' we have app actions. App actions have a wide variety of uses and, similar to the workflow designer, can be placed in series with the outputs of one being fed into the next and so on and so forth. App actions represent an ever growing pool of functionality within IPL due to the fact that they are created within the TDK. 

![screenshot.15](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.15.jpg?width=406&name=screenshot.15.jpg) 

 
Under the section labelled 'workflow', we have all the listeners that exist in the linked project. This gives us the ability to trigger workflows in the back-end through a wide variety of app related scarios. If you would like to read more about listeners, click [**Here**](https://docs.toca.io/knowledge/listeners-and-triggers)



![screenshot.27](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.27.jpg?width=345&name=screenshot.27.jpg) 

 
And finally there is a text box which allows you to search for any event, app action or workflow by name.

![screenshot.31](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.31.jpg?width=543&name=screenshot.31.jpg) 


#### Advanced view.

 
Most of the time we will only be using the event viewer in the 'editor' view, however there is also an 'advanced' view. To switch between these views, click on the tabs in the top left of the event viewer.

![screenshot.25](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.25.jpg?width=378&name=screenshot.25.jpg) 

 
The advanced view shows the event model as a YAML file. This can be useful for debugging or easily allowing you to copy and paste events or actions. Anything added into the advanced view has to be valid YAML and should only really be used by power users or developers.

![advanced view](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/advanced%20view.png?width=397&name=advanced%20view.png) 

 

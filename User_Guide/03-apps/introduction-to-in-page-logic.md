
# Introduction to In-Page Logic



 
In-Page Logic is a way for events and actions to be used within Toca Apps. This is done through events attached to components that the components can trigger; the user can then attach app actions to these events to perform different actions. For the majority of the following articles, In-Page Logic will be abbreviated to IPL.

This series of articles will primarily focus on how to use IPL and explaining the terminology surrounding it. If you are familiar with these concepts and more interested in IPL in relation to the TDK e.g creating app actions, then click [**Here**](https://docs.toca.io/knowledge/creating-app-actions-ipl-tdk)




First, let's create a page in an app.
 

![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.1.jpg?width=418&name=screenshot.1.jpg) 

 
This will take you to the App designer where we can begin to explore the functionality of IPL.

![screenshot.46](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.46.jpg?width=602&name=screenshot.46.jpg) 

 
Drag a Flex Layout onto the canvas and then, inside that layout, insert a 'button' component. The button, when clicked, will eventually trigger the actions we set it to. As such, the button component is where most of our IPL will be defined in this example.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.3.jpg?width=688&name=screenshot.3.jpg) 

 
Next, let's introduce a transition layout within the aforementioned flex layout. This has a variety of transition effects that can be chosen in the properties panel but, for now, we will choose the transition effect 'collapse' with a 'collapsed height' of 0.

![screenshot.9](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.9.jpg?width=670&name=screenshot.9.jpg) 

 

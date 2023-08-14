
# In-Page Store (IPL cont.)




###  

The In-page store allows us to store values in-browser and use them in apps. Traditionally in Toca we would use a datastore in the backend to manage all of our data and then feed it into the app through an automation project. In this sense, data stores should be seen as a more permanent place to store data due to the fact that clearing your browser cache, for example, will empty the in-page store.
 
Let's continue with our example. Introduce a flex layout onto the canvas and inside that a text component. Use the screenshot below for reference as to how this should look within the explorer.

![screenshot.32](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.32.jpg?width=602&name=screenshot.32.jpg) 

 
Next, return to the event viewer for the button component so that we can begin to manipulate the text component we just introduced.

![screenshot.33](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.33.jpg?width=602&name=screenshot.33.jpg) 

 
Drag three app actions onto the workspace in the same sequence as below. The actions are as follows:


- Get In-Page Value


- If Block


- Set In-Page Value.


![screenshot.34](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.34.jpg?width=524&name=screenshot.34.jpg) 

 
Drag a connector from the *'Click'* event to the *'Get in page value'* node. As you can see from the screenshot below, we are beginning to create a multi-line IPL thread which originates from a single event.



![screenshot.35](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.35.jpg?width=602&name=screenshot.35.jpg) 

 
When we click the connector between these nodes we can see some fields appear on the right hand side. These are our inputs for the *'Get in page value'* action. For the field 'Key', we will put: *'MyValue'* and for 'Fallback Value' we will choose: *'Hello World!'*. For the duration of this example we will only be setting one item to the in-page store and so we will only need to reference one key: *'MyValue'.*





![screenshot.36](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.36.jpg?width=602&name=screenshot.36.jpg) 

 
Next, drag another connector between *'Get in page value'* and *'If Block'.* If you highlight the *'Get in page value'* action then you will see that under the heading 'outputs', there is a datachip labelled '**value'**. This is simply because that app action is outputting that value; in this case that value is: *'Hello World!'.*






![screenshot.37](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.37.jpg?width=602&name=screenshot.37.jpg) 

 
By highlighting the connector which leads to *'If Block',* we can once again specify the inputs. The first step in doing this is to drag the grey '**value**' datachip into the field labelled 'statement'.



![screenshot.38](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.38.jpg?width=602&name=screenshot.38.jpg) 

 
Now that the 'value' datachip has been dragged across, we need to write a statement around it. This should read: *'****Value****' === Hello World!* 




Make sure that the datachip is wrapped in apostrophes as shown in the screenshot below.
The true value will be: **Goodbye World!**

The false value will be: **Hello World!**


![screenshot.39](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.39.jpg?width=602&name=screenshot.39.jpg) 

 
Link the *'if block'* and *'set in page value'* actions together with a connector. Then, drag the grey datachip '**value**' into the field labelled 'value', (this is the output from the *'if block'* action). For the field labelled 'key', type **MyValue**.






![screenshot.40](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.40.jpg?width=602&name=screenshot.40.jpg) 

 
Click the save icon to save your work.

![screenshot.41](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.41.jpg?width=395&name=screenshot.41.jpg) 

 
Finally, let's return to our text component. In the properties panel, click the option which says *'{X} variable'.*


![screenshot.42](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.42.jpg?width=602&name=screenshot.42.jpg) 

 
Once you have clicked *'{X} variable',* a menu should appear where you can navigate to the tab labelled 'In Page Value'. For the field 'key' choose the key we have been using for the duration of the example: **MyValue**.


For this example to render properly you must change the update rate. It's default will be -1 (live updates disabled), but it must be changed to any positive number e.g 1 (second).

![screenshot.43](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.43.jpg?width=602&name=screenshot.43.jpg) 

 
With some minor changes to the styling of our text, our app should look something like this:

![screenshot.44](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.44.jpg?width=602&name=screenshot.44.jpg) 

 
And if we press our button the card will appear as per our earlier example, but the text will now change to *'Goodbye World!'.*


![screenshot.45](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.45.jpg?width=602&name=screenshot.45.jpg) 

 
Let's recap what we have done in this example. The *'get in page value'* action, is looking for an item in the in-page store with the key: **MyValue**; if it cannot find one it will use the fallback value *'Hello World!'.* Whatever it finds it will output as the **'value'** datachip. The *'if block'* action makes the statement that the **'value'** datachip = *'Hello World!'.* If this action deems that statement to be true, it will itself output the value *'Goodbye World!'*. Similarly, if this action deems the statement to be false it will output the value *'Hello World'.* The key: **MyValue,** in the in-page store will always correspond to one of these two options which is what allows us to alternate between them. The action *'set in page value'* then uses that value as an input and updates the in-page store key: **MyValue,** to whichever of the two options it has received. We then set the text component to use **'MyValue'**, from the in page store. The result is as such: the clicking of the button transforms the text from *'Hello World!'* to *'Goodbye World!'* and vice versa depending on what key value is found in the in-page store when the button is clicked.















 
As a final addendum, it may occasionally be useful for debugging or general understanding to look at the in-page store; especially if you are using it to store a lot of data. Accessing the in-page store also allows you to manually delete items etc.
This can be achieved in Chrome browser by right clicking on the app page and clicking 'inspect'.

![screenshot.53](https://docs.toca.io/hs-fs/hubfs/screenshot.53.jpg?width=547&name=screenshot.53.jpg) 

 
This will open [**DevTools**](https://developer.chrome.com/docs/devtools/). From here you should navigate to the tab labelled 'Application'.



![screenshot.54](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.54.jpg?width=602&name=screenshot.54.jpg) 

 
Then, under the heading 'storage', navigate from 'indexDB' &gt; 'inPageDB' &gt; 'InPageStore' using the dropdown menu.

![screenshot.55](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.55.jpg?width=602&name=screenshot.55.jpg) 

 
This is the in-page store. As you can see, there is one item: the key is **MyValue** and the value is *Hello World!* 



![screenshot.51](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.51.jpg?width=374&name=screenshot.51.jpg) 

 
And once the button is clicked, **MyValue** is updated in the in-page store as per the in-page logic we have defined. You may need to click 'refresh' to see this change.


![screenshot.52](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/IPL/screenshot.52.jpg?width=404&name=screenshot.52.jpg) 

 

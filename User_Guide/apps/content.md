
# Utilising App Content




###  

 
When placing down content it is important to remember that it **must** be placed inside a layout component. 

Content can be added by manually typing the text or data that you want to be displayed. To do this place down a content component such as a Text component.
 

![Image](https://lh3.googleusercontent.com/-P7qm1XkMbkhoochnf-c4qBzdWaPFw-aviyMxKJeIa7EzWYT5I0-1s3F5xpxVlW4ca393_Q2n-yTO0bDWCsGFw67xnQwwWF2hfy_x1MUmqK5e9asrzLYGht8LdQNsn4-YfOEFhqH) 

Once you have added some text, have a play with the text properties until your text appears exactly as you would like it to.

![Image](https://lh5.googleusercontent.com/uCB8E0L-olbnLgO5shULTBSUVpWhRqFuAy3dc4oq6UcgMKMh9ZKqBVvv68_rAWwJPjuilZXAwNb5AWYUSpha-KDaSW4CPAT0eC-2zy6S5m4IjUsFVZHXE3315tugbM6u6tuwVhF1) 

At the top of the properties panel is a section called Text Properties and it is here that we can control the size, style, font, position and colour of the text.
Type something into the text box that currently says *A line of text in a paragraph.* 


![Content 3](https://docs.toca.io/hs-fs/hubfs/Content%203.png?width=338&name=Content%203.png) 

Once you have added some text have a play with the text properties until your text appears exactly as you would like it to.

![Content 4](https://docs.toca.io/hs-fs/hubfs/Content%204.png?width=339&name=Content%204.png) 

This is great if you are making a static App that never changes. But what if you want to display data that can update once the App is published? Fortunately, we can do this by linking content to a Datastore!

#### Displaying Content from Datastores

You can actually directly display data that you have inside your datastore from a content component. First make sure that the data you want to display is in a Datastore and that you have linked your Datastore with your App.
 

![Image](https://lh3.googleusercontent.com/H9IqIuUGZjq3Sbec9Om4Q8J0rzVR4ReSkVlBUW-h-4Q292R87OXko1BKxvj0sG1Jgg4M5HQaj090p2PbshAzNS01tlI2GrYzKZcDuMmpFeAIhTETJoqGt38jxkhg3wG6a0942QDm) 

Here we have a variable in a datastore called *variable_one* which has the value of "Hello there!".

Now, back to the App, if you place down a text component and have a look at the text properties, you'll notice a datachip button.

![Content 6](https://docs.toca.io/hs-fs/hubfs/Content%206.png?width=343&name=Content%206.png) 

To insert data from the datastore simply click the datachip button and this will show a menu which allows you to specify where to get the data from.

![Image](https://lh3.googleusercontent.com/fB6HnEItHtbNLRyRq6t53-DsFcAvsujMKOZEYEiIY1n-SAfpfEOEfAfcxxegZJ8-XAEo2c2m7kDRcmujM0uOv_E1jTT5zgRENW3FsZbSL8hF9Ii9RsHkd3QnhzL79oo-L0xNH0cb) 

You either choose a Datastore or from a workflow output (form result) but we're only interested in the data in the Datastore at the moment.
Select the Datastore that contains the data from the dropdown.

![Content 8](https://docs.toca.io/hs-fs/hubfs/Content%208.png?width=315&name=Content%208.png) 

Then select the variable from the datastore you want by clicking in the Variable box.

![Image](https://lh3.googleusercontent.com/DDgvWErJsREjuPUydAxEmPN5aC8ilFpcnozV0T51IGpBn3XLXq42YQsUpEx-QlkdO0fmevgvDDnYu_hwRhQk1nK2-DJZzvM5wm3A2DYRAqLLnr4zRBrxgdthyxPDHbCnnrBxYirL) 

This will show you what variables you have in that Datastore which you can choose to display. Here it shows a variable called users which is actually the Users table for this app and a variable called *variable_one*.


![Image](https://lh5.googleusercontent.com/WNnQ-iOSXpm-t7_bSlb5sfuHc4Z20dTyfBW2wFUwFIOAf8-2C-aaYO6vGLOL5lk_qpuFIdwTqQHR9nnorwOhqxFhqgTRGRYGQVUVY1SAW65p7PN2fAuyZMCCyUQFJWQSxNqlBKE1) 

The next property is the Update Rate which tells the App how often to check the Datastore to see if the value of the variable has updated and display the new value if it has updated. Click INSERT when you are finished selecting the source of your data.

![Image](https://lh4.googleusercontent.com/4Vr_RQjhFPMn36t8sOwc0T9Cr-ocKXUpbUI4BBdDyb39SIX7owrvj5hTloLTOlI02LNDsX_PZOZ2EK2rWZeIIrdvHaEz-OrMhlKQpAFJeMNmpI0HSJ0zxXdsYGekjBpbK618hzY6) 

Your variable will be inserted and you can add text either side of the variable as well if needs be. Any text style you apply will be applied to the variable.
Displaying data from a datastore lets you dynamically change what your App displays without having to republish it or make any changes to the App itself. You just need to change the values in the datastore, see the Datastore section of the Automation Projects chapter to learn more about this.
 

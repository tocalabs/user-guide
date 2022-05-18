
# Dynamic Pages



 
Dynamic pages allow you to have a single page that is supplied with different data depending on a URL-part that you supply.
For example you may have a dynamic page called \'articles\'. The url for this page is actually: [app url]/articles/123456 where 123456 is the ID of some data in a datastore. The page can then retrieve the data for that specific item.
To begin, set up a table in a datastore containing the data you want to display. In this example our table contains data about fruit which could potentially be used for some sort of marketplace. The table should have columns for all the bits of data you want to display. One column should contain a unique ID. This could be a number, and generated UUID or a human-readable string, but it must be unique.

![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.1.jpg?width=602&height=210&name=screenshot.1.jpg) 

Create an app with the datastore as a dependency (or add the datastore as a dependency of an existing app).

![screenshot.2](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.2.jpg?width=565&height=440&name=screenshot.2.jpg) 

Next, add a page which will become our dynamic page. Adding a page will automatically take you to the App designer screen so you will need to back out to the menu of the App before you can make the page dynamic.
Open the page settings popup for the new page and click the checkbox: Dynamic page?

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.3.jpg?width=602&height=319&name=screenshot.3.jpg) 

Select your Table as the datasource after specifying which datastore you want to use.

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.4.jpg?width=602&height=419&name=screenshot.4.jpg) 

Pick the column in the table with your unique IDs.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.5.jpg?width=602&height=425&name=screenshot.5.jpg) 

You will now notice that the icon of the page has changed to include the variable sign {x}. The URL will also be appended with '/:id'

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.6.jpg?width=586&height=94&name=screenshot.6.jpg) 

For now, let's return to our Home page as this is where we will be linking to the dynamic page from. Dynamic pages work especially well with repeating layouts and so this is what we will use in our example. Click [HERE](https://docs.toca.io/knowledge/layouts) If you would like to read more about repeating layouts. Drag the layout onto the canvas and, in the properties panel, click the {x} under 'datasource' to specify the datastore and the variable (in this case our fruit table).


![screenshot.7](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.7.jpg?width=602&height=214&name=screenshot.7.jpg) 

Click 'Insert' and you will see that the variable has populated the 'datasource' field.

![screenshot.8](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.8.jpg?width=339&height=370&name=screenshot.8.jpg) 

Next, drag a link button into the repeating layout. 

![screenshot.10](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.10.jpg?width=332&height=471&name=screenshot.10.jpg) 

Inside the link button properties, click the 'page' dropdown and choose whatever you have named your dynamic page.

![screenshot.9](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.9.jpg?width=602&height=264&name=screenshot.9.jpg) 

As well as specifying the page, you also need to specify the dynamic page ID within the link button. Click the field labelled: 'dynamic page ID', and navigate along to the 'context' tab where you will see a dropdown labelled 'variable'.

![screenshot.27](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.27.jpg?width=602&height=333&name=screenshot.27.jpg) 

Choose your ID column.

![screenshot.26](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.26.jpg?width=602&height=434&name=screenshot.26.jpg) 

 
If we look at our home page in preview now, we will see that there are 4 link buttons. This is because the table we have used as our datasource within the repeating layout has 4 rows.

![screenshot.11](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.11.jpg?width=602&height=281&name=screenshot.11.jpg) 

At this point you may have noticed that, unhelpfully, all 4 buttons have the same label. To remedy this, return to the properties panel of the link button and click the {x} in the label field. Click on the tab which says 'context', and choose which variable you would like to be shown as the label for the link button. In this case, we will choose 'Type of fruit'.

![screenshot.12](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.12.jpg?width=602&height=303&name=screenshot.12.jpg) 

Click 'insert', and then preview the home page again and it should look as below. As you can see, each button corresponds to a row in the table. This will help us to choose what content we want to see once we have inserted data into our dynamic page.

![screenshot.14](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.14.jpg?width=602&height=270&name=screenshot.14.jpg) 

Now, let\'s return to our dynamic page and drag a card layout onto the canvas.

![screenshot.15](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.15.jpg?width=602&height=215&name=screenshot.15.jpg) 

 
Much like we did previously when we chose the label of the link button from context, we will now do the same with the title and sub header of the card. Click the {x} in the 'Title' field, choose the context tab and then the variable: 'type of fruit'.

![screenshot.16](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.16.jpg?width=602&height=313&name=screenshot.16.jpg) 

As you can see, the title of the card now reads 'Apple', but this will change depending on what link button was pressed. We can see what this looks like later, but for now let\'s input the rest of our values from context. Repeat the same process as the title, but this time in the field labelled 'subheader' choose 'price'.

![screenshot.17](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.17.jpg?width=675&name=screenshot.17.jpg) 

Finally, drag an image component into the highlighted red box at the bottom of the card component.

![screenshot.18](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.18.jpg?width=602&height=224&name=screenshot.18.jpg) 

In the properties panel of the image component, click where it says '{x} pick Datachip'. You may remember that in our original datastore table, we had a column containing image URL's for each fruit*. This is how we will be inserting images into this component.

![screenshot.19](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.19.jpg?width=602&height=180&name=screenshot.19.jpg) 

*This is with the exception of 'Banana'. The image for which, instead of a URL, is Base64 format. Either method of storing an image is acceptable.

![screenshot.26-1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.26-1.jpg?width=602&height=224&name=screenshot.26-1.jpg) 

As we have done when inputting all previous values from context, navigate to the context tab and where it asks for a variable choose: 'Image URL'.

![screenshot.20](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.20.jpg?width=602&height=430&name=screenshot.20.jpg) 

Click 'insert', and the image will render.

![screenshot.21](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.21.jpg?width=602&height=219&name=screenshot.21.jpg) 

As is the case with repeating layouts, only the first row will render in the App designer. However, if we now preview our home page, we should be able to click any of the link buttons and the corresponding data will render.
So if we click the button labelled orange we get:

![screenshot.22](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.22.jpg?width=602&height=381&name=screenshot.22.jpg) 

And if we click banana we get:

![screenshot.23](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/dynamic%20pages/screenshot.23.jpg?width=602&height=435&name=screenshot.23.jpg) 

On this dynamic page we are successfully pulling 3 values from context, one of them being an image.

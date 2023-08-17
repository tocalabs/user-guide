
# Integrating Forms



 
Once set up you can link Listeners to the App but how do you actually integrate Listeners and, by extension Workflows, into your App? This is where Forms make their introduction. Form components and components embedded inside form components let you integrate and interact with your workflows.
It is strongly recommended that you familiarise yourself with the concepts of Listeners in Toca before reading further. Please refer to the [Listener section](https://docs.toca.io/knowledge/listeners-and-triggers) of the Automation Projects documentation for more information.


#### Link a form to a Workflow

The first step to integrating your App with your Automation project is linking a form with your App. 
First place down Form layout onto a page in your App.

![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/screenshot.1.jpg?width=336&name=screenshot.1.jpg) 

Once you have done this, open the Properties menu on the right hand side.

![Image](https://lh4.googleusercontent.com/ufQAkf7T9MlydOeA-eSmNe0tATCtJjpBqPbFPLl-EfKVhXUZs5JVldt1AdpZ4BNMXyD3uW0wy9-mRzi5zVJntU2Dm0Zy8dsgMiLl4674koLYfz3V0AaFhIHnZi3iK1Jn4EMm4jFn) 

There are several new properties that are specific to a Form layout component and they are:


- Form Type - Link to a Listener or Datastore


- Listener Form - Name of listener, success message and failure message.


- Open page on submission - Open a different page of the App when the user submits the form


- Send user info - Use user inputs as the inputs to the linked workflow.

 
We'll first have a look at the Listener form type.

#### Run a Workflow via a Listener

If you require to run a Workflow from an App, then the Form type you want to select on the Form layout is *Listener.*


![Image](https://lh4.googleusercontent.com/fazbPDGc2jKpZtCMeVViW0dhBrYl3ReJ0jAyhjGkbfu5JwFoVqQi9-mAXMeMG3AEHwECV_TV2XW6LGrXo9lFLJtV-PBzzS-UfIdJKzMZ7gI59y1UCec6hBRwc41CfT1qGMrew8r_) 

Focus in the Listener field of the properties to select what Listener the App will link to. If you need to create a new listener then you can do that as well and you can do that by clicking the + New Listener option. 

![Image](https://lh5.googleusercontent.com/0qIy-_fd3JWs0VCxRfWqyHcmmCyaj1rXh9oaGQ0eIAFoZmhsQzL2sQClUxFPOOaNVesGS2WefDt29ZcskRq1EyES_ZarD_8-92NV-Suj-yfR0uZrEa_YHwwPen8v9uXfuUnP2Lt2) 

The next options allow you to notify the user with a message if the form submission was successful or failed. These default to *Form submitted* and *Failed to submit form* but you can customise these to suit the nature of the form being submitted.


The next property allows you to open a new page of your App when the user submits the form. You can learn more about pages in Apps in the next section of this chapter.
We need to add a button so that someone using the App can actually submit the form to the Listener. Locate the Submit Button component from the Form section in the components tab.

![screenshot.2 - Copy](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/screenshot.2%20-%20Copy.jpg?width=325&name=screenshot.2%20-%20Copy.jpg) 

Drag the Submit button inside of the Form layout component you have just placed down.

![Image](https://lh5.googleusercontent.com/Czz85ffNSzq22n08ZgLtuV-JHER8m9NZljS2e4fyi11mCtqSOFUAY1jWTlpVVWe_5rTL-7hfnb-yBOGFwxEaQtMZnukgmLF3xWQbX53inJr57X61jY6KZrTBo7aAmBiSVcdfoekN) 

Open the properties panel when the Submit button is selected.

![Image](https://lh4.googleusercontent.com/xxlDwqdDlPOyLR5O9uEasGKD2B5a0k1s7AA8gCAx0MEeL3pXk9CZefBw5Ehh7LX_dl3IdO0oOfos3I58473W_v9m6XZeIEWP4J_Bfvrv31LweTxnrdd9gjwOBi7plhGD0K3JCDJu) 

You can change the style, colour and text of the button but you don't have to configure anything else as the button knows what to do based on the form layout you placed it in.
Your form is now ready to go and your users can run the linked workflow simply by clicking the Submit button!
 
If your Listener is not expecting inputs then you can ignore this next bit but if your listener (and by extension Workflow) is expecting inputs then read on.
 
When you know the inputs you want the user to provide, the next step is dragging in fields which the user can use to provide the inputs.
Drag the relevant component in from the Form category.


- If the input is text then a Text field is a good choice


- If the input is a number then the Range input is a good choice


- If the input is a boolean then the Checkbox is a good choice


- If the input is a table then the interactive data table is a good choice

These are just examples; there are plenty of other components that can be used to create effective forms.

![screenshot.2](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/screenshot.2.jpg?width=325&name=screenshot.2.jpg) 

Drag the relevant component(s) inside your form layout and move them around inside the form layout until they are in the order you want.
Then configure the inputs, for each input go to the properties and find the property called *Form input.* This is how you map the input to the Listeners inputs.


![Forms 9](https://docs.toca.io/hs-fs/hubfs/Forms%209.png?width=345&name=Forms%209.png) 

Click on the dropdown and select the relevant input.

![Forms 10](https://docs.toca.io/hs-fs/hubfs/Forms%2010.png?width=348&name=Forms%2010.png) 

Once you have done this, save your App. When published your App will look something like this:

![Image](https://lh5.googleusercontent.com/G4LiWIf7PaoTZc0aXp9Eje5L4npx7a_qd8v7NhBZ541lQpVsytMLYI91j_ghQfBTNuo4FrD3oo9G4-Ab7DWsuuUXOTN2JlWO51h6gHW34IQyMva0E-EZ78g1lS8M8SPmcEcPQzhQ) 

And it will allow users to specify the input and then run a workflow with the specified inputs.

#### Send user inputs to a datastore

Sometimes it is not necessary to run a Workflow the instant a user submits some data via inputs and in some cases we actually want to process the user-defined inputs in batches. For this you can submit data as a table in a datastore instead. You can then write some automation to iterate through all these tables and process the data accordingly.
First, place down a Form Layout component and open the properties panel. On the properties panel select the Form Type dropdown and select Datastore.

![Forms 12](https://docs.toca.io/hs-fs/hubfs/Forms%2012.png?width=306&name=Forms%2012.png) 

This will render a new set of options inside the Form Layout properties panel.

![Image](https://lh5.googleusercontent.com/DLwL-aDnTS8foHajXwCQElbNKSXRcxfBCguPMAhqVPGsNK2Mzf7rdiHlRACgbR9Jm3O7RFHzFw4FijCd1aEKAxWZG5w7P1qXtpcpQwngA3taaMBsyXXcBxNI45MqbBWQnl9xx-bs) 

You now have to provide:


- The Datastore the data will be written to.


- The notification message when the data is successfully submitted.


- The notification message if the data is unable to be submitted.


- The prefix to give the variable when it is written to the datastore.


- The name of the fields to write to the datastore

 
Let's go through an example to illustrate how it works.
First, select the datastore you want to write the users inputs to, you can only select Datastores you have already linked with your App.

![Image](https://lh3.googleusercontent.com/QctyY_ZRD0rS6JZtvQfRWsl3PSEG7S6x-3OdCOi7XdNIG2qroEvufECHwmXbTzIsIMFAhpxjr4dvGMY7FcRd3ERXMSSq47ceo75VCgYKCJEuf32ZQ1KzDiEtCKPnuGwYkFo_rFPf) 

Add a custom message for the user when they submit their data.

![Image](https://lh4.googleusercontent.com/F9z7hGG-c9OMjOR8cL9Ls_Kg_sSqwayKIgHeVoKolurBxuPu6YkUwJm4WBhiGmPj5KgV2O1IgMc98CANpqFqIGQSHJAO0kGe3C-IE9U1pqOApdiTsH28NvkNDJdh0vxTcoOIQwT2) 

Set the prefix for the variable names when the data is written to the datastore.

![Image](https://lh4.googleusercontent.com/_CVYEVMFo2eiwdTm9rplpBeDJrRZZ_GYV0XbmPKNJ5HYD0O_iX6pCM7Vm8wyRVbPd-EfweyFoQYhX8IqE9jaEqpOoY8P18Wxu-WJyabWrlNgaEMNOUHASoKYjHG0mN0g0BR9AbYv) 

Then add the names of the fields that the user will enter data to.

![Image](https://lh4.googleusercontent.com/5HjIDNltdL7wHHP17Sk3B7kThBB241FvjITQ-Uf9IGPHN5AVsKDdBndIvSaP7iK-p12unedEHLTCcYoiopzLCdM6ADalnLaKQ2yh3_MjDcjrklC5_i8FlvpcoZXLW7Gm9IYwh_NN) 

Now lets add the input components for these fields to the form layout and connect everything up. We'll need four text inputs for the fields shown in the screenshot above.

![screenshot.2 - Copy (2)](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/screenshot.2%20-%20Copy%20(2).jpg?width=325&name=screenshot.2%20-%20Copy%20(2).jpg) 

When you have dragged a text field into the Form Layout open the properties panel and find the form input field.

![Forms 19](https://docs.toca.io/hs-fs/hubfs/Forms%2019.png?width=339&name=Forms%2019.png) 

This will let you choose which of the inputs defined in the form layer this input field maps to.

![Image](https://lh4.googleusercontent.com/tJ88TxeDSTCnQz6HgwRpyqxhtM-EBfzVtUfxWlb6jC2aTETqImZtVoqcoCJc9AH4KlVaHvn-ghbqctw7_Qf1URfa_0qzBAubJqGrAy5iW3_t2AoUC1AaJfosPC2um8sexwJZxwB2) 

Select the one that this input will map to and then give the input a relevant label so the user of the App knows what the field is for.

![Image](https://lh5.googleusercontent.com/QdYigsWw63oB2bVyeNth_K5Rr_7Av5FkJIIbTUCdRE0T8s1CsbY9TER6MssG5Q33ud6TC0vEMq6Tbl8PSHfR_8PQB7JV6da4mzXk-IDQXSCVr5MGMKQjjhi2JvhXL5cazbNq99I7) 

Repeat for all the inputs and then when this is done the preview will look like this:

![Image](https://lh5.googleusercontent.com/nwK3wOyRPWc0XmFaQic672XAO5gSZd89CT7PYrh6Ww_k2_3YUJ8tPwjqfLC8hv0UIFfakHMnQ39LKKNWtFwXmuut949agylFGWQnibdYrGqiPlg5_1oSIpcw-3B6eTFyqpOVhExE) 

Finally we need to add a button for the user to submit their data. Drag in a Submit Button from the Form components and add it to the bottom of the Form Layout. Give the button a label that makes sense to the user.

![Image](https://lh6.googleusercontent.com/1JYYofNzDLIRxcThj8QO7vBKQIzTDDfNXwb7bcuqruuNPlmbulZSsXkBfXgqXMofNPFpLV84sl5D5DI-7CMQqw-Ao2kLGr-hR_vk5Zp5bhWybi_dyZP5RQUtOSTtmq0ONnTO8Lqt) 

Now lets see what the data looks like in the Datastore when the data in the below screenshot is submitted.

![Image](https://lh6.googleusercontent.com/y8YGmC2uCaVyU0NKfwTrqpDhOPoaAuhOW02QT3430-P3NPiu-yJNRm-9vLgIH27YuRGS9mhLsnnWtyd6tup2pY0cEsPNk_et1MTbipxtNpZM-NihpS4SESl4DY-mdNPfiBto9nA7) 

We can see a new Table variable has been added to the Datastore, the table contains a single row which contains the data just entered in the form.

![Image](https://lh6.googleusercontent.com/GwiNLRKsEV0a8l_6yrXMWfwTVL5AaIURSq9UukFm7Uoa8KtEAe4WpqaINREiTWDCnibvde7t69StYzfahLslVzRjwImm0fb-LPP3P-VSEEF3NMBvWy3JxTysnJ7uf89V73Wd_og3) 

You have successfully submitted data from a form to a datastore!

#### Displaying Workflow Outputs

The workflow that you integrate with your App may return some outputs which you want to display. To do so, add your form layout and link it to a Listener as shown in the *Run a workflow via a Listener* section of this chapter. 

Identify what outputs the workflow could return and drag the corresponding content component into the Form Layout to render the outputs. In the screenshot below you can see that a Text component has been dragged in beneath the Submit button.

![Image](https://lh6.googleusercontent.com/IcQpWx__N73CiEBLdCtnUMPH76dcOQKAhvdDluuSZJhiDuJjshbQZgLT4VdSwlbaN0NvaTt-1wtCANMXf3MJgi8hdASlKg8RxdxkhrYIBh1M5kVjvMEcRm2ZeEHLvC4NiCw-ui5K) 

To render the outputs of the workflow in this component open up the properties panel and click the datachip button.

![Forms 27](https://docs.toca.io/hs-fs/hubfs/Forms%2027.png?width=290&name=Forms%2027.png) 

This will open a datachip menu which allows you to define the source of the datachip. Select the Form Result tab instead of the Datastore tab.

![Forms 28](https://docs.toca.io/hs-fs/hubfs/Forms%2028.png?width=333&name=Forms%2028.png) 

Select the Listener that is linked to the workflow which returns the data you want to display.

![Image](https://lh4.googleusercontent.com/lua_csmfUEcYZLKutscrdJUJqUeKzk4ZNBar30Y7ejOQyNVXKasqDlGRBVlqiQdq6s4RrMg2eJhiM3SwOW5ZdymH51xWxufpmjv8NgeB9hmz_myJwXnK5s1VA6c6e_Bouvfvk0f-) 

Once you have selected the correct listener, it will show you a topological map of the workflow the listener is attached to and all the activities within the workflow which can be expanded to show the outputs of each activity. Select the output that you wish to display.

![Image](https://lh3.googleusercontent.com/mbNCFk-4ZwySApDpb0p9gNHyUedw_P-XgOTYuaOo6C1gwf3cP7KS9pTC-VuVabQ0rHh6hhZvenNvk7aBvcG7lOY4j9zpVC_-MUDeOtdU-kbVTkTdnoil7cMJIE22sp2G9fLInni6) 

Click INSERT and this will add the output as a datachip to your components content; add any additional text around your datachip as required.

![Image](https://lh4.googleusercontent.com/XzJyZuw-YdCtJCD6syZMIt2JSWKKLlQG8d0sDq9ODRbl1y1grMYXRV44LZOU3Ne100hoIVA3VHUmXpquekqnQoA3V0h2w1_w1Ki09EjWAQo19R4i_hB00BmbjeiJ3sNv9jyisFJY) 

Now let's test this by running the workflow from the app and seeing if the output appears. Before anything is run the datachip does not have a value so looks like this:

![Image](https://lh6.googleusercontent.com/T5J_Bq5k-FGigzsGMSoJVXPAryWrenPZ2SfTWRbI_SUe785YnT4AaB9_2G7LyxLDLi6vas87RwAxCtftDRovhWGK6wV4H0aj4QdMsN-6tk4DKeRptUpsgHW1wRS1Es4IXujGwiKr) 

Let's set the starting number to 50 using the range selector and click ADD ONE to start the workflow.

![Image](https://lh5.googleusercontent.com/2rKnlk5LRKB977evowYphprDPlbYgt08-3iHP3SK1PwBFCiyBps2pgonj4ImU_zPcIy8HFScu0c5FuT7ZcAAhDX15HhWt0CIg20BvPnNiC6xX0-of1UglVaY-KllXPSJWyrRZGYw) 

Where the form result was placed you can see it now says "Loading...a6" as it is waiting for the output to become available. Once the output is available it will give us the expected output.

![Image](https://lh3.googleusercontent.com/807tiMDNZtyZlTK9ltssWDReR4F8jgZ1CFRW5MnQXk04VRKIhOmhGSUOuazCv6XamC5sX-A6np3GlEg5OY-5TjvMaPqICclrkTuo1JIscQ6y-yJ40-wqEDLv0zMlO6hfDVqxWpiE) 

 

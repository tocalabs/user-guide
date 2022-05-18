
# Listeners and Triggers explained



 
Listeners and Triggers describe a set of features which allow you to turn your Workflow into a RESTful API (Application Programming Interface) endpoint and make RESTful API requests from the workflow. [[https://en.wikipedia.org/wiki/Representational_state_transfer](https://en.wikipedia.org/wiki/Representational_state_transfer)]


#### Listeners

A listener is something you can set up on the start node of a Workflow and it turns the workflow into an externally callable RESTful API endpoint. This allows you to embed Workflows into your own applications and call workflows from third-party apps. This allows you to seamlessly integrate Toca with any existing or new in-house development.
To create a Listener, create a workflow or open an existing one and select the start node.

![Image](https://lh5.googleusercontent.com/v8vkrSIP0_H20zUY_RRZ5F3z3whJcbE7oUOLvhjeYGV3Kdg4TLuAOs0wPydNctKxolSfUZ-ngXW8f5o4viyjSxBw3AwiJLgyQ-Dr9gFbiki-zamU6g8Zs2m_wfIlQjot4-80EirX) 

The listener panel appears on the right-hand side allowing you to add a new listener or edit existing listeners.
Click on Add Listener and a window will open allowing you to set up and configure your listener.

![Image](https://lh6.googleusercontent.com/tui-Eil_ulNQOX6ij9hnjIrlx4qLP1D_Cky9jNakWuwDFXnitsd1bQbpUE_VIlWHhCy-frKoCgNJWHa7jzPiY-tqtJ-dN24cokt75WJE6kWG_x9AQtz8IHZerk8aNyI5XsWQM7ii) 

You can give the listener a name that will help you identify which workflow the listener corresponds to. You can add a description too but it is optional.
The next property allows you to make the listener public or private. A public listener can be called without any API keys whereas a private listener will only work if you send a valid API key in the request to the listener. To add an API key, click the ADD KEY button.

![Image](https://lh3.googleusercontent.com/XqieAm4vf4LFo3KPJ1Ht2dWLukcxr7AXyQZwnhNL3b4eLpAlil48uzibeC3QXtfN7zUMCl49YEiiSnOxSkPJcfb7Pkb2pdmejyKXCCixGPthw8Cu1V_hbNBgn6rWM-PhDMqRV8AB) 

 
This will automatically generate an API key for you and make it valid for approximately 30 days time. You can modify how long it is valid for by changing the *valid before* date and also you can change the name of the key to something more meaningful (e.g. *Key for Developers*). 


The next section down in the Listener window allows you to specify a payload to expect when the Listener is called. This can map to inputs expected by the activities in your workflow.
As one of the activities in the Workflow has a numeric input called *counter* the Listener has automatically generated that model.


![Image](https://lh5.googleusercontent.com/r80sWb9xjo99D5uLuF9bl-iD2TEVDQ7Dv670egxZOFWPsh1koRLRTQA77UylYWzPIf1-UICvqucPQbNgHFKnkXrW95pm6OdaYOgDfRN5BbgDgx4kX7tN_PqJb2vCDvCR0yQjCCdO) 

You can remove any auto-generated inputs and you can add to them.
Once you have configured the Listener to meet your requirements, you can press SAVE.

![Listeners and Triggers 5](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%205.png?width=602&name=Listeners%20and%20Triggers%205.png) 

When you have created a listener, it will now appear in the Listener panel in the Workflow Designer when you have selected the start node.

![Image](https://lh3.googleusercontent.com/PXdts33G_WbXga3WCc-xgUQosPukd3dwoJxpLjZkX3NCqYXjXfGtL9iZgRXAqFx92FUegNO_23xRYmXDg7EnLGyPdmjnJe-WC-iVB_lQXf2WbJ7PKDRKOw7WhmTsOEiPGx_gXElR) 

To see information about a listener, just expand it by clicking on it in the panel.

![Listeners and Triggers 7](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%207.png?width=313&name=Listeners%20and%20Triggers%207.png) 

This will show information about the listener such as the URL to call, the API keys associated with the listener, and the JSON (JavaScript Object Notation) body the listener is expecting.

![Image](https://lh5.googleusercontent.com/3-znvvWIhjSet3uN_Qvgj_3SHUHpmRI8WmDY5xZiVMjksJgndgIRQLXonXt_sW7tRGqAYjVCKFVbncp7w3dC6h7OV2QUd_6Hfm9pO6WhPk52r0dibI6BBCrBDkUN85esKoRFKAUK) 

Finally, an example cURL request is included so you can test the listener easily.

![Image](https://lh4.googleusercontent.com/xSIZVXy7k185Vj0CsvO-4QhatzHIXyIdoacGouFvfRtVMjfcOxOEA9w64C9g8AQd99b4TQjTq7k_vM1eg0xAk9_uPIBnfmFfVzhcTBjpk9SooaKk6IdacGvm-P4cB3ejiQ32aPYF) 

Your Workflow can now be run by sending a POST request to the URL shown in the Listener panel and with a JSON body as shown.

#### Triggers

The Trigger node in the Workflow Designer allows you to call RESTful API endpoints from the Workflow level rather than using an action in an Activity to do so. Using the Trigger you can call external endpoints or Listeners within the Toca platform. This means you can actually start other workflows from within your current workflow. 
To create a Trigger in your workflow, create or open an existing Workflow and place a Trigger node down in the position you wish it to run in the workflow.

![Image](https://lh5.googleusercontent.com/xuV8J83Z1FLKtwwz8B1OCgQyCtuBO4RshP06ddFR-suD92rpI50YCcY_1HBCAM-1kiHPFI-LKpnUoxN3tzV8h12MowKTwioB20hjkLMPIHd3w445kX34K9igYDcrtr0IMgHwMhyD) 

Once you have placed the Trigger down, connect it up.

![Image](https://lh6.googleusercontent.com/Uv3UNGEf8lmOIKe96uPOLBaBDpNkQrpbJtFNavTXPDGBq9phMtgKFx--XCKx6DWaKieV5SeELfb0JsFAMuoPHKgmcqYSeOalALFvyi-7uYZZFjUXPya711SSkwdjNdlrqs4Kg49n) 

Then to edit the properties of the Trigger node, click on the trigger node and the panel on the right will show the properties.

![Image](https://lh4.googleusercontent.com/bPQZOvJxo5ji5dfrycrQNy6x19h6AQNv6prQjZOyETrpqTQHOxH_q_Vb0CmObbugA1ZCj53xtgyCb5DSkr8XcfUGSIaEt_YNoVbTC86w_CbKPTlm4YWNHuAjPL1wREYapQGOSHAJ) 

As can be seen from the above screenshot, there are two different tabs on the Trigger properties panel. One for Listeners and another for Custom API endpoints.
We'll cover how to configure these properties for both Listeners and Custom endpoints later on.

#### When to use them?

Triggers and Listeners bring a lot of functionality to your workflows but when should you actually use them? 
**Listeners.** Listeners allow you to start a workflow by making an API call instead of using a schedule or manually running your Workflow from the Toca platform. This makes sense if you have a use case similar to:



- Starting a Workflow from another workflow in the Toca platform.


- Embedding Toca into your own internal applications (e.g. adding a Run button to an existing dashboard)


- Allowing third parties to run Workflows on your behalf to integrate your automation with other providers.

**Triggers.** Triggers allow you to call an API from within your workflow, this API could be a Listener you have set up on another Workflow or it could be an API that exists outside of the Toca platform. Use cases for a trigger may include:



- Running another workflow from the current workflow using a Listener.


- Sending some data from your automation to an API that exists outside of the Toca platform.


- Retrieving some data from an external endpoint that is required for your Workflow.

These are just some example use cases for Triggers and Listeners, of course, there are many other uses for them.

#### How to call a Listener

One of the use cases that was described in the section before was that you can use Triggers and Listeners to run other workflows from the currently running workflow. Let\'s explore how to achieve this.
First, let's create a Listener on the Workflow we want to trigger from the other Workflow.

![Listeners and Triggers 13](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%2013.png?width=602&name=Listeners%20and%20Triggers%2013.png) 

Select the start node and look for the Listener panel on the right. Click the ADD LISTENER button as shown above.

![Listeners and Triggers 14](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%2014.png?width=602&name=Listeners%20and%20Triggers%2014.png) 

Fill in the Listener properties as appropriate and then click SAVE on the Listener window.

![Listeners and Triggers 15](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%2015.png?width=602&name=Listeners%20and%20Triggers%2015.png) 

Once you have saved the Listener, copy the API key using the copy button as highlighted by the red square in the screenshot above.
Now create or open an existing workflow where you want to call the Workflow you just added a Listener to.

![Image](https://lh6.googleusercontent.com/tjRgNHV1YwT-bwshC0Oz7EonGmuoJdJLWEg-7QbdTC5UQqHl5AOP3jGw92vZ6lSbMVan0FPDRQLycNUCqb12q9gbRZznIKhRrVe6IhbkE-YsPQ42FSyjQb4VbBXtRmPjyrC3RAkT) 

Now add a Trigger node at the position in this workflow you wish to start the other Workflow from.

![Image](https://lh3.googleusercontent.com/jq7U1hyuZk4uajG_6Fab8MqtnsUKGU5-6sfL_6GWb4ud1JYQ8MFRVUsLjvI3_1qdWFkb_SDc14VDQOtpvWJAzFh2w_qVS-SKScRnK9itc4GDOClDka5Y-vblQew1Lc2hL1JjwIh4) 

Select the Trigger node to show the Trigger properties panel on the right hand side.

![Image](https://lh6.googleusercontent.com/kARePiyYrqu_syPS-vbMHl2DzsfOvq4BO5IgRoDTTRVKoJ69yJZjuig5yJhcvgG8XFhcPsmLMcqiishAZcw2YF2bnjrIaeoNkPVXBSDczocz-8lpZiiGujKFmn8sqMRKkfkSXrRF) 

On the Trigger panel you need to select the Listener tab rather than the Custom tab. Once you have done this, type in the name of the Listener from the first Workflow and paste the API key you copied.

![Image](https://lh6.googleusercontent.com/paDCJKAs4B990bb98wNkleSzHCoH5ZznjGwhE8bzRjNT5ARynsRV4PVqlN88Cl1D5GfaIlHZEIgBsjc1zwKsXI_8jvondAUXiIT3BmNN8NeRdVeUgX0fKTcvFOimobHtD6_05T6j) 

Then once you have done this, click on Generate Model and any inputs that the Listener you setup is expecting will be automatically added to the trigger model.

![Image](https://lh6.googleusercontent.com/oWJ5NZQ_sHzV3qvkb2ZR4y-2hkH85ni73ojo-K6gyGE4nhNldEVw1zhTbcfI90h4ykadl5De4torvy67K3YnQq0vqKPSptzqalLcDj2noZjG4eicEHhsUG367IDLAvE9WC_s7-mT) 

The Listener that was setup for the first workflow expected an input called counter so this Trigger has added a variable called counter to the body which you can use as an output from an activity to populate using the datachip button.
Once you have set the properties of the trigger to the appropriate values, Save the workflow to save your changes.

![Listeners and Triggers 21](https://docs.toca.io/hs-fs/hubfs/Listeners%20and%20Triggers%2021.png?width=241&name=Listeners%20and%20Triggers%2021.png) 

Run the Workflow with the Trigger in and when it gets to the Trigger node, you'll notice your other Workflow with the Listener starts running too!

#### How to call an external API

Now we have successfully called an Listener using a Trigger, what about calling an external endpoint using a trigger?
It is worth noting that currently Triggers only support calling RESTful API's which accept the POST method and it does not yet support adding headers to the request.
 

# Linking Actions to Form an Activity

**Purpose:** This lesson aims to provide insights into how to effectively link multiple actions together, thus creating a cohesive activity within Toca.  
**Prerequisites:** A basic understanding of individual actions within Toca and the concept of thinking functionally about these actions.

## Table of Contents

1. [Understanding Linked Actions](#understanding-linked-actions)
2. [Extending our open browser example](#extending-our-open-browser-example)

## Understanding Linked Actions

In Toca, while single actions represent specific tasks, the power of automation truly shines when multiple actions are linked together to form a comprehensive workflow, or what we call an "activity". Each action in this chain relies on the output of the preceding one, ensuring a seamless flow of data and tasks.

## Extending our open browser example

In the upcoming sections, we will delve deeper into enhancing our 'open browser' function and turn it into something repeatable and valuable by integrating key data principles and introducing new practices to optimally structure your activities and actions. Let's dive in!

### Grouping our actions

As we create more complex sequences of actions it makes sensse to group them together to help strucutre our wider activity.

Using the search bar we can quickly look for the group action:

![group action](img/group_action_select.png)

Once selected we can create a meaningful name and the save:

![naming of group](img/group_name_and_save.png)

Once we have saved our `group` action we will need to drag it above our `open browser` block and once we have we merely need to drag our `open browser` action into our group:

![drag open browser](img/drag_into_group.png)

You should be able to see that our actions are now slightly nested:

![nested](img/nested_action.png)

Now we have a group that will contain our actions around capturing data from the web and ifwe then create more complex actions later on we can always clapse our web data capture to make things easier to view:

![closed group](img/closed_nested.png)

## Data inputs

We will be going into data management in actions in greater details in subsequent sections but we're going to imporve on our 'hard coded' browser open which was heading into `google.com`:

![](img/google_data_in_browser_action.png)

We want to change this so we can add an `argument` as highlighted in our [Functional Design Section](../00-thinking-functionally-designing-activities-with-purpose/thinking-functionaly-designing-activities-with-purpose.md).

To do this we must add an input by selecting and adding an input:

![adding and input](img/creating_an_input_variable_for_our_url.png)

and then clicking the add input button:

![select add input](img/select_add_an_input.png)

You will see from the manu that appears there are a huge amount of options when adding inputs but we're interested in adding a text input:

![select text input](img/setting_a_variable_options.png)

This will bring up the following fields:

* **Name** - Clearly name your input
* **Default** - The default value is what will be used if no other value is provided.

We will add the details `name: url` and `Default: https://www.hl.co.uk/shares/stock-market-summary/ftse-100` as below:

![input data example](img/input%20value%20example.png)

***NOTE*** -> The default value can be overridden when passing a value from a workflow (which we will cover in subsequent sections) or by selecting the `Start Activity` drop down as below:

![start activity drop down](img/start_actviity_drop_down.png)

And selecting `Start with Inputs`:

![](img/start_with_inputs.png)

Once selected the `Start with Inputs` option will bring up a menu with all available inputs available to you as well as being able to add new variables:

![start activity poop up](img/start_activity_pop_up.png)

For this example we will not be changing our variable at start activity and it will not always be the case that you will want to change the input variable value.

## Updating an action to use an input variable

Now we have an inout variable set up we need to utilise that variable in our `open browser` action. We do this by selecting the `edit properties`:

![action edit properties](img/open_browser_edit_properties.png)

We want to use our input variable and the default value it holds rather than manually input it ourselves. To do this we need to select the `variable` icon highlighted below:

![variable select button within open browser action](img/variable_button_open_browser_edit.png)

After clicking the variable you will see the menu expand to show your actions as well as the various tab options, we need to select `INPUT & OUTPUT` which will display our first `datachip` which is our `url` input variable:

![url datachip](img/url_datachip.png)

Now we have selected our new input variable `url`, if we now run our activity we should be able to see the browser hit our url destination:

![run activity using impur Var](img/run_activity_with_input_var.png)


### A quick note on datachips

Datachips are Toca's way of exposing data and as you can see, we had created an `input variable` for our `url` which is now available for use across our `actvity`.

we will be going into more depth on `datachips` in the subsequent sections.

## Interacting with the web page

Before we dive into gathering some data to use, we should ensure that we manage our data correctly by handling the cookies window:

![cookie wihtin the bot window](img/cookie-bot-window.png)

### Interacting with web elements

We want to be able to select an element within the bot window and on the browser to interact with it. To do this we can use the `get web element` action and select the Element 'finder' icon:

![get Element element finder](img/get_web_element.png)

Selecting the cross will allow you to interact with the bot and select an area of the screen:

![selecting web item](img/selecting_web_item.png)

As you see in the screen print we have select the item button on the page and options have now appeared in our get web elemetn window. **NOTE** - you will see as you navigate across the options to select that the toca window will darken to focus on what exactly that web element relates to which helps with laser focusing on that you need to interact with.

Once we have selected the button it will be visible within our web element and we will want to change our `interaction` to click.

![web element click](img/web-element_found_click.png)

## Data Outputs

In the previous section we have created an open browser action and utilised an `input variable` to manage our default `url` as well as giving our activity the option of changing the variable.

We now want to take a look at how we create a data output from an action.





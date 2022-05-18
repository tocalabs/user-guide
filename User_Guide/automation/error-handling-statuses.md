
# Error Handling & Statuses explained




#### Error Handling

When you are automating something it is good to be aware of all the things that could happen which could impede your automation. For example, what if you are trying to automate something on a web page but sometimes you get a pop up asking you to accept cookies? How do you handle a pop up that only occurs some of the time? The following three properties allow you to customise error handling on a per action basis.
**Fail on Error.** All actions have an input called "*Fail on error?*", this input, if ticked, will set the actions status to Failed if an error occurs whilst the action is running. This is useful if something has gone wrong and it is irrecoverable. All actions have this option ticked by default.


**Timeout.** Some actions have a timeout property, examples of these actions are any action in the Vision, OCR or Flow Control categories. The timeout field (set in milliseconds) tells the action how long it can run for before it should stop itself. It is also worth noting that a timeout can be given the value -1 which means the action will ignore the timeout completely.

**Error on Timeout.** The actions which have the Timeout property will also have an Error on Timeout property. This tells the action whether or not to treat a timeout as an error. In some instances it may not be considered erroneous for an action to timeout. An example of this is if an image search action is looking for a pop up that only appears sometimes, we want to click Accept on the pop up if it appears but keep going if it does not appear.


The table below is a handy guide to show you what combinations of the above inputs lead to what outputs when a timeout occurs.

|Error on Timeout|Fail on Error|Description|
|:-- |:-- |:-- |
|N|N|The action is marked as Success as a timeout is not treated as an error.|
|N|Y|The action is marked as Success as a timeout is not treated as an error.|
|Y|N|The action is marked as Continued with Errors as the timeout is considered an error but we have told the action NOT to fail on errors.|
|Y|Y|The action is marked as Failed as a timeout is treated as an error and we have told the action to Fail if any errors occur.|

#### Statuses

There are 3 statuses to be concerned about when looking at actions.

|Status|Description|
|:-- |:-- |
|Success|Everything has worked as expected and no errors occurred|
|Continued With Errors|An error occurred but the action that it occurred on had Fail On Error unchecked, meaning the action errored but the activity will keep running|
|Failed|An irrecoverable error has occurred, this will stop the activity running.|



If an action goes wrong then the console will include the reason for the error to help you troubleshoot any issues.

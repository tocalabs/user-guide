
# Using Datachips



 
Most actions will return one or more results that can be used later on in the Activity. An action\'s results are unchangeable and represent the result the last time the action was run.
To see what results a particular Action can return, find the action you want to get the results from and hover over it.

![Datachips 1](https://docs.toca.io/hs-fs/hubfs/Datachips%201.png?width=404&name=Datachips%201.png) 

You'll notice an Info button appears, highlighted by the red circle in the above screenshot.
If you click this the action card will flip over and on the reverse side of the action you'll see all the results the action returns.

![Image](https://lh5.googleusercontent.com/gF-ib2k7weSu0u38bc1QapbtV4ycCjz2syweJEa643hxeEgwv1cXV3uDUMK9Qxow-YrthdaWzCZiDdIpWFaV_fOzaoVcY1IdTXtE9MX1_2-5yAD0j6unm56I_lOxHIyhWeVTqopr) 

The Rename File action shown here will return 3 results:


- actionId: The Action ID


- fileToRename: The original file path of the file we are renaming


- newFile: The resulting file path of the file after it has been renamed

To use a previous action's results in a new action then this is where the Datachip button comes in. On each input in an action there is a datachip button which allows you to select a previous action result as the input value.
Continuing with the rename file action, what if we wanted to get the size of the renamed file to check the file wasn't modified incorrectly during the renaming step? To complicate matters, what if the new name changes each time we run the Activity? 
We can just use Datachips to solve our problem!

![Image](https://lh6.googleusercontent.com/5JrHwqFiBFp1CbgRRSA-bHknIvgtOPClkEbSkzObjUwF_btV-HYcGgf5GYLkXW-NIvrvH099U6T2dQ0ki7SJMeRV2Bt-1LRjJj9ldW_loSkSlWu9INEMevroKuDuojCb-vaRhMt9) 

These are the input fields of the Get File Information action, which will return the size of the file to us. 
It is asking for a file path to the file we are getting information about.

![Datachips 4](https://docs.toca.io/hs-fs/hubfs/Datachips%204.png?width=376&name=Datachips%204.png) 

On the file path input field, there is this button highlighted by a red box in the above screenshot. This is the datachip button.
If you click on this button then the action you are currently editing will drop to half height, exposing the other actions you have previously placed in your activity.

![Image](https://lh6.googleusercontent.com/gCvgytGd5KhOHYLSmOzQa0vPSFwZa6EKJwC5mN701LOH9Tc_V_SP9u8mNPlJQUt61qZKpQqhSxhj3_pKRW9xwzcJxjRVcAatqECXwXEx_sLVF6IO1XteG1nTXU4alWvlGgY6ZKYM) 

We want to select the newFile result from the Rename File action. To do so we just click the rename file action and this will flip that action card around showing its reverse side along with the results.

![Image](https://lh6.googleusercontent.com/FXn35B11IX79bypHxArygEQ8PgRpMne7cOEATmLLr8HJ-UA7vCpA0p1DkNCdYlja4JlezbwFEZt_9sDtyUEX2HvtOdUpOtPLU_eA6C4KfizE6vmNBewaV-Q-jfAol7ofKTLNgjHN) 

We click on the datachip we want (newFile) and this will bring the action we are currently editing back to full height and should look like this:

![Datachips 7](https://docs.toca.io/hs-fs/hubfs/Datachips%207.png?width=350&name=Datachips%207.png) 

You'll notice that the File Path input field now has the newFile result in.
Sometimes an action will return a result that is incompatible with the field we are currently editing. A mouse click returns the coordinates that it clicked,  if we tried to use the coordinates result from a mouse click action in our file path by accident, what would happen?
Well, fortunately Toca will prevent you from selecting incompatible results.


If I try selecting the coordinates result from a Mouse Click action for my file path I get the following:

![Image](https://lh5.googleusercontent.com/ThgWMcS8hMnWKcXYC2BoEhhStGZuPW4_2k5zqLNCDhn3ciw7MGkEG0Jt5YJUwuBLYPlRvYCtOJUABeBNiupgtSuE9H2PstOU3A359DQ2lXBYr-rkV6Q5FVawCiHdNd4lo10Z0usj) 

You'll notice that the coordinates chip is hashed out and you are actually unable to select it.
This will prevent a lot of mistakes and it will also guide you to let you know what results are compatible with the input field you are editing.


 

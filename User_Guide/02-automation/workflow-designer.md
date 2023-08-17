
# Navigating and Using the Workflow Designer



 
The workflow designer is where you create and design your workflows from. It offers a drag-and-drop interface to create workflows of all complexities easily and quickly.

#### Components of the Workflow Designer

When you create a workflow or click on a workflow from the project page then this opens the Workflow Designer.
Let's take a look at it!
 
In the middle of the workflow designer is your workspace where you drag your components in and organise them.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.5.jpg?width=602&name=screenshot.5.jpg) 

On the left hand side of the workflow designer there are three tabs. These are as follows:
Nodes: Shows you all the events and gateways available for you to use. More on these later.

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.4.jpg?width=602&name=screenshot.4.jpg) 

Activities: Every activity within the project which you can place down in your workflow.

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.6.jpg?width=602&name=screenshot.6.jpg) 

Actions and Integrations: Actions that work within your workflow E.G API caller.

![screenshot.7](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.7.jpg?width=688&name=screenshot.7.jpg) 

Then at the top of the Workflow Designer you have the options to run the workflow, configure the workflow and save it.

![screenshot.8](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.8.jpg?width=602&name=screenshot.8.jpg) 


#### Start and End Nodes

The start and end nodes represent the events in your Workflow. 
**Start.** Every Workflow must start with a Start node and there can only be one of them. 

**End.** An end node represents the end of your workflow, there can be more than one end node as your workflow could take many different paths to reach the end. When an end node is reached in your workflow, nothing else is run.

To add these nodes to your activity, simply drag and drop them from the sidebar into the workspace.

![screenshot.9](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.9.jpg?width=602&name=screenshot.9.jpg) 

You'll notice that once you have placed a start node, the start node on the sidebar is greyed out as you cannot place more than one in your workflow.

#### Adding Activities

At the moment our workflow does nothing; there is a start point and an endpoint but nothing to connect them.
Let's add an activity. Find the activity you want to run after the workflow starts in the Activity tab on the left side of the Workflow Designer.

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.6.jpg?width=602&name=screenshot.6.jpg) 

Once you have found the activity you want, drag it from the panel to your workspace.

![screenshot.18](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.18.jpg?width=602&name=screenshot.18.jpg) 

We have added an activity to the workflow but if we tried to run this it still wouldn't work and that's because we haven't told the workflow what order we want to run the nodes in.
Let's add some connectors to fix this!
Click on the start node and this will highlight the node and show a little context menu underneath the node.

![Image](https://lh6.googleusercontent.com/olgQ5pYEXs7jzFQH3WW-nmp97OYVrNjBTNHh7WCJgNUn-YscRjyYHobT7jthUe4egbWBKVLoNe8-G23uxAEGevN8ym6PRRAAtHq6MH3RVWJ320NVSLbqQicCU7UF3JKgYQvC5Wsy) 

Click on the arrow that appears to the right of the start node and click again on the activity node. Or simply drag the arrow from the start node to the activity node.

![Workflow Designer 10](https://docs.toca.io/hs-fs/hubfs/Workflow%20Designer%2010.png?width=158&name=Workflow%20Designer%2010.png) 

Once you have done this you'll have drawn a connector between the start node and your activity.

![Image](https://lh6.googleusercontent.com/0_tWB8wyivNNZxMLq6b7DpWgPZrxutFaSjuL5TAlQ96Ai-sZZH4Mm8nuBlsra-iiRNmnrBEz05wrV48qN2wXAFnfi0JFmBb-pTR1PWWuM53tRD9aH7yZ5LFw6JLcn7eVzSsysDA0) 

Let's finish the workflow off by doing the same between the activity and the end node.

![Image](https://lh5.googleusercontent.com/Bn3-XybLRUyChi5KFnRmIKGeRu-XnBiG0TReUICByq1ZcR66u5pKcoaBkH3BKdp_2BQIBh0oi5RsgS2kremR8Z4h-W3RQQDeKyVXkc5Ur3Qj_vXW6l2ym5LQgmeTeCylMGKqOFy-) 

Now we can run the workflow because we've told the workflow what order to run the nodes in.

#### Add Labels

Sometimes it is helpful to add a bit of documentation around your workflow as you may have added steps which may be complicated and they need explaining.
For this we can add a label. The label appears in the node panel on the left hand side of the Workflow Designer.

![screenshot.12](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.12.jpg?width=82&name=screenshot.12.jpg) 

Like the start and end nodes, drag it into the workspace to where you want to place the label.

![screenshot.16](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.16.jpg?width=602&name=screenshot.16.jpg) 

Once you have placed the label down, click on it and this will show a text editor for the label where the activities panel was.
Customise your label until it appears as you want it to.

![screenshot.17](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.17.jpg?width=602&name=screenshot.17.jpg) 

Click off the label to unfocus it and reveal the activities panel once again.

![Image](https://lh3.googleusercontent.com/oBKc7S03_5RO3fL1FqzE1K2Rkx_bzzoojGcwWGXNFjarW8gK1ZWCMMC2zINVLYady2IyeyntP2sTq4Wh6GeMScKrnLXMk3VDXe-rs7FAF4rTAmOL_K9tXvBnpNTACuzJjJ5gfYQ9) 


#### Configuring your Workflow

There are some workflow options which can be configured on a per-workflow basis. To discover these options, click on the Configuration button shown below.

![screenshot.13](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/wfs/screenshot.13.jpg?width=602&name=screenshot.13.jpg) 

This will open a menu which shows you what options are available to change.

![Image](https://lh6.googleusercontent.com/_0G5aX0aRW9jT1L1aFSehWUgMk3kyydKKtibs8c9jzNZ3gXyetUkQm584vaNXT3DCz3NGe4CcxCOAJHCSdczgX8PO6dBT5p_QXx4zRQZAt-r--5tHXkQoHp1-1eAdagBDcVZdoQD) 



- Receive email notification on fail/error - This will send an email to the notification email you set up in your profile settings (or your account email if there is no notification email) if this workflow failed when it ran.



- Show labels - Show activity names in the workspace of the Workflow Designer.


Once you have configured the choices you want, click save and these options will only be reflected for this particular workflow.
You can also configure activities in a workflow, if you select an activity you have placed in a workflow and click the cog icon.
 

![Workflow Designer 19](https://docs.toca.io/hs-fs/hubfs/Workflow%20Designer%2019.png?width=590&name=Workflow%20Designer%2019.png) 

This shows a menu which allows you to change which activity is in place and also allows you to configure whether or not to continue the workflow if this activity has failed.

![Image](https://lh3.googleusercontent.com/uFZZBQ-CwFSGISLqfZJTZNdnBhW99aI-x1_VIxcNRCSb7MZTD8NWs_TVwZIt60bANqfjwx7RAfnOxWAElrUT58tVOV_hrLlsb3RlBU9REYDrrL0zzMFCKvKunALdhlm1R871nGuc) 

If you check Continue On Error then the workflow will continue even if the Activity has failed. This comes in very useful when you are adding error handling to your workflow.
 

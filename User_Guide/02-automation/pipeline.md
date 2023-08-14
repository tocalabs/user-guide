
# Introduction to pipelines



When you run an individual activity from the Activity Designer you get a real time report of what is happening from the console. Is there an equivalent when you run a Workflow?
Yes there is: Pipelines.
Pipelines provide a report every time a Workflow is run. The report includes all the details necessary to see when your Workflow ran to completion or if something went wrong. When something has gone wrong, the pipeline report allows you to quickly identify what went wrong so you can add the necessary exception handling next time the Workflow runs.
 
You can navigate to the Pipelines page by clicking on the Pipelines icon in the navigation bar on the left hand side of Toca.

![Pipelines 1](https://docs.toca.io/hs-fs/hubfs/Pipelines%201.png?width=602&height=390&name=Pipelines%201.png) 


#### How is it organised?

Pipeline reports are organised into two different views, a high-level view and a detailed view.
The high-level view lets you know what the statuses of all jobs are, how the jobs were run and how long they took to complete. The detailed view lets you inspect each activity in the workflow and see how each action in the activities ran.
N.B. When a workflow is run this is known as a "Job".

#### High-level view

To see a high-level view of all the jobs that have been run and are running, navigate to the Pipelines page.

![Pipelines 2](https://docs.toca.io/hs-fs/hubfs/Pipelines%202.png?width=450&height=320&name=Pipelines%202.png) 

This will open up the Pipelines page to the high-level view which will look similar to the below image.

![Image](https://lh3.googleusercontent.com/yBeFqUel5iY72_CGkkxq7iE94F0HEz1vVleVasWu27b9Mejrix8XHf9A0giOovLsp9LgYcXfV0U8UJg8EyuFHa0dKuZ4DhQe-ub3e3jTLwSokvS03MuAKyZzAMh1_RRCZS5sR4LB) 

On this page we can see the headline figures at the top of the page letting us know how many jobs are currently running, how many jobs have run to completion and finally how many jobs have failed.

![Image](https://lh4.googleusercontent.com/8TWxVD5264nnuqskEc4nFj0rk5xiAh1D-GEnZbfoVCs2aCiUKu69fPNp3Uw0gWxlHzQl_T8lrumWmSk_ZJGY3WpdHMvT18ElJ4ICKcjQvzbUkI14wcAJ9h6twps8OG5roGPyuyq5) 

Moving down the page we can see the main table of entries. Each job has an icon to the left of it letting you quickly know what state the job is in, the next column along is the name of the workflow, then how the workflow was run (Manually or by Schedule), then the status of the job with the length of time it took to complete.

![Image](https://lh5.googleusercontent.com/h0tgDHIJcit2oOBHkgGOebDfMvEtlJIExKELplqqjPwVG9zLoDvAarwd9Dg35rI1m2A_JMyJvzPPN9RpZG086EEJzSczKWaSd7FldUpIAEPPkGOR5Wu2m5OwTOh1AuZixg2FMOE9) 

This table is paginated so you can navigate through the pages using the arrows at the bottom of the table.

![Image](https://lh3.googleusercontent.com/hm3Ewdiku7nmR1DqiZ0Lv-vk8fu-hsE8F7O_k1VazIkdonyyuRJQWB1aMNw7qKVcWjaWMbXna7vwuiD057qT7uYhkEYU3Mjucjeqfyeo5Ub-WT9J77MWohXy-uooERUPYjRZuVYd) 

At the top of the table there is a filter button.

![Pipelines 7](https://docs.toca.io/hs-fs/hubfs/Pipelines%207.png?width=324&name=Pipelines%207.png) 

Click the filter button to reveal all the ways you can filter the results.

![Image](https://lh6.googleusercontent.com/sVgg-s5tNPqF39THR1dqbqNdusSO7xbBDXDuqV84QeYWZGhKx1Sz93OebhhtcwR_G1lKGR_Rum13lb2yYUHYKbsnjSDtNUljvwgzFT98PRtz5b8pJdJhNBguun4Tn0jzY197jean) 

Using the filter you can search by:


- Job name


- How it was triggered


- The status of the job

These filters make it very quick and easy to find the exact Pipeline report you are after.
 
At the end of each row in the Pipeline table there are three icons.

![Image](https://lh4.googleusercontent.com/ModzrPFEX2qjkRVvUd7-48TEn2SQnXi52qhOyM56ajHYKHVv971Y0NYw9exr__z1sOHg-yr0aF3PxCfaTiNQlxuFBvsEUtwGUJCLJvfrFkxc5CatJl7Qc2Ny7rZTLeZeQXYPf2FY) 



- Clicking on the first one will open the workflow that this report represents.


- The second one will open the project which contains the workflow.


- The third one will remove this pipeline report from the Pipelines page.

 
This is all there is to the high-level view of the Pipelines page.

#### Detailed view

If you want to see more information about the job that ran then click on the job from the high-level view. This will take you to the detailed view for that particular job.
 

![Image](https://lh3.googleusercontent.com/wwrveDNOmnPeRqdqc59_wl4VAwvfT5y3bz00X-A6Ecld8Tc_aeMNj5mqeZXAG5VZZeK2S6u_Jr4NW64DJNRO8sB8qe_-NTZAYwJkAAYQ5afxMDBwfIv9FYPiFNv2AXIq2W__SR_A) 

This view shows you the nodes of the workflow that were run in the panel on the left-hand side.

![Image](https://lh5.googleusercontent.com/NPNXqp6nEucCcSka3Qz1rNNQzGRasYHZDaZp9K_G2KrbfDpahHl_vFyDRN6Pzn62rMkuK2mDcxoKb1dLjWQwD8h0wvMwOlwuv0hDazfa6J-f5ZI9QzRpBMdT4--jFXl9SPFVwQT7) 

This shows you the status of that node, when it ran and how long an activity took to complete. To see more detail about how the node ran, click on the node.

![Image](https://lh6.googleusercontent.com/a56SK6aTE-ovrNt1zG0gm1zTeC0oLJIgtuDC7aa_FMSyOGVVmaajZukReUf3UL6JgZhZmD5mfa0HvNE2d8Jc87baEHEPiq2tjZjK1wUTI1zYV9LsjyxTfw4MM1GAWsoZMGKHEHAs) 

This shows how each action inside the activity ran. It shows what the action was, when it ran, how long it took and the status of the action. If you want to see even more detail such as what each action had as an input and what the action returned then you can click on an individual action.

![Image](https://lh5.googleusercontent.com/hMZMlnhJUgG8q-8x1g23MLTd1w33LyxCzcENLo4vUA0pU0ad3y-qL3ZfnxEjjIC_tA7xsR17x2NlgggbwHtQuWDwoz3reTtonyHuxArzlQLocUggJs8Ko61Pl4lJUd8YDP6BbCXn) 

This lets you see all possible information about each action. You can then navigate between actions by clicking the arrows at the top right of each action window.
![Pipelines 14](https://docs.toca.io/hs-fs/hubfs/Pipelines%2014.png?width=346&name=Pipelines%2014.png) 

This particular view is very useful when you're trying to find out what went wrong if your Workflow failed.

#### Quickly find errors

Whilst it is nice to see all the jobs that have completed successfully, we are often more interested in finding out why something went wrong when a job has failed.
A good rule of thumb to follow with errors is that they will usually come at the end of a job. Unless you have configured your Workflow differently, a job will fail if an Activity fails and an Activity will fail if an action fails. So in a job that has failed, usually the last activity to run will be the one that caused the failure and in the last actions to run will be the ones which caused the Activity to fail.
With this in mind, there is a handy feature which allows you to view the actions in the reverse order that they ran in.
 
Click on the Job that failed to see the details.

![Image](https://lh4.googleusercontent.com/5Y5vt0YOtL0NEdqGuCPMnbQHOu5tSLnA9tk_2X2-RPan86hKvlDQ8_9w5ZXbAy2C37dWiooZWY6BQUWuK4-ylGEsn0ZuoBxE8VNwCch2tWWybZWjruymmwke6rnZ6p6aCq4LWDzx) 

Click on the node that failed and caused the job to fail.

![Image](https://lh4.googleusercontent.com/bx0JAC-oVL2jJe9c47xE4OhK7V6gxu7bAOmiU_c3ftZTtEpxKzaiPQ4TAjz4JVipqzM-76UlhJpZxKGqmvsXOHS5C30HbpSYb2JnKEiJjbxhygnOhj-O8i_6w2RhYjPCop2f00R1) 

We can see that an Image Click action Failed and that caused the workflow to fail. If this was a long activity then it could take us a long time to find that information. For occasions like that, you can reverse the order actions appear in.

![Pipelines 17](https://docs.toca.io/hs-fs/hubfs/Pipelines%2017.png?width=602&name=Pipelines%2017.png) 

Click on the dropdown that shows the order actions appear, by default they appear as oldest first.
If we click the dropdown and select Newest first then the actions appear in reverse.

![Image](https://lh5.googleusercontent.com/MAsFmb75kYKKcHHcWeV608Y6lxh3ixOe1xKyemLVU9U8wXWnoGCQB8yWMEWoN6XjGewgVZPymox4xl1jh5Xq-kdTL1Yeo6AGptcdzeWfJD0A8OnNF-uqpkEPun41mXtZ54Vg2Z1H) 

This makes it very quick to find your failed action even if there are 100's of actions within your Activity.
 

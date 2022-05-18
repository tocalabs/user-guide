
# Scheduling a Workflow



Once you have created your workflow(s) you now need to decide how and when to run them. Sometimes it is only necessary to run a Workflow occasionally and for this, it is often enough to run a Workflow manually by clicking Run Workflow in the Workflow Designer. However, usually, it is the case that a Workflow should be run routinely on a schedule. You can schedule any Workflow in Toca and no matter how complicated the schedule is, it can be accomplished.

#### Create a Schedule

To create a schedule navigate to the project which contains the Workflow you wish to schedule. 
Across the top bar of the project page, there is an Add Schedule button.

![Scheduling a Workflow 1](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%201.png?width=602&name=Scheduling%20a%20Workflow%201.png) 

Click on this button and a popup will appear which shows you the schedule wizard. 

![Image](https://lh5.googleusercontent.com/u_YwhP2q2yw_SsHV-7fGxRe7Z1kvLJQz9FX-MKTgChyjDtLzlcztOqcLs-x5pf1wTlXvgirUYqHm_lcSY5AuDvtg8tJNMv1OarPksbTuRvlUwzHVfvmfdUoLcHGHQpuuamYWSjS0) 

From this window you can select the workflow you want to apply the schedule to, you can also give the schedule a name to help you identify it in the future.
Each schedule has the following properties:


- Start Date and Time


- Interval


- End Date and Time

**Start Date and Time.** This signifies the date and time that the schedule will take effect from.

**Interval.** The regularity with which the schedule will run.

**End Date.** This is the date and time that the schedule will cease to run the Workflow from. If the End date switch is unchecked then the schedule will run forever or until it is deleted.

 
Using these three properties you can create a variety of schedules that should cover any business needs.

#### One-off schedules

To create a schedule that will execute the Workflow once in the future then we can create a one-off schedule. To do so, set the *Start Date and Time* as the date and time you wish the Workflow to be executed, set the *Interval* property to the Does not repeat dropdown option.



![Image](https://lh3.googleusercontent.com/-5yCAe3W05B8jj1m2cDNv7oBfmjQYkuwiuvkOi3oQT4HLJNgpfJ2AgS1JAPBg96gdT8RlS7bfPVjHZQCIavW7dlpxNVfJOqDvEcz3t6eRVCnpAalB43PYff1NX64QV41X79W5JlF) 

The schedule shown above will execute the *Series Workflow* once at 08:15 am on the 17th February 2021.


#### Repeating Schedules

If a Workflow requires a more routine execution schedule then we can apply a repeating element to the schedule.

![Image](https://lh6.googleusercontent.com/wqYn5twSRhcE3HLt-dH9DMDO4xyRznMgJEdE88nYhKg2hvroxQwrUR74cfnI1vXA-P8jdQSObPgOKUSTNbwMbG6D3qwRPWR18yF8YGRKXVbb5-X0QNu-XzjBCw0sxdwsMaTpy4Ij) 

Create a new schedule and click on the Interval dropdown to show what frequency of repetition you can use.

![Image](https://lh4.googleusercontent.com/l_GJej3C6xYmxrsbq4OBtZRc0fDJprTEPbfp8pgd5-s4QRGFT1MeOpCsUHB9WsKGIS7PeE4sjMW6jasvPx8tSyxl0ksVj-caEHNpcBqJcYibC4q0u-kudwgH-Uaoz_cqIQn696hW) 

You have the following options:
 
|Interval|Description|
|:-- |:-- |
|Every x minutes|Repeat every x minutes each hour of a day (x must be a factor of 60)|
|Hourly|Repeat every x hours in a day (x must be a factor of 24)|
|Daily|Repeat once per day at the time the schedule starts from|
|Weekly|Repeat once per week on the day of the week the schedule starts from|
|Monthly|Repeat once a month on the day of the month that the schedule starts from|
|Yearly|Repeat once a year on the day of the year that the schedule starts from|

 
Select the option that best suits your requirement.

#### Advanced Scheduling

If none of the previous options were viable for your Workflow's schedule then you can turn to the Advanced Schedule feature.
On the Interval property of a schedule, click the dropdown menu and click on Advanced Scheduler.

![Scheduling a Workflow 6](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%206.png?width=428&name=Scheduling%20a%20Workflow%206.png) 

This will present a series of new options so that you have extremely granular control over how and when the schedule will run.

![Image](https://lh3.googleusercontent.com/g2aOKHdIrUaeLuw2ezTp5Tofh8lA0hER1xOk_WnW9_kgHFcFmZzzYMtSfmCkt0mEYf6uRzlHu3AjNEElAeNE0QCPoi5_y9JTKy4z1CfDEY-k3ODaBjzi3ypW8ssMYjkh48oNn-so) 

Using the advanced scheduler you can specify the following:


- The minute(s) of an hour to run the schedule


- The hour(s) of a day to run the schedule


- The day(s) of the week to run the schedule


- The day(s) of the month to run the schedule


- The month(s) of the year to run the schedule

Simply select the options which fit your needs. Any categories which are left out in the advanced scheduler will default to "every" unit so if you fail to specify what day of the week the schedule should run on then it will run on every day of the week.

#### Disable and Enable Schedules

If you wish to temporarily disable a schedule as you are editing the workflow or there is maintenance being performed on your Toca platform then this can be easily achieved. 
Simply go to the project that contains the schedules in question and scroll to the bottom of the project page until you find your schedules.

![Image](https://lh5.googleusercontent.com/IIay6Wj3zd5lws8r0T4eUxvP6Dr4bsTkaHtMJ9aRyyrDOtyi_51E39dEekhZ3dJc0BsqIqfqaomc4iUL3XEPBgYsriXw21mFK4PseD6fXjzMaN55yFkfyhYam8euf3l2IcwevDYj) 

Hover over the schedule you wish to disable, this will reveal the schedules' menu.

![Scheduling a Workflow 9](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%209.png?width=236&name=Scheduling%20a%20Workflow%209.png) 

Click on the disable switch.

![Scheduling a Workflow 10](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%2010.png?width=232&name=Scheduling%20a%20Workflow%2010.png) 

This will disable the schedule until you enable it. To enable a schedule follow the exact same steps. 
A disabled schedule is identifiable as it is greyed out.

![Image](https://lh6.googleusercontent.com/haCNikTzNnMT7sMDSqt77yUAPH8cDI-211xzDYQD7BCh-n0UvZJ-r8NZ-j0qwwJ9RNE-WtRm11DnjXZbySensupNWqx_hgJVdFnVguRtK4k9dx4pIdqBef0hjc-2-kwHHc4j3JPy) 


#### Edit a Schedule

To edit a schedule, navigate to the project which contains the schedule you wish to modify. Scroll down to the bottom of the project page to find where the schedule is and hover over it to reveal the menu.

![Scheduling a Workflow 12](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%2012.png?width=236&name=Scheduling%20a%20Workflow%2012.png) 

Click on the pen icon to edit the schedule.

![Scheduling a Workflow 13](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%2013.png?width=237&name=Scheduling%20a%20Workflow%2013.png) 

This will open the schedule pop up which allows you to modify the schedule and save your changes.

![Image](https://lh4.googleusercontent.com/POYMs8q6-53N9RFqCUgsxMtDGQIrgUB17gi8txIOjFZ6smEAzdEgdJhXrPJMFQtpRC4QItue6e-fIG1kdE5lfiiQ-6TAZW9oBrE6xlvA4kyLI3BIy2PanM9tVBMcv1i_-qbV9ix3) 


#### Remove a Schedule

To remove a schedule, navigate to the project which contains the schedule in question. Scroll down to the bottom of the project's page and find the schedule you wish to remove. Hover over the schedule to show the menu for it.

![Scheduling a Workflow 15](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%2015.png?width=236&name=Scheduling%20a%20Workflow%2015.png) 

Then click on the bin icon to remove the schedule.

![Scheduling a Workflow 16](https://docs.toca.io/hs-fs/hubfs/Scheduling%20a%20Workflow%2016.png?width=230&name=Scheduling%20a%20Workflow%2016.png) 

This will trigger a popup to appear which will ask you to confirm this action as deleting a schedule is an irreversible process.
 

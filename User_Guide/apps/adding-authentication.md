
# Adding Authentication to Apps



 
By default, an App is set up so that it does not require users to login to use the App. This means that anyone can access and use it. If you wish to restrict access to your App then you have the following options:


- Username & Password



- No Registration allowed - Users must be manually added to the users table by the Apps creator


- Registration with Approval - Users can register for an account to use the App but they must be approved by the Apps creator before their account is created


- Registration with no Approval - Users can register for an account to use the App and no approval is required so anyone can sign up. The point of this option is so that you can monitor each user\'s activity as they will have a user ID against what they do on your App.


- OAuth 2 Login - Link your App with an Identity Provider (See the Administrator's Guide for how to set this up) so that people in your organisation can use their GSuite or Microsoft account to log into your App. This option is best if you want to distribute your App so that people within your organisation can use it.

Lets see how to set these different types of access up.

#### No Authentication

As mentioned above, the default setting for an App is to have unrestricted access so to set your App up be available to everyone simply untick the option to *Enable user login.*


![Image](https://lh6.googleusercontent.com/ssGgTOs0q1pxaBwpgZm7LXPjA16vB7uyw64ec-i28dV0-5viAypqZcKXkWpioOn4HU2NJ4bkKtMxd4mME-KLbu_cZsRnnk5c1US2d0x-FIS7fJoW6h4bHagFcPb6_0w-UqDwXmf6) 

 

#### Login only

If you want to restrict access of your App to a handful of people then you can add user login but without registration. This means that the Apps creator has to manually add and manage the users table. 
First you tick the option to *Enable user login.* This will then show a lot of new properties to fill in but don't worry, the wizard does most of the work for you!


![Image](https://lh6.googleusercontent.com/VC4GOGlT1NgHUgotBTWI4JKLcmKZ_fNnlC6JFAubK9cEWECBsxXJrBOeH8AmkgCEfH0uN5yqKpVw0iSk5yNGEQsfTP3iMCy5swPqpk5Cs0-LkENGwYuPgVP1xbrcQRQRtKj71ITW) 

The first property requires you to generate a secret, this is used to encrypt your users passwords and other sensitive information. Click on the button to the right of the field to automatically generate one.

![Adding Authentication 3](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%203.png?width=491&name=Adding%20Authentication%203.png) 

This will produce a long and random string of characters and numbers - fortunately you don't have to do anything with it and it is all handled for you.

![Image](https://lh4.googleusercontent.com/9046YsgUrmI3_AbmY7zpJHqs7rMpPMY-5F_6PseZfHkwGfpgJ6kmF2xfrh_ikfwkXfj5D2spY0ZXCVQUo_14K_tvmvxfP3Q6ffSIhEXy4ZNtn-znIch6ZUhURNQAyO1n5ZIHugg8) 

The next thing you are asked to do is set up a Users table which will store all the users who can access your App. If you have not already created a Users table then the wizard will create one for you.
First, choose a datastore which will store the users table (you must have linked a datastore to your App already for this to work). If you have not linked a datastore you can go back a step and link one in step 2 of the wizard.

![Image](https://lh4.googleusercontent.com/ZDqF5TLN80sZWSMzHe-oGKy6cOUJbadpUM2XvzUkogxYw3mcEfqRvmjHHdmIXO1ZdPJzStL2iXcP05td10rZOzQMrlTeWa2c6SVCBxcqMnPbPJV0e1ugwYbbTfrbM_Gb9CkXwDz2) 

Select the relevant datastore and by default the table name will be *users.* If this name clashes with a preexisting table or you want to name it to something else then you can.


![Image](https://lh6.googleusercontent.com/BGW7vWcLSWXFZBMdzjcfyXcdeYkIrDOdtl53LfcvwdxJXFN_ESjGFNfDSiJm5oQ3XDXuNvB05mqTYmgmDREBVX4ynwbOHL9jwsxPUzo0Ly4cPjLisHDffkvAtFUC3phBQ2GO84pX) 

As mentioned above, if you have not already created your user table the App will recognise this and offer to create the table for you, simply click CREATE TABLE when the prompt shows.

![Adding Authentication 7](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%207.png?width=481&name=Adding%20Authentication%207.png) 

The next and final step is to set up how users can log into your App.

![Image](https://lh6.googleusercontent.com/VHj55ygp_XgPaBTknaONv2VUSSuBDCmPXdb65R16Y_jOuPi7rl8HwJRJkI_f3jV58m4QgXg9RN_S8lhcgcUkM-iHBv2HKRZO7klzhwlkc-NYuTq3t4KltqIoODPdE9BAVO1KJP_B) 

The default method is *Username &amp; Password* which is correct if you want to have login without registration or login with registration.

The next two properties allow you to define the column names for the usernames and the passwords in your users table - these default to *username* and *password* respectively. If your table does not already have these columns then a prompt will appear and you can add the columns from the wizard - just click ADD COLUMNS when the prompt appears.



![Adding Authentication 9](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%209.png?width=269&name=Adding%20Authentication%209.png) 

If you do not wish for users to be able to register to use the App then untick the option to Allow user registration.

![Adding Authentication 10-1](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2010-1.png?width=269&name=Adding%20Authentication%2010-1.png) 

The final property is to tell the App which page to use as the Login page.

![Adding Authentication 11](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2011.png?width=493&name=Adding%20Authentication%2011.png) 

As this is a new App there are no pages yet so it will prompt you to create a new page.

![Image](https://lh3.googleusercontent.com/WksFZ_HueuFv6rCFCP9jRBFHd63XPHbA_wnghdzfMEdrHNZfazkCcZ_HfzVxewcrUwZi04c7Iok9ehgr26HM4qZMBcFNBUXji1VhMFes0MleZH8zX2NBts16fbhaspDzpHkDI5ve) 

Click on the + Add page option and a window will appear which shows you the details of the new page you're adding.

![Image](https://lh6.googleusercontent.com/zOyieHrIYo8DZsXyv-a2be8e08bwd1YjvRviIkIJ0GyOrfGJtNkXFa_Ihf4-Z8jLsUeUD4GOIXWDfdx32xCS8dpR_qUORra-vCHFHoK7kjxNB8Zvqpq-IiMAP4cORoFSERkDzRdv) 

This page will default to have the name *Login* and the URL slug (the text at the end of the url when you access this page) will default to *login*. You are free to change these. Once you are happy with the details for the login page click Add.



![Adding Authentication 14](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2014.png?width=148&name=Adding%20Authentication%2014.png) 

 
This concludes the user authentication step and you can click Next to continue with the wizard.

![Adding Authentication 15](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2015.png?width=448&name=Adding%20Authentication%2015.png) 


#### Login with Registration

If you want users to have the ability to register accounts to use your App then you have two choices.


- With approval - You must approve anyone who registers an account for your app.


- Without approval - Once a user is registered they can start using the app.

 
**With approval.** To let users register accounts for your App with your approval then follow the steps from the *Login only* section but instead of unticking the option to *Allow user registration*, make sure it is ticked.




![Adding Authentication 16](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2016.png?width=498&name=Adding%20Authentication%2016.png) 

When this option is ticked the wizard also shows the option to *Require approval once registered.* Tick this also.


![Adding Authentication 17](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2017.png?width=311&name=Adding%20Authentication%2017.png) 

Once this option is selected, a new field will appear beneath this option asking you to define a column in the users table which says whether a user is approved or not.

![Adding Authentication 18](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2018.png?width=514&name=Adding%20Authentication%2018.png) 

The column name for this new column defaults to *approved* but you can change it if required. If this column does not already exist in your users table you'll also notice a prompt appears letting you know that you can add the missing column. Click the ADD COLUMNS button to do this.


![Adding Authentication 19](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2019.png?width=466&name=Adding%20Authentication%2019.png) 

You have now successfully set up user authentication with registration that requires approval.
 
**Without approval.** To set up registration that does not require approval simply make sure the option to *Allow user registration* is ticked.



![Adding Authentication 20](https://docs.toca.io/hs-fs/hubfs/Adding%20Authentication%2020.png?width=437&name=Adding%20Authentication%2020.png) 

That is all that is required to allow users to register accounts for your App.

#### OAuth Login

The other type of login method is OAuth 2 login and this allows users who already have an account with the given Identity Provider (e.g. Google, Microsoft, Facebook) to login with those credentials. 

![Image](https://lh4.googleusercontent.com/aLDqkNJQ0xDeXOhNAw42Dh4xyLAdlxSVv-3BpcdOYaro6BT56GRjJDd3-mhL70KdJpaBVsDo6I4BiE2MuCFFvXUnwXdTi3QQDVUbM84PkseF4zX44Jz9pL3rNFKG7dtwHRmTvjmL) 

First, an administrator will need to set up an Identity Provider. Once this has been set up, you will be able to choose an Identity Provider and proceed with setting up OAuth 2 in your App.
In Scopes, enter the OAuth scopes that you require and which are available on your Identity Provider. One of the more common scopes is *OpenID*. Next, enter the Profile API URL. This is the endpoint supplied by the Identity Provider from which you can get the information you require in the scopes. For example, Google has a userinfo endpoint for *OpenID* scopes at [https://www.googleapis.com/oauth2/v1/userinfo](https://www.googleapis.com/oauth2/v1/userinfo). The Profile API Response Query is run on the JSON response from the Profile API URL. It is simply the path to the id field supplied by the Identity Provider. That will depend on the shape of the JSON returned by your Identity Provider. In the Google example, the id field is returned on the first level of the JSON response, so the query is simply `id`. If the id field was in an object called data, the path would be `data.id`. You can use [https://www.googleapis.com/oauth2/v1/userinfo](https://www.googleapis.com/oauth2/v1/userinfo) to test your query paths.





![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/OAuth/screenshot.1.jpg?width=434&name=screenshot.1.jpg) 

OAuth is implemented in Apps behind the scenes, so there is no need to add a login button. Simply mark a page with 'Require authentication' and users will be automatically redirected to your Identity Provider's OAuth service when they try to access that page. Once they have logged in, they are automatically redirected to the relevant page.
 

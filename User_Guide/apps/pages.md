
# Utilising Pages in Apps



 
Whilst sometimes you only need a single page for your App, other times you may require many pages. As an example you may need a login page, an About Us page, Home page and Contact Us page. Fortunately you can add as many pages as you like in each App.

#### Add pages

To add a page to your App you can either do so from the App Designer by clicking the + button next to the last tab.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/screenshot.3.jpg?width=335&name=screenshot.3.jpg) 

Or you can add a new page from the App's project page by clicking + NEW on the pages section.

![Pages 2](https://docs.toca.io/hs-fs/hubfs/Pages%202.png?width=602&name=Pages%202.png) 

When you add a page to your app you will be asked to define a name for the page and a URL slug although the slug will automatically populate based on the name you give the page.
 
![Image](https://lh5.googleusercontent.com/t2DxVqEUJKQOl8IyWvFmy0zD-6K_OmH6Fi6xdY-jpAWFpwS1sUfalPM1pN-WdGuDKeWuHHkoVgfTf6R8WAQZnTSbVhc7X3AqhxHSyVnNWQejmzesVmdSuYG3ClyZMjdgAQNeDeXN) 

If your App has user authentication set up then you can configure whether or not the new page requires a user to have logged in to be able to see it. If you try to access a page that requires authentication and you are not logged in then it will immediately redirect you to the login page.

#### Add links to pages

Now that you have added one or more pages to your App, how do you navigate between the pages? Well, as with most things in Toca, there are a few ways. 
 
**Navbar.** The most simple way is to put a Navbar layout component at the top of each page which will automatically add all pages in your App to the bar.


![Image](https://lh5.googleusercontent.com/jVPcgeYWjdfCBbXnevhTLcZo20G6c7NTiV7bFcLq3CpPA_e4MmmNPnvyVJvUqwizoothF5VaORyI6dYdVMNz2ZAljJCP2wU20INdqe4aYbQlw7vR2k1cOMdI6lmgS68vArXjcTB9) 

From the Navbar you can simply click on the page names and this will open up the requested page, you don't need to mess around with any links or URL paths.
 
**Links.** Another way to navigate around your App is with links embedded into buttons and other components. Drag a Link Button from the Content components into a layout component and open the properties panel.


![Image](https://lh6.googleusercontent.com/zsID1hAjznP3V4ROuzxL8D4u4cCzbuZkSsx3Jol79-INf0QVkj6JhS6SonyjpIvfbkYquV4DkZYZehqjmM7rodEdU0ZbogVUZlX1d6iNjrS0lRtvi1MbD_UspfvyGCkZNsB_VSpH) 

The second property is a Page dropdown which allows you to select which page clicking this link button should take the user to. Simply select the right one and give the link button a relevant label.

![Image](https://lh3.googleusercontent.com/h-qiAFowjEam8Eb83ntBJR1fks24v0VZeB-mQkmIdgPpKtMDRT1xBK7Ur2rhbIpbfpm-dxEzXZTKhDcLrEoglSdWZ0YOIIzpt1n6RKNRRtPpSknuV-9tuz9NT9aGil3xKO0rr7k-) 

And once we style the button up a bit it could look like the following:

![Image](https://lh4.googleusercontent.com/wML0-P_sN5jdKfSPmcSvlA_q37PSZ_5xRusoeLbBeQV1qKqiuZFmutPio7x8mIfqWNVXwCqEZ8XbH2T3zbd-NQZaElVGyz6V3ulBxjdoaTOvVw5FVMoM8tXFXYI9tb7q6Ix6dEqe) 


#### Opening pages as Modals

Sometimes it isn't necessary to open a new page as a whole new page and instead you just want to open the page as a smaller window on top of the current page. This is called a modal and on certain components you get the option to open a new page as a modal. A link button is an example of this, let's revisit the properties on a Link Button.

![Pages 8](https://docs.toca.io/hs-fs/hubfs/Pages%208.png?width=311&name=Pages%208.png) 

If you tick the option to open the linked page as a modal then this will open the page as a window on top of the current page. If we open the page now it looks like this:

![Image](https://lh3.googleusercontent.com/BXzsa7eViQ7v5TDN0xkgXGaqYn2QB4RQ8t0xNanj_ky_-p-AgsjiTOqHOJ1ctxwFc2T3nHq7rzxoXeCDHZDevk24XMqXRCjXzY9TxyWeYJ6VdjXPaZUYAxvEPKyhcbVd66S7j5JS) 

 

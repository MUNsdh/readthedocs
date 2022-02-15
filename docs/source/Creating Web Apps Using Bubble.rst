Introduction
============
Bubble.io is a code-free online web tool that is used to make many kinds of web applications. It is very versatile and can be used for anything ranging from social media sites, online marketplaces, landing pages, etc. This tutorial will explain the basics of using the interface and also show how to make a few simple web apps.

The Basics
==========
The following subsections will describe how to get started with Bubble and some of its most basic features that you will inevitably use while making your apps.

Creating a New App
---------------
To start making apps with Bubble, you must first create an account. After that is done, navigating to the home screen will show a label that says "My apps" along with a blue button which says "New app":

(Photo 1)

After clicking the blue button, a popup will appear that will allow you to give your app a name, specify the type of app you want to build, etc. Please note that your app's name must be unique from all other app names create on Bubble (not just your own apps):

(photo 2)

Press the blue button to be taken to the Bubble editor. You will see a popup on the left side of the screen called "New application assistant." By clicking "Let's get started," you will be able to change the icon and title that displays in your app's tab when it is running, along with a few other features that will be discussed later on.

(photo 3)

It is useful to keep in mind that you can always hover your cursor over anything in Bubble to get access to its reference page, where you can learn all about what it does.

(photo 15)

The Design Tab
--------------

You should now see the Bubble editor's Design tab. This is where you will decide how your app will look to its users. You will be able to drag and drop elements into the white area on the right side of the screen. You will also be able to resize, rotate and reposition those elements to your liking. Right now there is probably a default webpage showing where this white space would normally be, but that can easily be cleared by drag-selecting everything and pressing the "delete" button on your keyboard.

(photo 4)

The UI builder on the left allows you to add new elements to the page by dragging and dropping (or clicking and then dragging on the white space).You may notice several useful features under the "visual elements" dropdown:

(photo 5)

Here is a brief explanation of each:

| **Text** - Allows you to add text to the screen. Its font type and size can be changed.
| **Button** - Allows you to add a button to the screen. Making the button do something requires starting a *workflow*, which will be discussed later.
| **Icon** - Adds a common icon of your choosing to the screen (a "like" button, for example).
| **Link** - Adds hyperlinked text to the screen.
| **Image** - Adds an image to the screen.
| **Shape** - Adds a rectangle to the screen.
| **Alert** - Shows a temporary message when an event occurs. Triggered using a workflow.
| **Video** - Adds a playable video to the screen. Video must be accessed through Youtube or Vimeo.
| **HTML** - Allows you to embed HTML code into your web app.
| **Map** - Allows you to add a map that can be navigated and referenced by other elements in your app.
| **Built on Bubble** - Adds an optional Bubble watermark to your app.
| 
| Within the UI builder there is also a dropdown called "Containers." It contains several features that are necessary for almost every kind of web app:

(photo 6)

Here is what each container does:

| **Group** - Groups multiple elements together.
| **Repeating Group** - Repeats groups of elements vertically/horizontally on the page. Useful for displaying lists of data (comments on a post, for example).
| **Popup** - Shows a small "page" (really just a group) overlapping the original page when an event triggers it (a login popup, for example).
| **Floating Group** - A group of elements that stays in the same position on the screen as the user scrolls through the site.
| **Group Focus** - A group of elements that shows only when an event triggers it, and disappears once the user clicks outside of it.
| 
| The UI builder also has a dropdown titled "Input forms." These elements allow the user to enter information into the web app:

(photo 7)

Here is what each input element does:

| **Input** - Allows the user to enter a single-line input.
| **Multiline Input** - Allows the user to enter a multiline input.
| **Checkbox** - Adds a checkbox to the interface.
| **Dropdown** - Allows the user to choose an input from multiple options (an example would be sorting posts in order of most popular, most recent, or least recent).
| **Search Box** - Searches a database for the user's input and provides search suggestions.
| **Radio Buttons** - Allows the user to choice from a list of choices, but only one option is allowed at a time.
| **Slider Input** - Lets the user choose a value from a range of values (or specify a range within these values).
| **Date/Time Picker** - Lets the user input a date (and time, if needed).
| **Picture Uploader** - Lets the user upload an image to the app.
| **File Uploader** - Lets the user upload a file (of any type) to the app.
| 
| In each element dropdown, you may notice that there is an option to "Install more..." at the bottom. Clicking this option opens the plugins page, which will be discussed later. These are all the basic UI elements that you will need to build your apps.

The Workflow Tab
----------------

(photo 8)

The purpose of this tab is to add functionality to the elements you created in the design tab. For example, the event that occurs as a result of pressing a button would be specified here. The triggers/actions that can occur in a given workflow are too numerous to list in this tutorial, so it is best just to learn them as you need them. We will briefly talk about the basic interface.

Clicking on the event block lets you specify which event will trigger the action. It could be a page loading, a button being clicked, a popup opening, etc. Once an event is picked, a action section will appear, allowing you to choose what happens when this event occurs.

(photo 9)

Actually using the options presented in the actions tab is mostly self-explanatory, but can quickly become complicated in the later stages of building your app. The best way to get comfortable using it is through examples, which are available in the later sections of this tutorial.

The Data Tab
-------------
As you use Bubble, you will start to see references to database terminology:

| **Types** - Data templates that have several fields. For example, "user" is one of the preloaded data types in Bubble. Its fields include the user's email, the date their account was created (Created Date), the date the user's account was modified (Modified Date), and the user's account's slug. The "User" type defines what data is associated with a user's account.
| **Things** - Instances of a type. To use the "User" example again, this would refer to a specific user's account. When you create a new thing, you must specify what this thing's type is. If it is of type "User", then you are creating a new user account.
| **Fields** - Attributes of a type. A thing of type "User" has an associated Email, Creation Date, Modified Date, and Slug. More fields can be added to a type as desired, but default fields cannot be deleted.
| 
There are several tabs within the data tab, each dedicated to dealing with different parts of your app's data. Each will be described below.

| **The "Data types" Tab** - This tab deals with creating, viewing, editing, and deleting data types. It also lets you add/delete fields of each type (except for the default fields).

(photo 10)

| **The "Privacy" Tab** - This tab Lets you set privacy rules for each data type, such as what can be shared or searched by other users.

(photo 11)

| **The "App data" Tab** - This is where you can view, create, edit, or delete instances of different types (things). For instance, the information of someone who created an account with your app would be accessible in this tab.

(photo 12)

| **The "Option sets" Tab** - Allows you to create, view, edit, and delete dynamic sets.

(photo 13)

| **The "File manager" Tab** - Allows you to upload, view, and delete files that users have uploaded to your app (can be of any file type).

(photo 14)

The Styles Tab
--------------

(photo 15)

This tab opens automatically whenever you try to edit the style of one of the elements in the design tab. It allows you to change the appearance of the element by altering fonts, colors, shapes, etc.

The Plugins Tab
---------------

(photo 16)

Bubble has a vast library of plugins for integrating third-party services into your app. Some of the most popular plugins allow you to integrate Facebook, Google, Amazon, PayPal, etc. directly into your app. Pretty much any app that you could ever want to make will require a plugin.

First Example: Social Media App
===============================

In this section, we will create an app that can do the same basic functions as most social media apps. The user will be able to create posts (with pictures, if they want), like other people's posts, comment on those posts, and reply to those comments. We will also implement a "map" feature, which will show where each post was created on a map.

Creating the Header as a Reusable Element
-----------------------------------------
If you look at a web app today, most (if not all) of them use a header. A header is simply a bar at the top of the screen showing the site's logo, the sign in/sign up button (or the user's username and profile photo if they are signed in), and tabs for navigating the site.

We will start by clicking the dropdown menu in the top-left corner of the screen to see all the pages that current exist in our web app. The reusable elements are also listed here. 

(photo 17)

From here, we will click "Add a new reusable element" to create our header. Give the header element a unique name and click CREATE.

(photo 18)

You will now be taken to a new page. The white block that you see in the center of the screen will become our reusable element. You can edit the properties of any element in Bubble by double-clicking on it. Double-click on the white box to change its width to be the same as the width of your index page (usually 1080px). Also adjust the height and color to your liking.

(photo 19)

Now we will add a logo to out header. Select the "Text" element from the visual elements dropdown on the left, then click and drag over the rectangle we just edited. This clicking and dragging is how all elements are added to your app. Double-click the textbox to change the font size, type, and color of the logo to be on-brand with your website. You may notice that the text does not show up in the editor, despite the text being visible when the app is running or when you use the element in another page. This is likely just a bug, and should not affect your app.

Lets add a Login/Sign up button to the header. We want the button to open a new page where the user can login or sign up. Create a new page using the dropdown in the top-left corner and name it "sign in page" or something similar. Click the "Button" element and place it somewhere on the header. Now lets open the button's properties window and click the "Start/Edit workflow" option.

Bubble will assume that the event that triggers the action is when the button is clicked. Click on the box below it to add an action and go to *Navigation > Go to page...* to make the button move the user to another page. A window will pop up requiring a "destination". Input the page you created for signing the user in.

(photo 20)

You can now test your button. Navigate to the "index" page and add the header to the top of the screen (find the "Reusable elements" dropdown on the left). Click "Preview" in the top right corner and you should be taken to a new tab where you can test your app. When you click a button, you should be taken to a blank page.

(photo 21)

As an exercise, you can also make your logo act as a button that takes you back to the "index" page. The process for doing this is almost identical to the process for the button. (hint: you can only edit elements within a reusable element by going back to that element's page using the page dropdown.)

Account Functionality
---------------------
It is surprisingly simple to create a login/sign up system in Bubble. Navigate to your sign in page and Add input lines for the user's email, password, and password again (retyped for confirmation). For the email line, type "Enter an email" as a placeholder and select Email from the dropdown menu for "Content format". For the passwords, type "Type a password" and "Retype password" respectively for the placeholders of each, and set their content formats to "Password".

Now add a button below these input lines that says "Sign up". You can also add some text above the input lines that says "Sign Up". Your page should now look something like this:

(photo 26 cropped)

Now open up the properties for the sign up button and start a workflow. Add an action by navigating to *Account > Sign the user up*. A window will pop up with multiple options. 

(photo 23)

First, check the "Require a password confirmation" checkbox. This will mean the user must type the password in the second password input as well as the first to create an account. Now click the red box next to "Email" and click the options so that it says **Input Enter an email's value**. Next, click the red box next to "Password" and click the options to say **Input Type a password's value**. Lastly, put **Input Retype password's value** next to "Confirmation". The window should now look like this:

(photo 24)

You can now test the sign up functionality using the "Preview" button. Nothing will actually change in the test app yet, but you can go to the "App data" section of the Data tab to see if a new entry has been created under "All Users":

(photo 25)

You may notice that the input fields do not become empty when you click the "Sign up" button. This does not affect the functioning of the app, but it does look messy. To fix this, we can add an extra step to the end of the "Sign up" button's workflow to clear all inputs. Open the button's properties window and click the button to edit its workflow. Add another action to happen after signing the user up under *Element Actions > Reset inputs*. This will reset all the inputs on the page to be their default value (which we have kept empty).

Now lets add the inputs for logging in. The workflow for this is very similar to signing the user up, except the password is only needed once. Lets add another email and password input along with a "Login" button and a title. The result should look like this:

(photo 26)

Enter the login button's workflow and select *Account > Log the user in*. Enter **Input Email's value** next to Email and **Enter Password's value** next to password. Once again, start another action to reset the inputs. The log in/sign up functionality is now complete!

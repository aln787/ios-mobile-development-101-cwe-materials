---
title: iOS Development 101
duration: "1:25"
creator:
    name: John Doe
    city: NYC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) iOS Development 101

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*
- Explain relevant history and trends in iOS development.
- Identify key skills leveraged by iOS developers.
- Survey the common tools used within the iOS ecosystem.
- Apply key concepts and skills to build your own basic iOS application.
- Create a custom learning plan to help you continue to build fundamental iOS development skills after this workshop.

### STUDENT PRE-WORK
*Before this lesson, you should already be able to:*
* Bring a Mac laptop (*required*) and iOS testing device (*optional*).
- Upgrade your OS to the latest version.
- Download and install the latest version of [Xcode](https://developer.apple.com/xcode/).

### INSTRUCTOR PREP
*Before this lesson, instructors will need to:*
- Review & modify lesson plan & slide deck as needed
- Write learning objectives & relevant information on board

### WORKSHOP AGENDA
| TIMING  | TYPE  | TOPIC  |
|:-:|---|---|
| 10 min  | [Opening](#opening)  | Greetings + The GA Experience  |
| 15 min  | [Introduction](#intro1)   | Discuss history & scope of iOS development |
| 15 min  | [Demo](#demo1)  | Visualize the iOS ecosystem  |
| 20 min  | [Guided Practice](#guided-practice1)  | Navigate your iOS environment |
| 20 min  | [Independent Practice](#ind-practice1)  | "Test" your iOS skills |
| 5-10 min  | BREAK  |   |
| 15 min  | [Introduction](#intro2)   | iOS Fundamentals: What Do You Need to Know?  |
| 15 min  | [Demo](#demo2)  | Foundational Concepts in Your Xcode IDE |
| 20 min  | [Guided Practice](#guided-practice2)  | Practice iOS Fundamentals |
| 20 min  | [Independent Practice](#ind-practice2)  | Apply iOS Fundamentals |
| 10 min  | [Conclusion](#conclusion) | Review + Recap |
| 10 min  | [Takeaways](#takeaway) | Learning Plan, Q&A |

---

<a name="opening"></a>
## Opening (# mins)

> Note: Let people know where restrooms and kitchen are located, as needed.

#### Instructor Bio

Welcome to iOS Development 101! Here's a bit about me:
> Provide your name and brief bio, including: your background in iOS development, any experience you've had with GA, and one "fun fact" about yourself.

#### Introduce Yourselves

Before we dive in, a bit about you!

> Have students introduce themselves: name, what brings them to GA (ask for their current career & any specific goals), & one "fun fact".

> **Example Exercise**: *Have students submit this information in a format easily accessible so you can input information into a demo/dummy app that describes the class.*

> **Alternate Exercise**: *Have students share their information in pairs/groups and have other pairs/group members recite this information back to the class.*


#### Our Expectations

- You're ready to take charge of your learning experience.
- You have a Mac laptop and *optional* testing device.
- You've downloaded and installed the latest version of [Xcode](#).
- You're curious and excited about iOS development!

#### Our Objectives

> Note: Write workshop objectives on board before class

- Why this topic matters (general relevance)
- Why this topic rocks (interest/hook)

> Note: Tailor these 2 points to student interests. Relate to their career info & goals students described during attendance.


***

<a name="intro1"></a>
## Introduction: History & Scope of iOS Development (15 mins)

### What is iOS?

iOS is the operating system that powers the iPhone and iPad. It's based on a set of frameworks and programming languages that power all of Apple's devices, including Macs and Macbooks (macOS, or until recently, Mac OS X), the Apple TV (tvOS), and the Apple Watch (watchOS). Learning iOS is a great starting point for gaining access to the rest of Apple's device ecosystem, and as Apple continues to standardize the frameworks that power these devices, the easier it is to build for all of them simultaneously by sharing code.

iOS stems from a long history of Apple development. Most notable is Objective-C, a 30-year old programming language, which still exists as a viable, low-level language for building apps. However, _Swift_ is the new language of choice for Apple development, being more modern, approachable, and automated than Objective-C. It's a great way to build apps as well as learn programming if you're new to code.


***

<a name="demo1"></a>
## Demo: Visualizing the iOS Ecosystem (15 mins)

### Xcode

Xcode is an integrated development environment (or IDE) made available to every Mac owner and contains nearly all of the tools necessary for building apps for iOS. It's essentially an app that contains all the tools for building apps.

It is a combination of tools that work together (hence, "integrated") in a single place (hence, "environment") for developing apps and programs. By using Xcode, you can learn Swift, develop projects that work on any Apple device, and simulate those apps without having to own a mobile device, Apple watch, or Apple TV.

Those tools integrated into Xcode consist of a code editor, "Playgrounds," Interface Builder, an iOS device simulator (or just, "simulator"), a debugging suite, and other various tools that help with editing various files that comprise an app (property lists, data schemas, etc.).

Xcode can be downloaded from the Mac App Store, along with other third-party tools used for testing and building various components that go into apps (like icons). Other popular tools exist online that enable us to use open source code to simplify our iOS development.

### The Ecosystem

Before we start diving into building iOS apps, there are some concepts we have to introduce.

The "operating system" is the software that provides the environment in which our apps live. This is iOS, which is analogous to Windows, Linux, or Android, but runs exclusively on Apple's mobile devices.

"Frameworks" are code that Apple provides that standardize the interaction between our apps and the operating system and device. For example, the "UIKit" framework provides user interface elements like buttons, toolbars, and tables that comprise user interfaces. It means we don't have to worry about writing code that draws typical elements, and it provides a consistent look-and-feel between apps.

Once you start working with code, you'll take advantage of third-party frameworks (also called "libraries" or "packages") written by other iOS developers that will make your life easier. For example, one library called `SDWebImage` is used to load images from the Internet asynchronously (so the UI doesn't stall), and cache them on the device (so you only have to download them once).

### Parts of an App

Xcode enables you to develop almost any aspect of an app in one place. Here are the things that we're going to need to know to be effective with building apps:

**User Interfaces.** Interface Builder enables you to build UIs for apps in a kind of visual flowchart. In fact, Xcode's Interface Builder is so robust, that you can prototype entire apps and run them on your iPhone without needing to write a single line of code! You can drag-and-drop interface components onto screens that will adapt to the user's device size and its orientation. Also, Xcode has features that present code and UI side-by-side, so you can work with them together conveniently.

**Code.** Xcode naturally gives you the ability to write code, but its integrated nature means it "understands" the code much more than a basic text editor would. This means you can reference Apple's documentation, jump to places where functions or classes are defined, and even get suggestions on what to write next, all from Xcode itself. When you're writing code, you might want to try something out before committing it to the app itself, so Xcode provides _Playgrounds,_ interactive environments that evaluate Swift code in real time.

**Tests.** Learning to write tests (code that ensures your code runs correctly) is a major step in becoming a professional app developer. Xcode provides facilities to help you automatically build your app. Tests enable you to make changes with confidence. _And don't let anyone convince you that "moving faster" is more important!_ Writing tests empowers you to move faster, because you won't have to fix all the bugs that will result from changing untested code!

**Assets.** These are all the media files that you need to make an app look professional and consumable by customers. This includes icons, videos, graphics, etc. Xcode puts them into a Media Library so you can access them from any part of the app.

In this course, we'll introduce you to building a simple app with Interface Builder and running it in the simulator (or on your device, if you so choose). This will enable you to deploy app prototypes on your phone and demonstrate them to others. We'll also give you some resources to continue your learning and dive into powering that app with actual Swift code.

***

<a name="guided-practice1"></a>
## Guided Practice: Navigating your Xcode environment (15 mins)

### Create an Xcode Project

An Xcode "project" contains everything needed to make one or more related apps. If you're building for iPhone, iPad, Apple TV, and a Mac, you can share code between those apps and deploy them to Apple's App Stores all from Xcode.


### What's in an Xcode project?

There are four file types that come with an Xcode project.


### Introduction to Interface Builder

#### What are Storyboards?

Storyboards are a mechanism that enables you to compose multiple Scenes, the transitions between them, and their respective Views in a single place.

Sitemaps that web designers draw show the structure of the site and describe the "flow" from one page to another. Storyboards are like this. It shows various screens of the app (called "Scenes"), and how one flows to into the next. Each line of flow (transition) from one Scene to the another is called a "Segue."

#### View Controllers + Scenes

View Controllers manage Views and generally represent one "Scene" of an app. We can attach a bunch of code to a View Controller. That’s where the "logic" for an app generally lives.

#### First, disable Auto Layout.

Auto Layout is the modern way of building responsive interfaces for iOS. That means that you can declare rules for how the app should adapt a user interface for multiple devices, like an iPhone SE, iPhone 6S, iPad, etc., without having to build a separate Storyboard for each device.

Auto Layout is quite complicated. It gives you a lot of power as an app developer, but it hours of practice to gain the basics (and even longer to master). We're going to avoid it for now by using the "old school" method of automated layout called "Springs-and-Struts."


### What are views?


- Launch Xcode.
- How to create a project.
- What's in an iOS project? (file types)
- What are views?
- Disable auto layout.
- Add a text field to a view controller in Interface Builder.
- Run your app in a simulator.
- Tap on the text field, enter text. Observe how UIKit automates the keyboard appearance and animations.
- Change properties of the text field in Interface Builder.

***

<a name="ind-practice1"></a>
## Independent Practice: "Test" your user interface skills (20 mins)

Change the keyboard of the text field to an email entry.

Add another text field to the view controller below the initial on. Add placeholder text that says, "Password". In the text field's properties, check the box that says "Secure text entry" in order to conceal the characters the user will type.

Find a button in the UI library and add it below the password field. Double-click it to change its text to "Sign In".

Run the app in the iOS simulator. Verify that the top text field, when tapped, shows a keyboard that has an "@" symbol. Also verify that the password entry field obfuscates any typed characters.

Tap on the button. Does it animate?


***

> **BREAK**

***

<a name="intro2"></a>
## Introduction: App Fundamentals (15 mins)

- Storyboards for complex user interfaces.
- Playgrounds for Swift experiments. Quick intro.
- We can prototype apps using Interface Builder alone.
- We can also prototype code in Playgrounds.
- Ultimately, you'll learn how to power the UI with code. But not in this workshop.

***

<a name="demo2"></a>
## Demo: App Fundamentals: Storyboards (15 mins)

### Navigation Controllers

Navigation Controllers manage View Controllers. A Navigation Controller decides which View Controller to display at any given moment, and it also keeps track of the ones that it has displayed previously and in which order. Think of it like how a web browser keeps track of history.

There are a couple of terms we need to introduce to understand what's going on in the Storyboard when we introduce a Navigation Controller:

* Initial View Controller - The first View Controller an app will display when launching.
* Root View Controller - The first View Controller that a Navigation Controller will show.

There are a couple of ways to add a Navigation Controller, but we'll use one that makes it easy to get started:

1. Select the View Controller in Interface Builder.
2. Go to the menu item `Editor > Embed In > Navigation Controller`.
3. Notice how the IB canvas shows another box labeled "Navigation Controller," which points to your original View Controller.

### Segues

Segues are animated transitions between two View Controllers. The Source View Controller renders the scene a user sees before the Segue, and the Destination View Controller is the one the UI will render afterwards. There are several types that determine how a View Controller is "presented" to the user.

For example, when a user taps on the "Sign In" button, we would want first to check the user's password (which we won't do this time), then if the password is correct, have the current scene "segue" to the home scene of the app.

### Creating a Segue

The Navigation Controller gives your app the ability to use Segues. Here's how to add that next Scene to your app and Segue to it:

1. Drag a UITableViewController to the canvas, just to the right of the login scene.
2. Press CTRL and click-and-drag from the "Sign In" button to the UITableViewController.
3. You should see a blue line and when you hover over the table, it should highlight.
4. Let go of the mouse button. A small dark menu should appear. This is asking you what kind of Segue you want to create.
5. Click on "Push."
6. Run your app!

Now, when the app loads, you should see a Navigation Bar at the top, and when you click on the "Sign In" button, it should segue to the table, which slides in from the right.

Note how the table view controller shows a "Back" button at the top. This is one of the conveniences that the Navigation Controller offers. Let's explore a bit how this works:

1. Go back to Interface Builder.
2. Click on the original Scene you made, which we'll call the "Login View Controller."
3. Double-click in the middle of the Navigation Bar at the top.
4. When the editor appears, type "Login".
5. Run your app.

Now when you tap "Sign In," the back button now says "Login," reflecting the title of the previous (i.e. Source) View Controller. The Navigation Controller "knows" which View Controllers it has shown to the user. Later, you'll be able to use this fact (leveraging Swift, of course) to pass data between the View Controllers, like the user's email address.

***

<a name="guided-practice2"></a>
## Guided Practice: App Fundamentals: Media and Tables (20 mins)

We're going to investigate one of the most common design patterns in iOS, the master/detail view. A master view is a list of a set of items, like the view of tweets in the Twitter app. The detail view is a whole-screen view that shows _details_ about a selected item from the master list.

To do this, we're going to create a catalog of objects, introduce the process of importing media that you'll find in Google Image Search (or another source), then include the images in the project's media library.



- Add media to the media library.
- Drop in an image on the front page.
- Drop media into the first cell in the table.
- Add a segue from the cell to a new view controller.

***

<a name="ind-practice2"></a>
## Independent Practice: Apply App Fundamentals (20 mins)

- Add more images and labels to more cells in the table.
- Add more view controllers. Segue to them.
- Add more views to the target view controllers (images, text views, labels).
- Run the app and test it.
- Have others test it.
- Tweak and modify properties of the text and other views.

***

<a name="conclusion"></a>
## Conclusion: Review + Recap Topics (10 mins)

> Review Deliverables

> Review Topics Covered

***

<a name="takeaway"></a>
## Takeways: Learning Plan + Q&A (15 mins)

#### What Should You Do Next?

- Check out the learning resources at https://developer.apple.com.
- Download Apple's new Swift iBook.
- Watch videos from WWDC.
- Read more about Apple technologies.
- Practice using Xcode to build app prototypes.
- Download sample icons from thenounproject.com
- Download Prepo from the App Store to size media and import it into your app.
- Start linking user interface to code via IBOutlets and IBActions.
- Learn more about mobile design and what makes it unique and powerful.


#### Q & A

***

## ADDITIONAL RESOURCES

- [a](#)
- [b](#)
- [c](#)

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

iOS stems from a long history of Apple development. Most notable is Objective-C, a 30-year old programming language, which still exists as a viable, low-level language for building apps. However, Swift is the new language of choice for Apple development, being more modern, approachable, and automated than Objective-C. It's a great way to build apps as well as learn programming if you're new to code.


***

<a name="demo1"></a>
## Demo: Visualizing the iOS Ecosystem (15 mins)

### Xcode

Xcode is an integrated development environment (or IDE) made available to every Mac owner and contains nearly all of the tools necessary for building apps for iOS. It's essentially an app that contains all the tools for building apps.

It is a combination of tools that work together (hence, "integrated") in a single place (hence, "environment") for developing apps and programs. By using Xcode, you can learn Swift, develop projects that work on any Apple device, and simulate those apps without having to own a mobile device, Apple watch, or Apple TV.

Those tools integrated into Xcode consist of a code editor, "playgrounds," Interface Builder, an iOS device simulator (or just, "simulator"), a debugging suite, and other various tools that help with editing various files that comprise an app (property lists, data schemas, etc.).

Xcode can be downloaded from the Mac App Store, along with other third-party tools used for testing and building various components that go into apps (like icons). Other popular tools exist online that enable us to use open source code to simplify our iOS development.

### Parts of an App

Before we start diving into building iOS apps, there are some concepts we have to introduce.

The "operating system" is the software that provides the environment in which our apps live. This is iOS, which is analogous to Windows, Linux, or Android, but runs exclusively on Apple's mobile devices.

"Frameworks" are code that Apple provides that standardize the interaction between our apps and the operating system and device. For example, the "UIKit" framework provides user interface elements like buttons, toolbars, and tables that comprise user interfaces. It means we don't have to worry about writing code that draws typical elements, and it provides a consistent look-and-feel between apps.

Once you start working with code, you'll take advantage of third-party frameworks (also called "libraries" or "packages") written by other iOS developers that will make your life easier. For example, one library called `SDWebImage` is used to load images from the Internet asynchronously (so the UI doesn't stall), and cache them on the device (so you only have to download them once).


***

<a name="guided-practice1"></a>
## Guided Practice: Navigating your Xcode environment (15 mins)

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
- Playgrounds for Swift experiments.
- We can prototype apps using Interface Builder alone.
- We can also prototype code in Playgrounds.
- Ultimately, you'll learn how to power the UI with code. But not in this workshop.

***

<a name="demo2"></a>
## Demo: App Fundamentals: Storyboards (15 mins)

- Add a navigation controller.
- Add a segue from the button tap to a UITableViewController.
- Run the app and demonstrate the segue.

***

<a name="guided-practice2"></a>
## Guided Practice: App Fundamentals: Media and Tables (20 mins)

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

- Learn about Swift.
- Learn about IBOutlets and IBActions to "link" UI with code.
- Check out the learning resources at https://developer.apple.com.
- There's a new Swift iBook with interactive lessons!

#### Q & A

***

## ADDITIONAL RESOURCES

- [a](#)
- [b](#)
- [c](#)

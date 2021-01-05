# Hello, World

## Hello world App

Create an app with the famous greeting - "Hello, world!" in some language of your choice. Add the iOS logo from the resources folder.

## Create project

Create a new Xcode project > Select **iOS** platform > **App** > Leave Interface to Storyboard and Life Cycle to UIKit App Delegate > select **Objective-C** from the Language menu > you could check Use Core Data and Include Tests, but we will not focus on those 2 for now...

Don't forget to add **.gitignore** to your repo, [this](https://github.com/github/gitignore/blob/master/Objective-C.gitignore) is good enough for a starter.

## Some guidance

### Creating the UI

Select `Main.storyboard`, the place where you could create the UI skeleton for the app. Right beside the toggle for showing/hiding Code Review, there is a + button from where you could browse UI components.

### Connecting it with your code

Split your screen, you should have `Main.storyboard` on one side and `ViewController.m` on the other. Tap and hold on some UI element, press Control and by dragging you should be able to create an **[IBOutlet](https://www.hackingwithswift.com/example-code/xcode/what-is-an-iboutlet)** in the interface section of the file.

Then you could set them in the `viewDidLoad` method.

### Usefull controls

- [UIImageView](https://developer.apple.com/documentation/uikit/uiimageview?language=objc)
- [UILabel](https://developer.apple.com/documentation/uikit/uilabel?language=objc)

## If that was easy enough

Create an app with a text field for your name and Done button on the first screen, and some greeting in the same fashion as above on the second screen.

## Again, guidance

You can just modify the existing app.

### For the first screen

You will need a **[button](https://developer.apple.com/documentation/uikit/uibutton?language=objc)** connected with your `ViewController` implementation by an **IBAction**.

When the button is tapped the second ViewController should be instantiated, its greeting set and then presented.

### For the second screen

Add new file > Select **Cocoa Touch Class** > Name it > Inherit UIViewController instead of NSObject.
Add UIViewController in the **Interface Builder** and set its `Class` and `Storyboard ID`.

# JSButton
[![Version](https://img.shields.io/cocoapods/v/JSButton.svg?style=flat)](http://cocoapods.org/pods/JSButton)
[![License](https://img.shields.io/cocoapods/l/JSButton.svg?style=flat)](http://cocoapods.org/pods/JSButton)
[![Platform](https://img.shields.io/cocoapods/p/JSButton.svg?style=flat)](http://cocoapods.org/pods/JSButton)
![Language](https://img.shields.io/badge/language-Swift%203-orange.svg)
[![Twitter](https://img.shields.io/badge/twitter-@imjog24-blue.svg?style=flat)](https://twitter.com/imjog24)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

<img src="https://github.com/imjog/JSButton/blob/master/Example/jsbuttonss.png" width="300">

## Demo

```bash
$ pod try JSButton
```

...or clone this repo and build and run/test the `JSButton` project in Xcode to see `JSButton` in action. If you don't have [CocoaPods](http://cocoapods.org) installed, grab it with `[sudo] gem install cocoapods`.

```bash
$ cd Example
$ pod install
$ open JSButton.xcworkspace
```

## Requirements
- iOS 8.3+
- Xcode 9.0
- Swift 4.0

## Installation

JSButton is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "JSButton"
```
### Manual Installation

Just drag the `JSButton.swift` files into your project.

### IBDesignable

`JSButton` includes `IBInspectable` annotations to enable configuring the label inside Interface Builder. However, if you see these warnings when building...

```
IB Designables: Failed to update auto layout status: Failed to load designables from path (null)
IB Designables: Failed to render instance of JSButton: Failed to load designables from path (null)
```

...then you are likely using `JSButton` as a static library, which does not support IB annotations. Some workarounds include:

- Install `JSButton` as a dynamic framework using CocoaPods with `use_frameworks!` in your `Podfile`, or with Carthage
- Install `JSButton` by dragging its source files to your project

## Usage
### Creating a view from the storyboard

- If you already have a Label where you want to use then set it's `class` to `JSButton` in identity inspector.

- Or drag a **Button** from object library and then change it's `class` to `JSButton` in identity inspector.

- Set the `module` property to `JSButton`.

<img
src='https://github.com/imjog/JSButton/blob/master/Example/jsbuttonclass.png' width='260' alt='Add JSButton to storyboard'>

- Customize the view properties in the attributes inspector.

<img
src='https://github.com/imjog/JSButton/blob/master/Example/jsbuttondesignable.png' width='360' alt='Attributes inspector'>
<img
src='https://github.com/imjog/JSButton/blob/master/Example/jsbutton1.0.0-features.png' width='360' alt='Attributes inspector'>

### Add action to button
To add action to your button just use `.action` you dont have to add Target and then handler function.
```swift
yourButton.action {
  print("Button Pressed!")
}
```

## Author

<table>
<tr>
<td>
     <img src="https://avatars2.githubusercontent.com/u/20956124?s=400&u=01fab3fc9bb3d2ee799e314d3fe23c54d1deeb07&v=4" width="180"/>
     
     Jogendra Singh

<p align="center">
<a href = "https://github.com/imjog"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "https://twitter.com/imjog24"><img src = "https://www.shareicon.net/download/2016/07/06/107115_media.svg" width="36" height="36"/></a>
<a href = "https://www.linkedin.com/in/jogendrasingh24/"><img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36"/></a>
</p>
</td>
</tr> 
  </table>

## What's next

- Any suggestions?

## Contribution

- If you found a **bug**, open an **issue**
- If you have a **feature request**, open an **issue**
- If you want to **contribute**, submit a **pull request**
- If you have any issue or want **help**, please drop me a mail on jogendra.iitbhu@gmail.com

## License

JSButton is available under the MIT license. See the [LICENSE](https://github.com/imjog/JSButton/blob/master/LICENSE) file for more info.

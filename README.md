# Recast.ly-native

Now that you have done the Recast.ly sprint, the next step is to implement the application in a mobile application using [React Native](https://github.com/facebook/react-native). iPhone applications are usually written in Swift/Objective-C, and Android applications are usually written in Java, but React Native allows you to deploy to both platforms in Javascript. 

## Before getting started with this sprint, you should:

- [ ] Know how to import and export React files
- [ ] [Know how to think about web apps as components](https://cloud.githubusercontent.com/assets/6980359/12561583/cf9b2a1a-c355-11e5-9fe6-9aeffbce4a28.png)
- [ ] Know what props are, and how to pass them in
- [ ] Know what state is, and how it affects the render cycle
- [ ] Be familiar with ES6 properties such as destructuring and fat arrow functions


## Getting started

One of the most difficult things about getting started with React Native is the work required to get your enviornment setup. While React Native works with both iOS and Android, you cannot use the iPhone simulator on a Windows or Linux machine, but you can use the iPhone and Android simulator on a Mac. The following instructions need to be done for both iPhone and Android

- [ ] Upgrade to the latest version of Node
- [ ] Run `npm install -g react-native-cli`
- [ ] Run `brew install watchmen`

## For iPhone 
- [ ] [Download or update XCode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12), which is Apple's SDK for all of Apple's platforms (iPhone, iPad, iWatch, Macbook, iMac, etc)

## For Android (TODO: Currently incomplete)
Android has a lot more initial setup than iOS
- [ ] Download the [Android Studio SDK](https://developer.android.com/studio/index.html)
- [ ] Download the [JAVA SE](http://www.oracle.com/technetwork/java/javaseproducts/downloads/index.html)
- [ ] Once both is installed, you'll need to add a default simulator within Android Studio SDK (Screenshots and more clear directions coming soon)

Once everything is updated and installed, 

- [ ] In a new directory, run `react-native init (NAME OF PROJECT)`. This process takes a while
- [ ] cd into the project, and then either run `react-native run-ios` or `react-native run-android`. For this sprint, we will be using the iOS simulator

After running `react-native init` you'll notice once you open the project that the boilerplate includes two files, `index.ios.js` and `index.android.js`. These are the respective starting points for the application. 


## Understanding the differences between developing for web and developing for mobile

Mobile applications are different than web applications, and there are somethings you need to keep track of as you learn React Native

* In each component, you'll need to import react and react-native
* Mobile applications do not have a DOM, and do not have HTML elements. Instead, they have VIEW and TEXT tags, which can be pulled from the react-native module. 
* The root file contains `AppRegistry.registerComponent...` this is the starting point to the application, the index file is the only one that should have it. 
* Because there is no DOM and no HTML, that also means there is no CSS. Instead, react-native has its own styling that is very similar to css. Each component should have it's own style guide, [try it out in this sandbox](https://facebook.github.io/react-native/docs/style.html)
* Mobile devices have properties that are unique to them, such as cameras, scroll views, geo location, pinching, swiping, etc. All of those features and demos of them can be found at the [React Native page under APIs](https://facebook.github.io/react-native/docs/tutorial.html). 

## Resources

* [React Native Docs](https://facebook.github.io/react-native/docs/tutorial.html)
* [List of useful React Native Links](https://github.com/enaqx/awesome-react#react-native)
* [React Native Fundamentals Tutorial by Tyler McGinnis](https://egghead.io/courses/react-native-fundamentals)
* [The Complete React Native and Redux Course (Paid Course)](https://www.udemy.com/the-complete-react-native-and-redux-course/learn/v4/overview)

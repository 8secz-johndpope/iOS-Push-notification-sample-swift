# Flurry Marketing Sample Application (Swift Version)

1) Clone the repo
2) Run 'pod install' in the project folder
3) Replace the sample app's bundle id with your own
4) Replace the app's api key with your own in FlurryMarketingConfig.plist

This app is for iPhone only.

Detailed instructions are written in [Yahoo Developer Network Website](https://developer.yahoo.com/flurry/docs/push/integration/ios/).

This is an Swift version sample app based on Flurry Push service. See [Objective-C version](https://github.com/flurrydev/iOS-Push-notification-sample-ObjC) here. Flurry Push enables external app developers to send targeted messages to re-engage and retain users.<br/>

Detailed instructions are written in [Yahoo Developer Network Website](https://developer.yahoo.com/flurry/docs/push/integration/ios/). Developers can choose either auto integration mode or manual integration mode. There are two AppDelegate in this project. If choosing auto mode, please change value to YES under key "isAuto" in the FlurryMarketingConfig.plist file. If choosing manual mode, change the boolean value to NO instead. In the main function, appropriate AppDelegate will be used based on "isAuto" value. (AppDelegate_Auto.swift -> Auto Use, AppDelegate.swift -> Manual Use). 

Flurry Push Campaign can be created or modified in [Flurry Analytics Portal](https://dev.flurry.com). If this is the first time that you use the Flurry SDK, please see this [link](https://developer.yahoo.com/flurry/docs/integrateflurry/ios/) first to see how to integrate Flurry SDK into your own iOS project. <br/>

In this sample project, there are three views. They are home view (landing page), deeplink view and key-value view. When starting a campaign in the flurry analytics portal, developers can have several options besides basic notification attributes. One of them is deeplinking. Developers can specify a location in the app after a notification being clicked. In this sample app, if the deeplink is set to flurry://marketing/deeplink, the deeplink view will show up. Another option is that developers can pass any key-value pairs as part of notification payload to devices. Key-value view will show all the key-value pairs.

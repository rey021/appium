# appium

Important Appium links
Appium 2.0 overall documentation: https://appium.github.io/appium/docs/en/2.0/

Appium GitHub root: https://github.com/appium

Appium GitHub issues page: https://github.com/appium/appium/issues [Report server defects here]

Appium Inspector: https://github.com/appium/appium-inspector

UiAutomator2 Driver Documentation: https://github.com/appium/appium-uiautomator2-driver

Android (UiAutomator2 Capabilities): https://github.com/appium/appium-uiautomator2-driver#capabilities

XCUITest Driver Documentation:  https://github.com/appium/appium-xcuitest-driver

iOS (XCUITest Capabilities): https://github.com/appium/appium-xcuitest-driver#capabilities

Java Client: https://github.com/appium/java-client [Report client defects here]

Driver Ecosystem: https://appium.github.io/appium/docs/en/2.0/ecosystem/

API Demos app: https://github.com/appium/appium/blob/master/packages/appium/sample-code/apps/ApiDemos-debug.apk

UIKitCatalog app: https://github.com/appium/ios-uicatalog

SauceLabs Demo app: https://github.com/saucelabs/sample-app-mobile

iOS Real Device setup: https://github.com/appium/appium-xcuitest-driver/blob/master/docs/real-device-config.md

Driver Management Commands - Extension CLI: https://appium.github.io/appium/docs/en/2.0/cli/extensions/

Hybrid App Automation: https://appium.io/docs/en/writing-running-appium/web/hybrid/

https://appiumpro.com [For amazing articles from Jonathan Lipps - Appium Project Lead]

Cucumber:

Cucumber JUnit Documentation: https://cucumber.io/docs/cucumber/api/?lang=java#junit

Cucumber TestNG Samples: https://github.com/cucumber/cucumber-jvm/tree/main/cucumber-testng/src/test/java/io/cucumber/testng

Gherkin Syntax and Step Organization: https://cucumber.io/docs/gherkin/

Cucumber Expressions: https://github.com/cucumber/cucumber-expressions#readme


========================
debug the issue at your end.

You can follow these steps:

Look at the Appium server logs for errors. This way you will also understand about internal workings of the Appium server.

In the IDE, look at the exception stack trace. It will show the exact line of code that caused the failure.

Print out the logs strategically in the console. For e.g. if you suspect the driver could be null, then print it out just before the code that threw the exception.

Setup steps might vary. There could be minor variations. In that case, just follow those variations and get the setup done.

Take help from internet (e.g. Google, StackOverFlow, Appium discussion forum, etc.)

Visit the Appium's GitHub issue page (https://github.com/appium/appium/issues) to see if similar issue is already reported.

Go through the Q&A section to check if the issue is already reported. I might have already answered it.

Read through the official documentation: https://appium.io/docs/en/about-appium/intro/

All these steps will help you with enriching your debugging skills. Searching on internet is an art. Master it.

From my experience, I can tell 60% of the issues are mostly coding/setup mistakes or the setup prerequisites are not met.

Many a times, the issues are not even related to Appium. It could be the OS, Android Studio, Emulator, ADB, XCode, Device, IDE and so on. If you follow the above steps, you will be able to narrow down the issue to specific component.

When you are reporting any issue in the Q&A, please share at least the below information:

1. Elaborate what you were trying to do. Write down the steps. For e.g. I got Android studio installed. Created an emulator with name <name>. When I tried to launch the emulator, I'm getting error <error>

2. Elaborate your environment/setup: For e.g. Device platform (Android/iOS), Android studio version, OS, Appium server version, CLI or Desktop and so on....

3. If you are getting an exception, share the complete stack trace

4. Share the Appium server logs

5. Share the code snippet.

6. Screenshots, if applicable.


================

setup
- npm install -g appium@next
- appium driver list
- appium inspector
- java (dont use 16+), 15 is enough
- Android Studio
    - add environment path (C:\Users\user\AppData\Local\Android\Sdk)
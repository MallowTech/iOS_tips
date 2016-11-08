---
title: UIWebView vs WKWebView Performance
tip-number: 03
tip-username: arasu01
tip-username-profile: https://github.com/arasu01
tip-description: `WKWebView` rendering performance is noticeable in WebGL games and something that runs complex JavaScript algorithms which `UIWebView` lacks.

---

####Demo ScreenShot

A screenshot from his demo app running a performance test in the standard Hello World app using the new plugin versus without it is shown below. Notice the difference in FPS (frames per second) and CPU by using this plugin:

![UIWebView vs WKWebView Performance](UIWebView-vs-WKWebView.png "UIWebView vs WKWebView Performance")

####Note:
Here is a test iOS app that can be used to open any website using either UIWebView or WKWebView and you can compare performance, and then decide on whether to use WKWebView or UIWebView:
https://itunes.apple.com/app/id928647773?mt=8&at=10ltWQ
# GWPayment

The official WeChat SDK for iOS apps to access WeChat platform. This is a mirror repository maintained by iOS developers from GWPayment


## Usage

To run the example project:

* Clone the repo, and run `pod install` from the Example directory first.
* Open `GWPayment.xcworkspace`.
* Replace the example target's URL schemes `YOUR_WECAHT_APP_ID` with your WeChat app ID.

Now, let's rock 🚀.


## Requirements

* iOS 8 and later
* Xcode 8 and later


## Installation

BXWeChatSDK is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

``` ruby
pod "GWPayment"
```

Then follow the [instructions](https://open.weixin.qq.com/cgi-bin/showdocument?action=dir_list&t=resource/res_list&verify=1&id=1417694084&token=&lang=zh_CN)
provided by Tencent.

### iOS 9+ Security Issues

Add the following lines to your project's info.plist file so that your app would be allowed to open WeChat.app.

```xml
<key>LSApplicationQueriesSchemes</key>
<array>
<string>wechat</string>
<string>weixin</string>
</array>
```

Or if security is not an issue to your app, use the following lines.

```xml
<key>NSAppTransportSecurity</key>
<dict>
<key>NSAllowsArbitraryLoads</key>
<true/>
</dict>
```


# Pipl Device Intelligence SDK for iOS

Binary distribution of the Pipl Device Intelligence SDK. This repository contains
package manifests only — no source.

**Current version:** `1.2.3` · iOS 16+

## Swift Package Manager

In Xcode: **File → Add Package Dependencies…** and paste:

```
https://github.com/piplcom/device-intelligence-sdk-ios-dist.git
```

Or in a `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/piplcom/device-intelligence-sdk-ios-dist.git", from: "1.2.3")
]
```

## CocoaPods

```ruby
pod 'PiplDeviceIntelligence', :podspec => 'https://raw.githubusercontent.com/piplcom/device-intelligence-sdk-ios-dist/1.2.3/PiplDeviceIntelligence.podspec'
```

## Quick start

```swift
import PiplDeviceIntelligence

_ = try? await DeviceIntelligence.initialize({
    var options = DeviceIntelligenceOptions()
    options.apiKey = "<your-api-key>"
    return options
}())

let token = await DeviceIntelligence.getElephantDevice()
```

Full integration guide: see the Pipl documentation site.

## License

Proprietary. Use of the SDK is governed by the
[Pipl Device SDK Addendum](https://trust.pipl.com/dashboard/device-sdk-addendum).
The full notice ships inside the XCFramework at `PiplDeviceIntelligence.xcframework/LICENSE`.

## Support

engineering@pipl.com

# Pipl Device Intelligence SDK for iOS

Binary distribution of the Pipl Device Intelligence SDK. This repository contains
package manifests only — no source.

**Current version:** `1.2.1-rc.1` · iOS 16+

## Swift Package Manager

In Xcode: **File → Add Package Dependencies…** and paste:

```
https://github.com/piplcom/device-intelligence-sdk-ios-dist.git
```

Or in a `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/piplcom/device-intelligence-sdk-ios-dist.git", from: "1.2.1-rc.1")
]
```

## CocoaPods

```ruby
pod 'PiplDeviceIntelligence', :podspec => 'https://raw.githubusercontent.com/piplcom/device-intelligence-sdk-ios-dist/1.2.1-rc.1/PiplDeviceIntelligence.podspec'
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

## Support

engineering@pipl.com

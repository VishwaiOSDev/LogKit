![LogKit](https://user-images.githubusercontent.com/71421776/182191029-877eeb22-282c-482a-8d89-6118dd150dbb.jpg)

# LogKit
A logger for Xcode

## Motivation
LogKit is designed to be a simple and universal logging library with support for multiple Xcode projects. LogKit will have different types of log level.

## Features

 - [x] Easy to use
 - [x] Highly customizable
 - [x] Provides clean information

## Available Log Levels

 - Verbose
 - Info
 - Debug
 - Warning
 - Error

## đĻ Installation

### Swift Package Manager
The [Swift Package Manager](https://swift.org/package-manager/) is a tool for automating the distribution of Swift code and is integrated into the `swift` compiler.

Add this Swift package in Xcode using its Github repository url. (File > Swift Packages > Add Package Dependency...)

Add this URL https://github.com/VishwaiOSDev/LogKit.git and select **Add Package**.

After adding it select LogKit.

<img width="648" alt="Screenshot 2022-08-01 at 9 14 56 PM" src="https://user-images.githubusercontent.com/71421776/182190544-0dbdd51a-df00-44f2-9064-cd33e44d192b.png">

### đ  How to use

LogKit makes your life easier

Firstly, import the LogKit

```swift
import LogKit
```

For logging,

```swift
Log.verbose("Example of verbose log.")
Log.info("Something went wrong")
Log.debug("Debug mode enabled")
Log.warning("Warning, duplication warning.")
Log.error("Error, data didn't fetch properly.")
```

LogKit will provide clean information for you. Output for above code as follows:

```
[VERBOSE âī¸âī¸] Example of verbose log. â LogKitTests.swift:7 testVerboseLog()
[INFO âšī¸âšī¸] Something went wrong. â LogKitTests.swift:12 testInfoLog()
[DEBUG đđ] Debug mode enabled â LogKitTests.swift:17 testDebugLog()
[WARN â ī¸â ī¸] Warning, duplication warning. â LogKitTests.swift:22 testWarningLog()
[ERROR ââ] Error, data didn't fetch properly. â LogKitTests.swift:27 testErrorLog()
```
# License
LogKit is released under the MIT license.

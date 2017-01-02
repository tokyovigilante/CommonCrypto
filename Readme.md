CommonCrypto
============

This is a raw CommonCrypto module for Swift. This means there is no swift wrapper for the framework. 

This project is Xcode and Swift Package Manager compatiable.

Usage - Xcode 
-------------

Supports iOS, macOS, watchOS and tvOS.

Create a CommonCrypto library project and add the contents of the CCommonCrypto folder to your project. The xcconfig file tells Xcode where to find the correct module map for the relevant target.

Usage: Swift Package Manager 
----------------------------

Supports OS X.

Add the following dependency in your `Package.swift`:

```swift
#if os(OSX)
package.dependencies.append(.Package(url: "https://github.com/tokyovigilante/CommonCrypto.git", majorVersion: 1, minor: 1)
#endif
```
The library is named CCommonCrypto so your Swift wrapper target can be called CommonCrypto as per the Swift PM documentation.
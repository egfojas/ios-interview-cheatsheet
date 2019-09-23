# ios-interview-cheatsheet
A compilation of iOS topics

## iOS Application States
Not running
  - Application haven't been started yet or the app was terminated
  
Inactive
  - Application is in foreground but is not receiving any events. Usually happens when receiving phone calls
  
Active
  - Application is in foreground and is receiving events.
  
Background
  - Application is in background and executing code 
  
Suspended
  - Application is in background and not executing code.

## Objective-C
**Synthesize**
  - used to relate a property to an iVar

**Non-Atomic vs Atomic**
  - Atomic properties guarantee atomic read/write access to an object meaning 
  - Non-Atomic does not

**Method Swizzling**
  - Method swizzling is a runtime process of changing the implementation of a selector. It is done via changing the method invocations by modifying the class's selector-to-function dispatch table mapping

**Associated Properties**
  - An Objective-C runtime capability that allows the addition of custom properties to existing classes in categories.

## Swift
**Structs vs Classes**
  - Structs are value types while Classes are reference types
  - Structs are usually allocated in stack while classes are in heap

**Protocols**

**Enums**

**Generics**

**Associated Types**

**Opaque Types**

**Closures**

## Memory Management
**MRC vs ARC

**strong, weak, unowned*

## Concurrency
**NSThread**

**GCD**

**NSOperation**

## Persistency
**UserDefaults**

**File**

**CoreData**

## User-Interfaces
**Responder Chain**

**ReuseIdentifiers**

## Auto Layout
**Content-Hugging vs Compression-Resistance

**Intrinsic Size**

**Constraints**

## Design Patterns
**MVC**

**MVVM**

**VIPER**

**Singleton**

**Factory**

**Builder**

## Security
**SSL Pinning**

**Keychain**

## Testing
**UnitTesting**

**UITesting**

## Tools
### Xcode
### Instruments
### Dependency Management
1. Cocoapod
2. Carthage
3. Swift Package Manager
### Version Control
1. Git
### Continuous Integration
1. Fastlane
2. Bitrise
### Sniffing
**Wireshark**

## Frameworks
### CoreData
### URLSessionManager
### RxSwift
### SwiftUI
### Combine
### MLKit


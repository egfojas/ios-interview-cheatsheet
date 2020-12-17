# ios-interview-cheatsheet
A compilation of iOS topics

## iOS Application States
* Not running - Application haven't been started yet or the app was terminated
* Inactive - Application is in foreground but is not receiving any events. Usually happens when receiving phone calls
* Active - Application is in foreground and is receiving events.
* Background - Application is in background and executing code 
* Suspended - Application is in background and not executing code.

## Memory Management
### ARC (Automatic Reference Counting)
* used by iOS to track and manage memory usage. To make sure that instances don’t disappear while they are still needed and is done via reference counting. ARC tracks how many properties, constants, and variables are currently referring to each class instance. ARC will not deallocate an instance as long as at least one active reference to that instance still exists. ARC is a compile time process, it automatically pads retain and release calls on compile time
### Weak vs Strong Reference
* Strong - declaring a strong referance to a class instance will increase its reference count of that instance by 1
* Weak - declaring a weak reference to a class instance will not increase its reference count

## Concurrent Programming
### GCD (Grand Central Dispatch)
* GCD is a mechanism that allows concurrent programming via the use of DispatchQueues
⋅⋅⋅Concurrent - executes code blocks concurrently, meaning order of execution and completion of codeblocks are not guaranteed to be the same as order of when they were dispatched
⋅⋅⋅Serial - executes code blocks serially, meaning, order of execution and completion of codeblocks are guarateed to follow the order of when they were dispatched

### OperationQueue
* OperationQueue is a mechanism that allows concurrent programming via the use of Operation and OperationQueues
### Mutex vs Lock vs Semaphores
* mutex -
* lock -
* semaphores - 

## Persistency
### UserDefaults
### Files
### CoreData
### Keychains

## User Intefaces
### Storyboard vs XIB vs NIB
### Autolayout
* formula = c2 = c1 * multiplier + constant
* content-hugging
* compression-resistance
* priorities
### Animations
### View Lifecycle
* loadView
* viewDidLoad
* layoutSubviews
* viewWillLayoutSubviews
* viewWillAppear
* viewDidAppear
* viewWillDisappear
* viewDidDisappear
* deinit

## Design Patterns
* Singleton -  single instance - UserDefaults, UIApplication
* Facade - Easy swap (network, database)
* Factory - builder, use enums, same base class or protocol confirmation
* Delegation - UITableView
* Observer - Rx, Combine, KVO
* Decorator - extension, wrap urself, delegation
* Adapter - use to make old stuff work with new, wrap things around


## App Architectures
* MVC - Model-View-Controller
* MVVM - Model-View-ViewModel
* VIPER - View-Interactpr-Presenter-Entity-Router
* Coordinator
* MVP - Model-View-Presenter

## Security
### SSL Pinning

## SOLID Principles
* Single Responsibility - A class should have one and only one reason to change, meaning that a class should have only one job.
* Open-Close Principle - Objects or entities should be open for extension, but closed for modification.
* Liskov Substitution - Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T
* Interface Segregation - A client should never be forced to implement an interface that it doesn’t use or clients shouldn’t be forced to depend on methods they do not use.
* Dependency Inversion - Entities must depend on abstractions not on concretions. It states that the high level module must not depend on the low level module, but they should depend on abstractions.

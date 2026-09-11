# Swift — Beginner to Advanced

> A complete Swift programming guide from **Beginner → Intermediate → Advanced**, with **English + Khmer explanations** and practical code examples.

![Swift](https://img.shields.io/badge/Swift-6.x-orange?logo=swift)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Advanced-blue)
![Platform](https://img.shields.io/badge/Platform-macOS%20%7C%20Linux%20%7C%20Windows-lightgrey)

---

## 📚 Table of Contents

* [1. What is Swift?](#1-what-is-swift)
* [2. Installing Swift](#2-installing-swift)
* [3. Your First Swift Program](#3-your-first-swift-program)
* [4. Comments](#4-comments)
* [5. Variables and Constants](#5-variables-and-constants)
* [6. Data Types](#6-data-types)
* [7. Type Inference](#7-type-inference)
* [8. Strings](#8-strings)
* [9. Characters](#9-characters)
* [10. Numbers](#10-numbers)
* [11. Boolean](#11-boolean)
* [12. Operators](#12-operators)
* [13. Conditions](#13-conditions)
* [14. Switch](#14-switch)
* [15. Loops](#15-loops)
* [16. Arrays](#16-arrays)
* [17. Sets](#17-sets)
* [18. Dictionaries](#18-dictionaries)
* [19. Functions](#19-functions)
* [20. Function Parameters](#20-function-parameters)
* [21. Return Values](#21-return-values)
* [22. Optionals](#22-optionals)
* [23. Optional Binding](#23-optional-binding)
* [24. Guard](#24-guard)
* [25. Nil-Coalescing](#25-nil-coalescing)
* [26. Structs](#26-structs)
* [27. Properties](#27-properties)
* [28. Methods](#28-methods)
* [29. Initializers](#29-initializers)
* [30. Enums](#30-enums)
* [31. Associated Values](#31-associated-values)
* [32. Classes](#32-classes)
* [33. Struct vs Class](#33-struct-vs-class)
* [34. Inheritance](#34-inheritance)
* [35. Protocols](#35-protocols)
* [36. Extensions](#36-extensions)
* [37. Closures](#37-closures)
* [38. Higher-Order Functions](#38-higher-order-functions)
* [39. Map](#39-map)
* [40. Filter](#40-filter)
* [41. Reduce](#41-reduce)
* [42. Error Handling](#42-error-handling)
* [43. Generics](#43-generics)
* [44. Type Casting](#44-type-casting)
* [45. Access Control](#45-access-control)
* [46. Static Members](#46-static-members)
* [47. Property Wrappers](#47-property-wrappers)
* [48. Result](#48-result)
* [49. Codable](#49-codable)
* [50. JSON Encoding and Decoding](#50-json-encoding-and-decoding)
* [51. Foundation](#51-foundation)
* [52. Date and Time](#52-date-and-time)
* [53. File Handling](#53-file-handling)
* [54. Async/Await](#54-asyncawait)
* [55. Tasks](#55-tasks)
* [56. Actors](#56-actors)
* [57. MainActor](#57-mainactor)
* [58. Sendable](#58-sendable)
* [59. Memory Management](#59-memory-management)
* [60. Weak and Unowned](#60-weak-and-unowned)
* [61. Protocol-Oriented Programming](#61-protocol-oriented-programming)
* [62. Dependency Injection](#62-dependency-injection)
* [63. Generics + Protocols](#63-generics--protocols)
* [64. Swift Package Manager](#64-swift-package-manager)
* [65. Testing](#65-testing)
* [66. SwiftUI Introduction](#66-swiftui-introduction)
* [67. MVVM](#67-mvvm)
* [68. Networking](#68-networking)
* [69. REST API](#69-rest-api)
* [70. Advanced Swift Project](#70-advanced-swift-project)
* [71. Best Practices](#71-best-practices)
* [72. Learning Roadmap](#72-learning-roadmap)

---

# 1. What is Swift?

Swift is a modern programming language created by Apple.

Swift is commonly used for:

* iOS
* iPadOS
* macOS
* watchOS
* tvOS
* visionOS
* Server-side applications
* Command-line tools
* Linux applications
* Windows development
* WebAssembly
* Embedded systems

### English

Swift focuses on:

* Safety
* Performance
* Readability
* Modern syntax
* Type safety
* Memory safety
* Concurrency

### ខ្មែរ

Swift គឺជា programming language ទំនើបដែលបង្កើតឡើងដោយ Apple។

វាត្រូវបានប្រើសម្រាប់៖

* បង្កើត iPhone App
* iPad App
* macOS App
* Apple Watch App
* Apple TV App
* Vision Pro App
* Backend / Server
* Command Line
* Linux
* Windows
* WebAssembly
* Embedded systems

---

# 2. Installing Swift

Swift can be installed on macOS, Linux, and Windows. The official getting-started documentation recommends checking the installation with:

```bash
swift --version
```

Example:

```bash
swift --version
```

You should receive information about the installed Swift toolchain.

### ខ្មែរ

បន្ទាប់ពីដំឡើង Swift រួច អាចពិនិត្យ version ដោយ៖

```bash
swift --version
```

Swift also includes Swift Package Manager (SwiftPM) for managing Swift projects and dependencies.

---

# 3. Your First Swift Program

Create:

```text
main.swift
```

Code:

```swift
print("Hello, Swift!")
```

Run:

```bash
swift main.swift
```

Output:

```text
Hello, Swift!
```

### English

`print()` displays information in the terminal.

### ខ្មែរ

`print()` ប្រើសម្រាប់បង្ហាញព័ត៌មាននៅក្នុង Terminal។

---

# 4. Comments

## Single-line comment

```swift
// This is a comment

print("Hello")
```

## Multi-line comment

```swift
/*
 This is a
 multi-line comment
*/

print("Swift")
```

### ខ្មែរ

Comment គឺជាអត្ថបទសម្រាប់អ្នក developer អាន។ Compiler មិន execute comment ទេ។

---

# 5. Variables and Constants

Swift has:

* `let` → constant
* `var` → variable

## Constant

```swift
let name = "Dara"

print(name)
```

You cannot change it:

```swift
let age = 20

// age = 21
```

## Variable

```swift
var age = 20

age = 21

print(age)
```

### English

Use `let` by default.

Use `var` only when the value needs to change.

### ខ្មែរ

ប្រើ `let` ជាមុនសិន ព្រោះវាមានសុវត្ថិភាពជាង។

ប្រើ `var` នៅពេលតម្លៃត្រូវការផ្លាស់ប្តូរ។

---

# 6. Data Types

Swift has many built-in types.

```swift
let name: String = "Dara"
let age: Int = 25
let price: Double = 19.99
let isActive: Bool = true
let letter: Character = "A"
```

Example:

```swift
let username: String = "admin"
let age: Int = 25
let salary: Double = 1500.50
let isAdmin: Bool = true

print(username)
print(age)
print(salary)
print(isAdmin)
```

### ខ្មែរ

Data Type ប្រាប់ Swift ថា value មួយមានប្រភេទអ្វី។

ឧទាហរណ៍៖

```text
String     → អក្សរ
Int        → ចំនួនគត់
Double     → ចំនួនទសភាគ
Bool       → true / false
Character  → តួអក្សរមួយ
```

---

# 7. Type Inference

Swift can automatically determine the type.

```swift
let name = "Dara"
let age = 25
let price = 10.50
let active = true
```

Swift understands:

```text
name   → String
age    → Int
price  → Double
active → Bool
```

### ខ្មែរ

Swift អាចស្គាល់ Data Type ដោយស្វ័យប្រវត្តិ។

---

# 8. Strings

```swift
let firstName = "Dara"
let lastName = "Kim"

let fullName = firstName + " " + lastName

print(fullName)
```

String interpolation:

```swift
let name = "Dara"
let age = 25

print("My name is \(name)")
print("I am \(age) years old")
```

Output:

```text
My name is Dara
I am 25 years old
```

### Multiline String

```swift
let message = """
Hello
Welcome to Swift
This is a multiline string
"""

print(message)
```

---

# 9. Characters

```swift
let letter: Character = "A"

print(letter)
```

Character is different from String.

```swift
let letter: Character = "A"
let word: String = "Apple"
```

---

# 10. Numbers

## Int

```swift
let age: Int = 25
let score: Int = 100
```

## Double

```swift
let price: Double = 19.99
```

## Float

```swift
let height: Float = 1.75
```

Example:

```swift
let a = 10
let b = 20

let result = a + b

print(result)
```

---

# 11. Boolean

Boolean has two values:

```swift
true
false
```

Example:

```swift
let isLoggedIn = true

if isLoggedIn {
    print("User is logged in")
} else {
    print("User is not logged in")
}
```

### ខ្មែរ

`Bool` មានតែ ២ តម្លៃ៖

```text
true  → ពិត
false → មិនពិត
```

---

# 12. Operators

## Arithmetic

```swift
let a = 10
let b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
```

## Comparison

```swift
let age = 20

print(age == 20)
print(age != 20)
print(age > 18)
print(age < 30)
print(age >= 20)
print(age <= 20)
```

## Logical

```swift
let age = 25
let hasID = true

print(age >= 18 && hasID)
print(age < 18 || hasID)
print(!hasID)
```

---

# 13. Conditions

## if

```swift
let age = 20

if age >= 18 {
    print("Adult")
}
```

## if / else

```swift
let age = 16

if age >= 18 {
    print("Adult")
} else {
    print("Minor")
}
```

## else if

```swift
let score = 85

if score >= 90 {
    print("A")
} else if score >= 80 {
    print("B")
} else if score >= 70 {
    print("C")
} else {
    print("F")
}
```

### ខ្មែរ

`if` ប្រើសម្រាប់សម្រេចចិត្តតាមលក្ខខណ្ឌ។

---

# 14. Switch

```swift
let day = 2

switch day {
case 1:
    print("Monday")

case 2:
    print("Tuesday")

case 3:
    print("Wednesday")

default:
    print("Other day")
}
```

Switch with String:

```swift
let role = "admin"

switch role {
case "admin":
    print("Administrator")

case "user":
    print("Normal User")

case "guest":
    print("Guest")

default:
    print("Unknown role")
}
```

---

# 15. Loops

## For-in

```swift
for number in 1...5 {
    print(number)
}
```

Output:

```text
1
2
3
4
5
```

## Array loop

```swift
let names = ["Dara", "Sok", "Kosal"]

for name in names {
    print(name)
}
```

## While

```swift
var number = 1

while number <= 5 {
    print(number)
    number += 1
}
```

## Repeat-while

```swift
var number = 1

repeat {
    print(number)
    number += 1
} while number <= 5
```

---

# 16. Arrays

Array stores multiple values in order.

```swift
var fruits = ["Apple", "Banana", "Orange"]

print(fruits)
```

Access:

```swift
print(fruits[0])
print(fruits[1])
```

Add:

```swift
fruits.append("Mango")
```

Remove:

```swift
fruits.remove(at: 0)
```

Complete example:

```swift
var fruits = ["Apple", "Banana", "Orange"]

fruits.append("Mango")

for fruit in fruits {
    print(fruit)
}
```

---

# 17. Sets

Set stores unique values.

```swift
var numbers: Set<Int> = [1, 2, 3, 3, 4]

print(numbers)
```

The duplicate `3` is stored only once.

Add:

```swift
numbers.insert(5)
```

Remove:

```swift
numbers.remove(2)
```

Check:

```swift
print(numbers.contains(3))
```

---

# 18. Dictionaries

Dictionary stores key-value pairs.

```swift
var user = [
    "name": "Dara",
    "role": "admin"
]

print(user["name"] ?? "Unknown")
```

Add:

```swift
user["email"] = "dara@example.com"
```

Update:

```swift
user["role"] = "user"
```

Remove:

```swift
user.removeValue(forKey: "role")
```

Complete:

```swift
var user: [String: String] = [
    "name": "Dara",
    "email": "dara@example.com"
]

if let name = user["name"] {
    print(name)
}
```

---

# 19. Functions

A function is reusable code.

```swift
func sayHello() {
    print("Hello Swift")
}

sayHello()
```

Function with parameter:

```swift
func greet(name: String) {
    print("Hello \(name)")
}

greet(name: "Dara")
```

---

# 20. Function Parameters

```swift
func add(a: Int, b: Int) {
    print(a + b)
}

add(a: 10, b: 20)
```

Custom argument labels:

```swift
func greet(person name: String) {
    print("Hello \(name)")
}

greet(person: "Dara")
```

No argument label:

```swift
func greet(_ name: String) {
    print("Hello \(name)")
}

greet("Dara")
```

---

# 21. Return Values

```swift
func add(_ a: Int, _ b: Int) -> Int {
    return a + b
}

let result = add(10, 20)

print(result)
```

Short form:

```swift
func multiply(_ a: Int, _ b: Int) -> Int {
    a * b
}

print(multiply(5, 4))
```

---

# 22. Optionals

Optional means a value may exist or may be `nil`.

```swift
var username: String? = "Dara"

print(username)
```

Optional with nil:

```swift
var email: String? = nil

print(email)
```

### ខ្មែរ

Optional គឺមានន័យថា value អាចមាន ឬមិនមាន។

```text
String
String?
```

`String?` អាចមាន:

```text
"Hello"
```

ឬ

```text
nil
```

---

# 23. Optional Binding

Use `if let`:

```swift
let username: String? = "Dara"

if let name = username {
    print("Username: \(name)")
} else {
    print("No username")
}
```

Using `guard let`:

```swift
func printUsername(_ username: String?) {
    guard let username = username else {
        print("Username is missing")
        return
    }

    print("Username: \(username)")
}

printUsername("Dara")
printUsername(nil)
```

---

# 24. Guard

`guard` is useful when a function should exit early.

```swift
func login(username: String?, password: String?) {
    guard let username = username,
          let password = password else {
        print("Missing credentials")
        return
    }

    print("Login with \(username) / \(password)")
}

login(username: "admin", password: "1234")
login(username: nil, password: "1234")
```

### ខ្មែរ

`guard` ជួយឱ្យ code អានងាយ ដោយដោះស្រាយ error/invalid condition នៅដើម function។

---

# 25. Nil-Coalescing

Use `??` to provide a default value.

```swift
let username: String? = nil

let name = username ?? "Guest"

print(name)
```

Output:

```text
Guest
```

---

# 26. Structs

Struct is a value type.

```swift
struct User {
    let name: String
    let age: Int
}

let user = User(
    name: "Dara",
    age: 25
)

print(user.name)
print(user.age)
```

### ខ្មែរ

`struct` គឺជា type ដែលមាន properties និង methods។

វាមាន value semantics។

---

# 27. Properties

```swift
struct User {
    var name: String
    var age: Int

    var description: String {
        "\(name) is \(age) years old"
    }
}

let user = User(
    name: "Dara",
    age: 25
)

print(user.description)
```

---

# 28. Methods

```swift
struct Counter {
    var value = 0

    mutating func increment() {
        value += 1
    }
}

var counter = Counter()

counter.increment()
counter.increment()

print(counter.value)
```

### Important

A mutating method is required when a value-type instance modifies its own stored properties.

---

# 29. Initializers

```swift
struct User {
    let name: String
    let age: Int

    init(name: String, age: Int) {
        self.name = name
        self.age = age
    }
}

let user = User(
    name: "Dara",
    age: 25
)

print(user.name)
```

---

# 30. Enums

```swift
enum Direction {
    case north
    case south
    case east
    case west
}

let direction = Direction.north

switch direction {
case .north:
    print("Going North")

case .south:
    print("Going South")

case .east:
    print("Going East")

case .west:
    print("Going West")
}
```

---

# 31. Associated Values

Enums can store associated data.

```swift
enum NetworkResult {
    case success(String)
    case failure(String)
}

let result = NetworkResult.success("Data loaded")

switch result {
case .success(let data):
    print("Success: \(data)")

case .failure(let error):
    print("Error: \(error)")
}
```

---

# 32. Classes

Classes are reference types.

```swift
class User {
    var name: String

    init(name: String) {
        self.name = name
    }

    func sayHello() {
        print("Hello \(name)")
    }
}

let user = User(name: "Dara")

user.sayHello()
```

---

# 33. Struct vs Class

| Feature       | Struct           | Class      |
| ------------- | ---------------- | ---------- |
| Type          | Value            | Reference  |
| Inheritance   | No               | Yes        |
| Deinitializer | No               | Yes        |
| Copy behavior | Value copy       | Reference  |
| Identity      | No               | Yes        |
| `mutating`    | Sometimes needed | Not needed |

Example:

```swift
struct CounterStruct {
    var value: Int
}

class CounterClass {
    var value: Int

    init(value: Int) {
        self.value = value
    }
}

var structA = CounterStruct(value: 10)
var structB = structA

structB.value = 20

print(structA.value)
print(structB.value)
```

Output:

```text
10
20
```

Class:

```swift
let classA = CounterClass(value: 10)
let classB = classA

classB.value = 20

print(classA.value)
print(classB.value)
```

Output:

```text
20
20
```

---

# 34. Inheritance

Classes can inherit from other classes.

```swift
class Animal {
    func speak() {
        print("Animal sound")
    }
}

class Dog: Animal {
    override func speak() {
        print("Woof!")
    }
}

let dog = Dog()

dog.speak()
```

---

# 35. Protocols

Protocol defines requirements.

```swift
protocol Vehicle {
    var brand: String { get }

    func drive()
}

struct Car: Vehicle {
    let brand: String

    func drive() {
        print("\(brand) is driving")
    }
}

let car = Car(brand: "Toyota")

car.drive()
```

### ខ្មែរ

Protocol គឺជា contract។

វាកំណត់ថា type មួយត្រូវមាន properties ឬ methods អ្វីខ្លះ។

---

# 36. Extensions

Extensions add functionality to existing types.

```swift
extension String {
    var isLong: Bool {
        count > 10
    }
}

let text = "Hello Swift Programming"

print(text.isLong)
```

Another example:

```swift
extension Int {
    var squared: Int {
        self * self
    }
}

print(5.squared)
```

---

# 37. Closures

Closure is an anonymous function.

```swift
let greet = {
    print("Hello Swift")
}

greet()
```

Closure with parameter:

```swift
let greet = { (name: String) in
    print("Hello \(name)")
}

greet("Dara")
```

Closure with return value:

```swift
let add = { (a: Int, b: Int) -> Int in
    a + b
}

print(add(10, 20))
```

---

# 38. Higher-Order Functions

Swift collections support powerful functional programming methods.

Common methods:

```text
map
filter
reduce
sorted
compactMap
flatMap
forEach
```

---

# 39. Map

`map` transforms every element.

```swift
let numbers = [1, 2, 3, 4, 5]

let doubled = numbers.map {
    $0 * 2
}

print(doubled)
```

Output:

```text
[2, 4, 6, 8, 10]
```

---

# 40. Filter

`filter` keeps elements matching a condition.

```swift
let numbers = [1, 2, 3, 4, 5, 6]

let evenNumbers = numbers.filter {
    $0 % 2 == 0
}

print(evenNumbers)
```

Output:

```text
[2, 4, 6]
```

---

# 41. Reduce

`reduce` combines values into one result.

```swift
let numbers = [1, 2, 3, 4, 5]

let total = numbers.reduce(0) {
    $0 + $1
}

print(total)
```

Output:

```text
15
```

Short form:

```swift
let total = numbers.reduce(0, +)

print(total)
```

---

# 42. Error Handling

Define an error:

```swift
enum LoginError: Error {
    case invalidUsername
    case invalidPassword
}
```

Throw an error:

```swift
func login(
    username: String,
    password: String
) throws {
    guard username == "admin" else {
        throw LoginError.invalidUsername
    }

    guard password == "1234" else {
        throw LoginError.invalidPassword
    }

    print("Login successful")
}
```

Handle the error:

```swift
do {
    try login(
        username: "admin",
        password: "1234"
    )
} catch LoginError.invalidUsername {
    print("Invalid username")
} catch LoginError.invalidPassword {
    print("Invalid password")
} catch {
    print("Unknown error")
}
```

---

# 43. Generics

Generics allow reusable code for different types.

```swift
func swapValues<T>(
    _ a: inout T,
    _ b: inout T
) {
    let temp = a
    a = b
    b = temp
}

var first = 10
var second = 20

swapValues(&first, &second)

print(first)
print(second)
```

The same function works with Strings:

```swift
var first = "Hello"
var second = "Swift"

swapValues(&first, &second)

print(first)
print(second)
```

### ខ្មែរ

Generic អនុញ្ញាតឱ្យ function ឬ type មួយអាចធ្វើការជាមួយ data type ជាច្រើន។

---

# 44. Type Casting

Swift provides:

```text
is
as
as?
as!
```

Example:

```swift
class Animal {}

class Dog: Animal {
    func bark() {
        print("Woof!")
    }
}

let animal: Animal = Dog()

if animal is Dog {
    print("This is a dog")
}
```

Using `as?`:

```swift
if let dog = animal as? Dog {
    dog.bark()
}
```

### Important

Prefer safe casting:

```swift
as?
```

Avoid forced casting unless you are certain:

```swift
as!
```

---

# 45. Access Control

Swift provides access levels such as:

```text
open
public
package
internal
fileprivate
private
```

Example:

```swift
public struct User {
    public let name: String

    public init(name: String) {
        self.name = name
    }
}
```

Private example:

```swift
struct BankAccount {
    private var balance: Double = 0

    mutating func deposit(_ amount: Double) {
        balance += amount
    }

    func getBalance() -> Double {
        balance
    }
}
```

---

# 46. Static Members

`static` creates type-level members.

```swift
struct AppConfig {
    static let appName = "MyApp"
    static let version = "1.0.0"
}

print(AppConfig.appName)
print(AppConfig.version)
```

---

# 47. Property Wrappers

Property wrappers allow reusable property behavior.

```swift
@propertyWrapper
struct Clamped {
    private var value: Int

    let range: ClosedRange<Int>

    init(
        wrappedValue: Int,
        _ range: ClosedRange<Int>
    ) {
        self.range = range
        self.value = min(
            max(wrappedValue, range.lowerBound),
            range.upperBound
        )
    }

    var wrappedValue: Int {
        get {
            value
        }
        set {
            value = min(
                max(newValue, range.lowerBound),
                range.upperBound
            )
        }
    }
}

struct Player {
    @Clamped(0...100)
    var health = 100
}

var player = Player()

player.health = 150

print(player.health)
```

Output:

```text
100
```

---

# 48. Result

`Result` represents either success or failure.

```swift
enum APIError: Error {
    case serverError
}

func fetchData() -> Result<String, APIError> {
    .success("Hello from API")
}

let result = fetchData()

switch result {
case .success(let data):
    print(data)

case .failure(let error):
    print(error)
}
```

---

# 49. Codable

`Codable` is commonly used to encode/decode data.

```swift
struct User: Codable {
    let id: Int
    let name: String
    let email: String
}
```

---

# 50. JSON Encoding and Decoding

Import Foundation:

```swift
import Foundation
```

Encode:

```swift
import Foundation

struct User: Codable {
    let id: Int
    let name: String
    let email: String
}

let user = User(
    id: 1,
    name: "Dara",
    email: "dara@example.com"
)

let encoder = JSONEncoder()

do {
    let data = try encoder.encode(user)

    print(String(data: data, encoding: .utf8)!)
} catch {
    print(error)
}
```

Decode:

```swift
import Foundation

let json = """
{
    "id": 1,
    "name": "Dara",
    "email": "dara@example.com"
}
""".data(using: .utf8)!

do {
    let user = try JSONDecoder().decode(
        User.self,
        from: json
    )

    print(user.name)
    print(user.email)
} catch {
    print(error)
}
```

---

# 51. Foundation

Foundation provides commonly used APIs.

```swift
import Foundation
```

Examples include:

* Date
* Calendar
* URL
* URLRequest
* JSONDecoder
* JSONEncoder
* FileManager
* UUID
* Data

Example:

```swift
import Foundation

let id = UUID()

print(id)
```

---

# 52. Date and Time

```swift
import Foundation

let now = Date()

print(now)
```

Formatting:

```swift
import Foundation

let formatter = DateFormatter()

formatter.dateFormat = "yyyy-MM-dd HH:mm:ss"

let now = Date()

print(formatter.string(from: now))
```

---

# 53. File Handling

```swift
import Foundation

let fileURL = FileManager.default
    .temporaryDirectory
    .appendingPathComponent("hello.txt")

let text = "Hello Swift!"

do {
    try text.write(
        to: fileURL,
        atomically: true,
        encoding: .utf8
    )

    let content = try String(
        contentsOf: fileURL,
        encoding: .utf8
    )

    print(content)
} catch {
    print("File error:", error)
}
```

---

# 54. Async/Await

Swift supports structured concurrency.

```swift
func fetchUsername() async -> String {
    "Dara"
}

func run() async {
    let username = await fetchUsername()

    print(username)
}
```

Run with a Task:

```swift
Task {
    let username = await fetchUsername()

    print(username)
}
```

### ខ្មែរ

`async/await` ជួយសរសេរ asynchronous code ឱ្យអានងាយជាង callback-heavy code។

---

# 55. Tasks

```swift
import Foundation

func fetchData() async -> String {
    try? await Task.sleep(for: .seconds(1))

    return "Data loaded"
}

Task {
    let data = await fetchData()

    print(data)
}
```

---

# 56. Actors

Actors protect mutable state from unsafe concurrent access.

```swift
actor Counter {
    private var value = 0

    func increment() {
        value += 1
    }

    func getValue() -> Int {
        value
    }
}

let counter = Counter()

Task {
    await counter.increment()
    await counter.increment()

    let value = await counter.getValue()

    print(value)
}
```

### ខ្មែរ

`actor` ជួយការពារ shared mutable state នៅពេលមាន concurrent code។

---

# 57. MainActor

`@MainActor` is commonly used for code that must interact with main-thread-isolated state, especially UI-related state.

```swift
import Foundation

@MainActor
final class UserViewModel {
    var username = ""

    func updateUsername() {
        username = "Dara"
    }
}

Task { @MainActor in
    let viewModel = UserViewModel()

    viewModel.updateUsername()

    print(viewModel.username)
}
```

Swift 6.2 also introduced improvements around approachable concurrency and main-actor isolation.

---

# 58. Sendable

`Sendable` indicates that a value can safely be transferred across concurrency domains.

Example:

```swift
struct User: Sendable {
    let id: Int
    let name: String
}
```

This is especially important when writing modern concurrent Swift code.

---

# 59. Memory Management

Swift uses Automatic Reference Counting (ARC) for class instances.

Example:

```swift
class User {
    let name: String

    init(name: String) {
        self.name = name

        print("\(name) initialized")
    }

    deinit {
        print("\(name) deinitialized")
    }
}

var user: User? = User(name: "Dara")

user = nil
```

Output:

```text
Dara initialized
Dara deinitialized
```

---

# 60. Weak and Unowned

## Weak

Weak references do not keep an object alive.

```swift
class Person {
    let name: String

    init(name: String) {
        self.name = name
    }

    deinit {
        print("\(name) deinitialized")
    }
}

class Apartment {
    let number: Int
    weak var tenant: Person?

    init(number: Int) {
        self.number = number
    }
}

var person: Person? = Person(name: "Dara")

let apartment = Apartment(number: 101)

apartment.tenant = person

person = nil
```

## Unowned

Use `unowned` when the referenced object is expected to outlive the reference.

```swift
class Customer {
    let name: String
    var card: CreditCard?

    init(name: String) {
        self.name = name
    }
}

class CreditCard {
    let number: String
    unowned let customer: Customer

    init(number: String, customer: Customer) {
        self.number = number
        self.customer = customer
    }
}
```

Be careful with `unowned`: accessing an unowned reference after its object has been deallocated causes a runtime failure.

---

# 61. Protocol-Oriented Programming

Swift strongly supports protocol-oriented design.

```swift
protocol Printable {
    func printInfo()
}

struct User: Printable {
    let name: String

    func printInfo() {
        print("User: \(name)")
    }
}

struct Product: Printable {
    let name: String

    func printInfo() {
        print("Product: \(name)")
    }
}

let user = User(name: "Dara")
let product = Product(name: "MacBook")

user.printInfo()
product.printInfo()
```

---

# 62. Dependency Injection

Dependency Injection means providing dependencies from outside instead of creating them internally.

```swift
protocol Logger {
    func log(_ message: String)
}

struct ConsoleLogger: Logger {
    func log(_ message: String) {
        print(message)
    }
}

final class UserService {
    private let logger: Logger

    init(logger: Logger) {
        self.logger = logger
    }

    func createUser() {
        logger.log("User created")
    }
}

let logger = ConsoleLogger()

let service = UserService(
    logger: logger
)

service.createUser()
```

### ខ្មែរ

Dependency Injection ធ្វើឱ្យ code:

* Test ងាយ
* Maintain ងាយ
* Replace implementation ងាយ
* Coupling តិច

---

# 63. Generics + Protocols

Advanced Swift often combines protocols and generics.

```swift
protocol IdentifiableItem {
    associatedtype ID: Hashable

    var id: ID { get }
}

struct User: IdentifiableItem {
    let id: Int
    let name: String
}

func printID<T: IdentifiableItem>(
    _ item: T
) {
    print(item.id)
}

let user = User(
    id: 100,
    name: "Dara"
)

printID(user)
```

---

# 64. Swift Package Manager

Swift Package Manager is the standard package-management system for Swift.

Create a package:

```bash
mkdir MyPackage
cd MyPackage

swift package init --type executable
```

Build:

```bash
swift build
```

Run:

```bash
swift run
```

Test:

```bash
swift test
```

Release build:

```bash
swift build -c release
```

A typical package structure:

```text
MyPackage/
├── Package.swift
├── Sources/
│   └── MyPackage/
│       └── main.swift
└── Tests/
    └── MyPackageTests/
        └── MyPackageTests.swift
```

---

# 65. Testing

Modern Swift supports the Swift Testing framework.

Example:

```swift
import Testing

struct CalculatorTests {

    @Test
    func addition() {
        let result = 10 + 20

        #expect(result == 30)
    }
}
```

Another example:

```swift
import Testing

struct UserTests {

    @Test
    func userName() {
        let user = User(
            name: "Dara"
        )

        #expect(user.name == "Dara")
    }
}
```

Run tests:

```bash
swift test
```

---

# 66. SwiftUI Introduction

SwiftUI is Apple's declarative UI framework.

Basic example:

```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        Text("Hello SwiftUI")
            .font(.largeTitle)
            .padding()
    }
}

#Preview {
    ContentView()
}
```

Button:

```swift
import SwiftUI

struct ContentView: View {
    @State private var count = 0

    var body: some View {
        VStack(spacing: 20) {
            Text("Count: \(count)")

            Button("Increment") {
                count += 1
            }
        }
        .padding()
    }
}

#Preview {
    ContentView()
}
```

### ខ្មែរ

SwiftUI ប្រើ declarative programming។

អ្នកប្រាប់ថា UI គួរមានរូបរាងដូចម្តេច ហើយ SwiftUI គ្រប់គ្រង UI update តាម state។

---

# 67. MVVM

MVVM means:

```text
Model
View
ViewModel
```

## Model

```swift
struct User {
    let name: String
    let email: String
}
```

## ViewModel

```swift
import Foundation

@Observable
final class UserViewModel {
    var user: User?

    func loadUser() {
        user = User(
            name: "Dara",
            email: "dara@example.com"
        )
    }
}
```

## View

```swift
import SwiftUI

struct ContentView: View {
    @State private var viewModel = UserViewModel()

    var body: some View {
        VStack {
            if let user = viewModel.user {
                Text(user.name)
                Text(user.email)
            } else {
                Text("No user")
            }

            Button("Load User") {
                viewModel.loadUser()
            }
        }
        .padding()
    }
}
```

> `@Observable` requires the Observation framework in environments where it is used.

---

# 68. Networking

Use `URLSession` for HTTP networking.

```swift
import Foundation

func fetchData() async throws -> Data {
    let url = URL(
        string: "https://example.com"
    )!

    let (data, _) = try await URLSession.shared.data(
        from: url
    )

    return data
}
```

Call it:

```swift
Task {
    do {
        let data = try await fetchData()

        print("Received \(data.count) bytes")
    } catch {
        print("Request failed:", error)
    }
}
```

---

# 69. REST API

Suppose an API returns:

```json
{
    "id": 1,
    "name": "Dara",
    "email": "dara@example.com"
}
```

Model:

```swift
struct User: Codable {
    let id: Int
    let name: String
    let email: String
}
```

API service:

```swift
import Foundation

struct APIService {

    func fetchUser() async throws -> User {
        let url = URL(
            string: "https://example.com/api/user"
        )!

        let (data, response) = try await URLSession.shared.data(
            from: url
        )

        guard let httpResponse = response as? HTTPURLResponse,
              200..<300 ~= httpResponse.statusCode else {
            throw URLError(.badServerResponse)
        }

        return try JSONDecoder().decode(
            User.self,
            from: data
        )
    }
}
```

Usage:

```swift
let api = APIService()

Task {
    do {
        let user = try await api.fetchUser()

        print(user.name)
    } catch {
        print(error)
    }
}
```

---

# 70. Advanced Swift Project

Here is a small architecture combining:

* Protocol
* Dependency Injection
* Codable
* async/await
* URLSession
* Error handling
* Actor
* Generic networking concepts

## Model

```swift
import Foundation

struct User: Codable, Sendable {
    let id: Int
    let name: String
    let email: String
}
```

## API Error

```swift
enum APIError: Error {
    case invalidURL
    case invalidResponse
    case serverError(Int)
}
```

## API Client Protocol

```swift
protocol APIClient {
    func fetchUser() async throws -> User
}
```

## Network Client

```swift
import Foundation

struct NetworkClient: APIClient {

    let baseURL: URL

    func fetchUser() async throws -> User {

        let url = baseURL
            .appendingPathComponent("user")

        let (data, response) =
            try await URLSession.shared.data(
                from: url
            )

        guard let response =
                response as? HTTPURLResponse else {
            throw APIError.invalidResponse
        }

        guard 200..<300 ~= response.statusCode else {
            throw APIError.serverError(
                response.statusCode
            )
        }

        return try JSONDecoder()
            .decode(User.self, from: data)
    }
}
```

## Repository

```swift
protocol UserRepository {
    func getUser() async throws -> User
}
```

Implementation:

```swift
struct DefaultUserRepository: UserRepository {

    private let apiClient: APIClient

    init(apiClient: APIClient) {
        self.apiClient = apiClient
    }

    func getUser() async throws -> User {
        try await apiClient.fetchUser()
    }
}
```

## ViewModel

```swift
import Foundation

@MainActor
final class UserViewModel {

    private let repository: UserRepository

    private(set) var user: User?

    init(repository: UserRepository) {
        self.repository = repository
    }

    func loadUser() async {

        do {
            user = try await repository.getUser()
        } catch {
            print("Failed:", error)
        }
    }
}
```

## Usage

```swift
import Foundation

let client = NetworkClient(
    baseURL: URL(
        string: "https://example.com/api"
    )!
)

let repository = DefaultUserRepository(
    apiClient: client
)

let viewModel = UserViewModel(
    repository: repository
)

Task { @MainActor in
    await viewModel.loadUser()

    if let user = viewModel.user {
        print(user.name)
    }
}
```

---

# 71. Best Practices

## 1. Prefer `let`

Good:

```swift
let name = "Dara"
```

Only use `var` when mutation is required:

```swift
var count = 0

count += 1
```

---

## 2. Avoid force unwrap

Avoid:

```swift
let name = optionalName!
```

Prefer:

```swift
if let name = optionalName {
    print(name)
}
```

or:

```swift
let name = optionalName ?? "Unknown"
```

---

## 3. Prefer guard for early validation

Good:

```swift
func process(user: User?) {
    guard let user else {
        return
    }

    print(user.name)
}
```

---

## 4. Keep functions small

Bad:

```swift
func doEverything() {
    // 500 lines
}
```

Better:

```swift
func validateUser() {}

func saveUser() {}

func sendEmail() {}
```

---

## 5. Use meaningful names

Bad:

```swift
let x = 100
```

Better:

```swift
let maximumRetries = 100
```

Swift's API Design Guidelines emphasize clarity at the point of use and consistent naming.

---

## 6. Prefer value types when appropriate

Use:

```swift
struct
enum
```

when reference identity is not required.

Use:

```swift
class
```

when you need:

* Shared identity
* Reference semantics
* Inheritance
* Lifecycle management

---

## 7. Use protocols for abstraction

```swift
protocol PaymentService {
    func pay(amount: Double)
}
```

Then implementations can change without changing the caller.

---

## 8. Use dependency injection

Prefer:

```swift
init(service: PaymentService)
```

instead of:

```swift
init() {
    service = PaymentServiceImplementation()
}
```

Dependency injection makes testing and architecture easier.

---

## 9. Prefer structured concurrency

Modern Swift code should generally use:

```swift
async
await
Task
actor
Sendable
```

rather than building new asynchronous code around callback pyramids.

Swift 6.2 introduced further improvements aimed at making concurrency easier to adopt while retaining safety.

---

# 72. Learning Roadmap

## 🟢 Level 1 — Beginner

Learn:

```text
1. Variables
2. Constants
3. Data Types
4. Strings
5. Numbers
6. Boolean
7. Operators
8. if / else
9. switch
10. loops
11. arrays
12. sets
13. dictionaries
14. functions
15. optionals
```

Practice project:

### Calculator

```swift
func calculate(
    _ a: Double,
    _ b: Double,
    operation: String
) -> Double? {

    switch operation {
    case "+":
        return a + b

    case "-":
        return a - b

    case "*":
        return a * b

    case "/":
        guard b != 0 else {
            return nil
        }

        return a / b

    default:
        return nil
    }
}

print(calculate(10, 5, operation: "+") ?? 0)
print(calculate(10, 5, operation: "*") ?? 0)
```

---

# 🟡 Level 2 — Intermediate

Learn:

```text
1. Struct
2. Class
3. Enum
4. Protocol
5. Extension
6. Closure
7. map
8. filter
9. reduce
10. Error Handling
11. Generics
12. Codable
13. Foundation
14. File Handling
15. Networking
```

Practice project:

### Todo Model

```swift
struct Todo: Codable, Identifiable {
    let id: UUID
    var title: String
    var isCompleted: Bool
}

var todos = [
    Todo(
        id: UUID(),
        title: "Learn Swift",
        isCompleted: false
    ),
    Todo(
        id: UUID(),
        title: "Build an App",
        isCompleted: false
    )
]

todos[0].isCompleted = true

let completed = todos.filter {
    $0.isCompleted
}

for todo in completed {
    print(todo.title)
}
```

---

# 🔴 Level 3 — Advanced

Learn:

```text
1. Generics
2. Associated Types
3. Opaque Types
4. Existentials
5. Protocol Composition
6. Property Wrappers
7. Result
8. ARC
9. Weak
10. Unowned
11. async/await
12. Task
13. TaskGroup
14. Actor
15. MainActor
16. Sendable
17. Structured Concurrency
18. Swift Package Manager
19. Testing
20. Macros
21. SwiftUI architecture
22. Dependency Injection
23. Modular Architecture
24. Performance
```

---

# 🚀 Recommended Swift Project Structure

For a larger application:

```text
MyApp/
│
├── App/
│   ├── MyApp.swift
│   └── AppEnvironment.swift
│
├── Core/
│   ├── Networking/
│   │   ├── APIClient.swift
│   │   ├── NetworkError.swift
│   │   └── Endpoint.swift
│   │
│   ├── Storage/
│   │   └── StorageService.swift
│   │
│   └── Extensions/
│
├── Features/
│   ├── Authentication/
│   │   ├── Models/
│   │   ├── Views/
│   │   ├── ViewModels/
│   │   └── Services/
│   │
│   ├── Home/
│   │   ├── Models/
│   │   ├── Views/
│   │   └── ViewModels/
│   │
│   └── Profile/
│
├── Shared/
│   ├── Components/
│   ├── Models/
│   └── Utilities/
│
└── Tests/
```

---

# 🧠 Swift Concepts You Should Master

Before calling yourself an advanced Swift developer, understand these deeply:

```text
Value Semantics
Reference Semantics
Optionals
Protocols
Generics
Closures
ARC
Memory Management
Concurrency
Actors
Sendable
async/await
Error Handling
Codable
Swift Package Manager
Testing
SwiftUI
Dependency Injection
Protocol-Oriented Programming
```

---

# 🏗️ Recommended Real-World Architecture

A scalable Swift application can be organized like:

```text
Presentation
     ↓
ViewModel
     ↓
Use Case
     ↓
Repository
     ↓
Service
     ↓
API / Database
```

Example:

```text
SwiftUI View
     ↓
UserViewModel
     ↓
GetUserUseCase
     ↓
UserRepository
     ↓
APIClient
     ↓
REST API
```

This separation makes large projects easier to:

* Test
* Maintain
* Scale
* Debug
* Refactor

---

# 📦 Useful Swift Technologies

## Apple App Development

```text
Swift
SwiftUI
UIKit
Foundation
Combine
Observation
Core Data
SwiftData
CloudKit
MapKit
AVFoundation
StoreKit
UserNotifications
```

## Backend

```text
Swift
Vapor
Hummingbird
SwiftNIO
```

## Tools

```text
Xcode
Swift Package Manager
SwiftPM
Swift Testing
DocC
VS Code
LLDB
```

Swift's official documentation covers the language, standard library, testing, Swift Package Manager, DocC, Apple platforms, Linux, Windows, WebAssembly, and embedded Swift.

---

# 🧪 Final Practice Project

After finishing this guide, build:

## 📱 Task Management App

Features:

```text
Authentication
    ↓
Login
    ↓
Register
    ↓
Home
    ↓
Tasks
    ├── Create
    ├── Update
    ├── Delete
    ├── Complete
    └── Search
    ↓
Profile
    ├── Name
    ├── Email
    └── Logout
```

Recommended architecture:

```text
SwiftUI
   ↓
MVVM
   ↓
Use Cases
   ↓
Repository
   ↓
API Client
   ↓
REST API
```

Recommended concepts:

```text
Swift
SwiftUI
async/await
Actor
Sendable
Codable
URLSession
Dependency Injection
Protocols
Generics
Swift Testing
Swift Package Manager
```

---

# 📚 Official Resources

* Swift official website
* The Swift Programming Language
* Swift Documentation
* Swift Package Manager
* Swift API Design Guidelines
* Swift Testing
* Swift Evolution

The Swift Programming Language is the authoritative language reference, while Swift.org provides getting-started material and documentation for Swift's ecosystem.

---

# 🎯 Final Goal

The recommended progression is:

```text
                    SWIFT
                      │
        ┌─────────────┴─────────────┐
        │                           │
    BEGINNER                    INTERMEDIATE
        │                           │
 Variables                    Struct / Class
 Functions                    Protocol
 Collections                  Enum
 Optionals                    Closure
 Conditions                   Generics
        │                           │
        └─────────────┬─────────────┘
                      │
                   ADVANCED
                      │
              async / await
                  Actors
                 Sendable
                   ARC
               Concurrency
              Architecture
                      │
                      ▼
                PROFESSIONAL
                      │
             ┌────────┴────────┐
             │                 │
          SwiftUI           Backend
             │                 │
            iOS              Vapor
             │                 │
             └────────┬────────┘
                      │
                      ▼
               REAL PROJECTS
```

---

# ⭐ Summary

If you are starting from zero, follow this order:

```text
01. Syntax
02. Variables
03. Types
04. Operators
05. Conditions
06. Loops
07. Collections
08. Functions
09. Optionals
10. Structs
11. Enums
12. Classes
13. Protocols
14. Extensions
15. Closures
16. Error Handling
17. Generics
18. Codable
19. Foundation
20. Networking
21. async/await
22. Actors
23. Sendable
24. SwiftUI
25. MVVM
26. Dependency Injection
27. Testing
28. Swift Package Manager
29. Architecture
30. Real-world projects
```

**The most important rule:**

> Don't just read Swift. Write Swift.

Build small projects, make mistakes, debug them, and gradually move from simple programs to complete applications.

---

## 🇰🇭 សង្ខេបជាភាសាខ្មែរ

បើអ្នកចាប់ផ្តើម Swift ពីសូន្យ សូមរៀនតាមលំដាប់៖

```text
Syntax
↓
Variable / Constant
↓
Data Type
↓
Condition
↓
Loop
↓
Array / Set / Dictionary
↓
Function
↓
Optional
↓
Struct
↓
Enum
↓
Class
↓
Protocol
↓
Extension
↓
Closure
↓
Error Handling
↓
Generic
↓
Codable
↓
Networking
↓
async / await
↓
Actor
↓
SwiftUI
↓
MVVM
↓
Dependency Injection
↓
Testing
↓
Architecture
↓
Real Project
```

គោលដៅចុងក្រោយគឺ **មិនត្រឹមតែចេះ syntax ទេ ប៉ុន្តែអាចបង្កើត project ពិតប្រាកដបាន**។

---

## 📖 Official Documentation

The official Swift documentation is the best reference when you need exact language/API behavior:

[Swift Documentation](https://docs.swift.org/?utm_source=chatgpt.com)

[The Swift Programming Language](https://www.swift.org/documentation/tspl/?utm_source=chatgpt.com)

[Swift Getting Started](https://www.swift.org/getting-started/?utm_source=chatgpt.com)

[Swift API Design Guidelines](https://www.swift.org/documentation/api-design-guidelines/?utm_source=chatgpt.com)

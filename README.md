# 🦅 Swift — Beginner to Advanced

A complete Swift learning guide from **Beginner → Intermediate → Advanced**, with practical examples.

> 🇬🇧 **English:** Swift is a modern, safe, fast programming language developed by Apple for building iOS, macOS, watchOS, tvOS, and server-side applications.
>
> 🇰🇭 **ខ្មែរ:** Swift គឺជាភាសាកម្មវិធីទំនើប ដែលបង្កើតដោយ Apple។ វាត្រូវបានប្រើសម្រាប់បង្កើតកម្មវិធី iOS, macOS, watchOS, tvOS និង Server-side applications។

---

# 📚 Table of Contents

* [1. What is Swift?](#1-what-is-swift)
* [2. Installation](#2-installation)
* [3. Hello World](#3-hello-world)
* [4. Variables and Constants](#4-variables-and-constants)
* [5. Data Types](#5-data-types)
* [6. Type Inference](#6-type-inference)
* [7. Operators](#7-operators)
* [8. Strings](#8-strings)
* [9. Input](#9-input)
* [10. Conditions](#10-conditions)
* [11. Switch](#11-switch)
* [12. Loops](#12-loops)
* [13. Arrays](#13-arrays)
* [14. Sets](#14-sets)
* [15. Dictionaries](#15-dictionaries)
* [16. Functions](#16-functions)
* [17. Function Parameters](#17-function-parameters)
* [18. Return Values](#18-return-values)
* [19. Optionals](#19-optionals)
* [20. Guard](#20-guard)
* [21. Closures](#21-closures)
* [22. Higher-Order Functions](#22-higher-order-functions)
* [23. Structs](#23-structs)
* [24. Classes](#24-classes)
* [25. Properties](#25-properties)
* [26. Methods](#26-methods)
* [27. Initializers](#27-initializers)
* [28. Inheritance](#28-inheritance)
* [29. Protocols](#29-protocols)
* [30. Extensions](#30-extensions)
* [31. Enums](#31-enums)
* [32. Error Handling](#32-error-handling)
* [33. Generics](#33-generics)
* [34. Access Control](#34-access-control)
* [35. Codable](#35-codable)
* [36. JSON](#36-json)
* [37. Async/Await](#37-asyncawait)
* [38. Actors](#38-actors)
* [39. Concurrency](#39-concurrency)
* [40. Property Wrappers](#40-property-wrappers)
* [41. Result Type](#41-result-type)
* [42. Memory Management](#42-memory-management)
* [43. Weak and Unowned](#43-weak-and-unowned)
* [44. Dependency Injection](#44-dependency-injection)
* [45. MVVM](#45-mvvm)
* [46. SwiftUI](#46-swiftui)
* [47. Testing](#47-testing)
* [48. Advanced Project Structure](#48-advanced-project-structure)
* [49. Best Practices](#49-best-practices)
* [50. Learning Roadmap](#50-learning-roadmap)

---

# 1. What is Swift?

## English

Swift is a strongly typed, compiled programming language created by Apple.

It focuses on:

* Safety
* Performance
* Readability
* Modern syntax
* Type safety
* Concurrency

## ខ្មែរ

Swift គឺជា programming language ដែលមាន **strong typing** និងត្រូវបាន compile ទៅជា machine code។

ចំណុចសំខាន់ៗ៖

* សុវត្ថិភាព
* ល្បឿនលឿន
* Code ងាយអាន
* Syntax ទំនើប
* Type Safety
* Concurrency

---

# 2. Installation

## macOS

Install Xcode from the Mac App Store.

Then check Swift:

```bash
swift --version
```

You can also use Swift Package Manager.

```bash
swift package init --type executable
```

Run:

```bash
swift run
```

---

# 3. Hello World

```swift
print("Hello, Swift!")
```

### Output

```text
Hello, Swift!
```

### English

`print()` displays information in the console.

### ខ្មែរ

`print()` ប្រើសម្រាប់បង្ហាញព័ត៌មានទៅកាន់ console។

---

# 4. Variables and Constants

Swift has:

* `let` → constant
* `var` → variable

```swift
let name = "Heng"
var age = 20

print(name)
print(age)

age = 21

print(age)
```

## English

Use `let` when a value should not change.

Use `var` when a value can change.

## ខ្មែរ

ប្រើ `let` នៅពេល value មិនត្រូវការផ្លាស់ប្តូរ។

ប្រើ `var` នៅពេល value អាចផ្លាស់ប្តូរ។

---

# 5. Data Types

Swift supports many built-in types.

```swift
let name: String = "Heng"
let age: Int = 20
let price: Double = 19.99
let isStudent: Bool = true
let grade: Character = "A"

print(name)
print(age)
print(price)
print(isStudent)
print(grade)
```

Common types:

| Type      | Example   |
| --------- | --------- |
| String    | `"Hello"` |
| Int       | `100`     |
| Double    | `10.5`    |
| Float     | `10.5`    |
| Bool      | `true`    |
| Character | `"A"`     |

### ខ្មែរ

Data Type គឺជាប្រភេទទិន្នន័យដែល variable អាចរក្សាទុកបាន។

---

# 6. Type Inference

Swift can automatically determine the type.

```swift
let name = "Heng"
let age = 20
let price = 99.99
let active = true

print(name)
print(age)
print(price)
print(active)
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

# 7. Operators

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
print(age != 18)
print(age > 18)
print(age < 30)
print(age >= 20)
print(age <= 20)
```

## Logical Operators

```swift
let age = 20
let hasID = true

print(age >= 18 && hasID)
print(age >= 18 || hasID)
print(!hasID)
```

### ខ្មែរ

Operators ប្រើសម្រាប់គណនា ប្រៀបធៀប និង logical operations។

---

# 8. Strings

```swift
let firstName = "Heng"
let lastName = "Developer"

let fullName = firstName + " " + lastName

print(fullName)
```

String interpolation:

```swift
let name = "Heng"
let age = 20

print("My name is \(name)")
print("I am \(age) years old")
```

Multiline String:

```swift
let message = """
Hello
Welcome to Swift
Programming is fun!
"""

print(message)
```

### ខ្មែរ

String interpolation ប្រើ `\(value)` ដើម្បីបញ្ចូល variable ទៅក្នុង String។

---

# 9. Input

```swift
print("Enter your name:")

if let name = readLine() {
    print("Hello, \(name)!")
}
```

Input number:

```swift
print("Enter your age:")

if let input = readLine(),
   let age = Int(input) {

    print("Your age is \(age)")
}
```

### ខ្មែរ

`readLine()` ប្រើសម្រាប់ទទួល input ពី user។

ដោយសារ `readLine()` អាច return `nil` យើងត្រូវ handle optional។

---

# 10. Conditions

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

`if` ប្រើសម្រាប់ពិនិត្យលក្ខខណ្ឌ។

---

# 11. Switch

```swift
let day = 3

switch day {
case 1:
    print("Monday")
case 2:
    print("Tuesday")
case 3:
    print("Wednesday")
case 4:
    print("Thursday")
case 5:
    print("Friday")
case 6:
    print("Saturday")
case 7:
    print("Sunday")
default:
    print("Invalid day")
}
```

### Multiple cases

```swift
let character = "a"

switch character {
case "a", "e", "i", "o", "u":
    print("Vowel")
default:
    print("Consonant")
}
```

### ខ្មែរ

`switch` មានប្រយោជន៍សម្រាប់ពិនិត្យ cases ច្រើន។

---

# 12. Loops

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

## Array Loop

```swift
let names = ["Dara", "Sok", "Heng"]

for name in names {
    print(name)
}
```

## While

```swift
var count = 1

while count <= 5 {
    print(count)
    count += 1
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

### ខ្មែរ

Loop ប្រើសម្រាប់ធ្វើ code ដដែលៗច្រើនដង។

---

# 13. Arrays

Array stores multiple values in order.

```swift
var fruits = ["Apple", "Banana", "Orange"]

print(fruits)
print(fruits[0])
```

Add:

```swift
fruits.append("Mango")
```

Remove:

```swift
fruits.remove(at: 1)
```

Loop:

```swift
for fruit in fruits {
    print(fruit)
}
```

Complete example:

```swift
var numbers = [10, 20, 30]

numbers.append(40)
numbers.append(50)

print(numbers)

for number in numbers {
    print(number)
}
```

### ខ្មែរ

Array គឺជា collection ដែលរក្សាទុក values តាមលំដាប់ index។

---

# 14. Sets

Set stores unique values.

```swift
var languages: Set<String> = [
    "Swift",
    "Python",
    "Java"
]

languages.insert("Go")
languages.insert("Swift")

print(languages)
```

`Swift` នឹងមិនត្រូវបានបន្ថែមម្ដងទៀតទេ ព្រោះ Set មិនរក្សាទុក duplicate។

### English

A `Set` is useful when uniqueness is important.

### ខ្មែរ

`Set` មានប្រយោជន៍នៅពេលយើងត្រូវការទិន្នន័យដែលមិនមាន duplicate។

---

# 15. Dictionaries

Dictionary stores key-value pairs.

```swift
var student: [String: Any] = [
    "name": "Heng",
    "age": 20,
    "active": true
]

print(student["name"] ?? "Unknown")
print(student["age"] ?? 0)
```

Typed dictionary:

```swift
var scores: [String: Int] = [
    "Math": 90,
    "English": 85,
    "Physics": 88
]

print(scores["Math"] ?? 0)
```

Loop:

```swift
for (subject, score) in scores {
    print("\(subject): \(score)")
}
```

### ខ្មែរ

Dictionary រក្សាទុក data ជា `key: value`។

---

# 16. Functions

```swift
func greet() {
    print("Hello, Swift!")
}

greet()
```

Function with parameter:

```swift
func greet(name: String) {
    print("Hello, \(name)!")
}

greet(name: "Heng")
```

### ខ្មែរ

Function គឺជា block នៃ code ដែលអាចហៅប្រើឡើងវិញបាន។

---

# 17. Function Parameters

```swift
func add(a: Int, b: Int) {
    print(a + b)
}

add(a: 10, b: 20)
```

Custom argument labels:

```swift
func greet(person name: String) {
    print("Hello, \(name)")
}

greet(person: "Heng")
```

Ignoring argument label:

```swift
func multiply(_ a: Int, _ b: Int) -> Int {
    return a * b
}

let result = multiply(5, 4)

print(result)
```

---

# 18. Return Values

```swift
func add(_ a: Int, _ b: Int) -> Int {
    return a + b
}

let result = add(10, 20)

print(result)
```

Multiple calculations:

```swift
func calculate(a: Double, b: Double) -> (sum: Double, difference: Double) {
    return (
        sum: a + b,
        difference: a - b
    )
}

let result = calculate(a: 20, b: 5)

print(result.sum)
print(result.difference)
```

### ខ្មែរ

Function អាច return value តាមរយៈ `-> ReturnType`។

---

# 19. Optionals

Optionals are one of the most important Swift concepts.

```swift
var name: String? = "Heng"

print(name)
```

An optional can contain:

```text
value
```

or:

```text
nil
```

Example:

```swift
var username: String? = nil

if let username = username {
    print(username)
} else {
    print("No username")
}
```

## Optional Binding

```swift
let input = "25"

if let age = Int(input) {
    print("Age: \(age)")
}
```

## Nil Coalescing

```swift
let username: String? = nil

let name = username ?? "Guest"

print(name)
```

### ខ្មែរ

Optional មានន័យថា value អាចមាន ឬមិនមាន (`nil`)។

Swift ប្រើ Optional ដើម្បីបង្កើន safety និងកាត់បន្ថយ runtime errors។

---

# 20. Guard

`guard` is useful for early exit.

```swift
func printUsername(_ username: String?) {
    guard let username = username else {
        print("Username is missing")
        return
    }

    print("Username: \(username)")
}

printUsername("Heng")
printUsername(nil)
```

### ខ្មែរ

`guard` ប្រើសម្រាប់ពិនិត្យ condition ហើយចាកចេញពី function ប្រសិនបើ condition មិនត្រឹមត្រូវ។

---

# 21. Closures

Closure is an anonymous function.

```swift
let greet = {
    print("Hello!")
}

greet()
```

Closure with parameters:

```swift
let add = { (a: Int, b: Int) -> Int in
    return a + b
}

print(add(10, 20))
```

Short syntax:

```swift
let numbers = [1, 2, 3, 4, 5]

let doubled = numbers.map { number in
    number * 2
}

print(doubled)
```

### ខ្មែរ

Closure គឺជា function ដែលគ្មានឈ្មោះ ហើយអាចរក្សាទុកក្នុង variable ឬផ្ញើទៅ function ផ្សេងបាន។

---

# 22. Higher-Order Functions

Swift collections provide powerful methods.

## map

```swift
let numbers = [1, 2, 3, 4, 5]

let squares = numbers.map {
    $0 * $0
}

print(squares)
```

## filter

```swift
let numbers = [1, 2, 3, 4, 5, 6]

let evenNumbers = numbers.filter {
    $0 % 2 == 0
}

print(evenNumbers)
```

## reduce

```swift
let numbers = [1, 2, 3, 4, 5]

let total = numbers.reduce(0) {
    $0 + $1
}

print(total)
```

## sorted

```swift
let numbers = [5, 2, 8, 1, 4]

let sortedNumbers = numbers.sorted()

print(sortedNumbers)
```

### ខ្មែរ

Higher-order functions អាចធ្វើឱ្យ collection processing មានភាពស្អាត និងខ្លី។

---

# 23. Structs

Struct is a value type.

```swift
struct User {
    let name: String
    var age: Int

    func introduce() {
        print("My name is \(name), age \(age)")
    }
}

let user = User(
    name: "Heng",
    age: 20
)

user.introduce()
```

### Mutating Method

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

### ខ្មែរ

`struct` ប្រើសម្រាប់បង្កើត custom data type និងជា **value type**។

---

# 24. Classes

Class is a reference type.

```swift
class User {
    let name: String
    var age: Int

    init(name: String, age: Int) {
        self.name = name
        self.age = age
    }

    func introduce() {
        print("My name is \(name), age \(age)")
    }
}

let user = User(
    name: "Heng",
    age: 20
)

user.introduce()
```

### Struct vs Class

| Struct                     | Class                            |
| -------------------------- | -------------------------------- |
| Value type                 | Reference type                   |
| No inheritance             | Supports inheritance             |
| Usually preferred for data | Useful for shared identity/state |
| Copy semantics             | Shared reference                 |

---

# 25. Properties

```swift
struct Person {
    var firstName: String
    var lastName: String

    var fullName: String {
        return "\(firstName) \(lastName)"
    }
}

let person = Person(
    firstName: "Heng",
    lastName: "Developer"
)

print(person.fullName)
```

## Property Observer

```swift
class BankAccount {
    var balance: Double = 0 {
        willSet {
            print("New balance: \(newValue)")
        }

        didSet {
            print("Old balance: \(oldValue)")
        }
    }
}

let account = BankAccount()

account.balance = 100
account.balance = 200
```

### ខ្មែរ

Property គឺជា data ដែលភ្ជាប់ជាមួយ type។

---

# 26. Methods

```swift
struct Calculator {

    func add(_ a: Int, _ b: Int) -> Int {
        return a + b
    }

    func subtract(_ a: Int, _ b: Int) -> Int {
        return a - b
    }
}

let calculator = Calculator()

print(calculator.add(10, 5))
print(calculator.subtract(10, 5))
```

---

# 27. Initializers

```swift
struct Product {
    let name: String
    let price: Double

    init(name: String, price: Double) {
        self.name = name
        self.price = price
    }
}

let product = Product(
    name: "Laptop",
    price: 1200
)

print(product.name)
print(product.price)
```

### Failable Initializer

```swift
struct User {
    let name: String

    init?(name: String) {
        guard !name.isEmpty else {
            return nil
        }

        self.name = name
    }
}

if let user = User(name: "Heng") {
    print(user.name)
}
```

---

# 28. Inheritance

Classes can inherit from other classes.

```swift
class Animal {
    let name: String

    init(name: String) {
        self.name = name
    }

    func speak() {
        print("Animal sound")
    }
}

class Dog: Animal {

    override func speak() {
        print("Woof!")
    }
}

let dog = Dog(name: "Buddy")

print(dog.name)
dog.speak()
```

### ខ្មែរ

Inheritance អនុញ្ញាតឱ្យ class មួយទទួល properties និង methods ពី class មួយទៀត។

---

# 29. Protocols

Protocols define requirements.

```swift
protocol Animal {
    var name: String { get }

    func speak()
}

struct Dog: Animal {
    let name: String

    func speak() {
        print("Woof!")
    }
}

struct Cat: Animal {
    let name: String

    func speak() {
        print("Meow!")
    }
}

let dog = Dog(name: "Buddy")
let cat = Cat(name: "Kitty")

dog.speak()
cat.speak()
```

### ខ្មែរ

Protocol គឺជា contract ដែលកំណត់ថា type មួយត្រូវមាន properties ឬ methods អ្វីខ្លះ។

---

# 30. Extensions

Extensions add functionality to an existing type.

```swift
extension String {
    func isLong() -> Bool {
        return count > 10
    }
}

let text = "Hello Swift Programming"

print(text.isLong())
```

Another example:

```swift
extension Int {
    var squared: Int {
        return self * self
    }
}

print(5.squared)
```

### ខ្មែរ

Extension អនុញ្ញាតឱ្យយើងបន្ថែម functionality ទៅ type ដែលមានស្រាប់ ដោយមិនចាំបាច់កែ original definition។

---

# 31. Enums

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

## Enum with Raw Value

```swift
enum HTTPStatus: Int {
    case ok = 200
    case notFound = 404
    case serverError = 500
}

let status = HTTPStatus.ok

print(status.rawValue)
```

## Enum with Associated Values

```swift
enum Result {
    case success(String)
    case failure(String)
}

let result = Result.success("Data loaded")

switch result {
case .success(let message):
    print(message)

case .failure(let error):
    print(error)
}
```

### ខ្មែរ

Enum ប្រើសម្រាប់កំណត់ finite set នៃ values ឬ states។

---

# 32. Error Handling

Swift uses `throw`, `throws`, `do`, `try`, and `catch`.

```swift
enum LoginError: Error {
    case emptyUsername
    case invalidPassword
}

func login(username: String, password: String) throws -> String {

    if username.isEmpty {
        throw LoginError.emptyUsername
    }

    if password.count < 6 {
        throw LoginError.invalidPassword
    }

    return "Login successful"
}

do {
    let message = try login(
        username: "heng",
        password: "123456"
    )

    print(message)

} catch LoginError.emptyUsername {
    print("Username is empty")

} catch LoginError.invalidPassword {
    print("Password is invalid")

} catch {
    print("Unknown error")
}
```

### ខ្មែរ

Error handling ជួយឱ្យ application ដោះស្រាយ errors ដោយមានសុវត្ថិភាព។

---

# 33. Generics

Generics allow reusable code for different types.

```swift
func swapValues<T>(_ a: inout T, _ b: inout T) {
    let temp = a
    a = b
    b = temp
}

var x = 10
var y = 20

swapValues(&x, &y)

print(x)
print(y)
```

The same function works with strings:

```swift
var first = "Hello"
var second = "Swift"

swapValues(&first, &second)

print(first)
print(second)
```

## Generic Type

```swift
struct Box<T> {
    let value: T
}

let intBox = Box(value: 100)
let stringBox = Box(value: "Hello")

print(intBox.value)
print(stringBox.value)
```

### ខ្មែរ

Generics អនុញ្ញាតឱ្យយើងសរសេរ code ដែលអាចប្រើជាមួយ data types ផ្សេងៗបាន។

---

# 34. Access Control

Swift provides:

* `open`
* `public`
* `internal`
* `fileprivate`
* `private`

Example:

```swift
public struct User {

    public let name: String

    private var password: String

    public init(name: String, password: String) {
        self.name = name
        self.password = password
    }

    public func login(password: String) -> Bool {
        return self.password == password
    }
}
```

### ខ្មែរ

Access control ប្រើសម្រាប់គ្រប់គ្រងថា property ឬ method អាចត្រូវបានប្រើពីទីណាខ្លះ។

---

# 35. Codable

`Codable` makes encoding and decoding data easier.

```swift
struct User: Codable {
    let id: Int
    let name: String
    let email: String
}
```

Encode:

```swift
let user = User(
    id: 1,
    name: "Heng",
    email: "heng@example.com"
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
let json = """
{
    "id": 1,
    "name": "Heng",
    "email": "heng@example.com"
}
""".data(using: .utf8)!

let decoder = JSONDecoder()

do {
    let user = try decoder.decode(User.self, from: json)

    print(user.name)
    print(user.email)
} catch {
    print(error)
}
```

### ខ្មែរ

`Codable` ជួយ convert Swift objects ទៅ JSON និង JSON ទៅ Swift objects។

---

# 36. JSON

Example API JSON:

```json
{
    "id": 1,
    "name": "Heng",
    "email": "heng@example.com"
}
```

Swift model:

```swift
struct User: Codable {
    let id: Int
    let name: String
    let email: String
}
```

Decode:

```swift
import Foundation

let json = """
{
    "id": 1,
    "name": "Heng",
    "email": "heng@example.com"
}
""".data(using: .utf8)!

do {
    let user = try JSONDecoder().decode(
        User.self,
        from: json
    )

    print(user.name)

} catch {
    print("Decoding failed:", error)
}
```

---

# 37. Async/Await

Swift supports structured concurrency.

```swift
import Foundation

func fetchUser() async -> String {
    try? await Task.sleep(for: .seconds(1))

    return "Heng"
}

Task {
    let user = await fetchUser()

    print("User:", user)
}
```

### Async throwing function

```swift
import Foundation

enum NetworkError: Error {
    case failed
}

func fetchData() async throws -> String {
    try await Task.sleep(for: .seconds(1))

    return "Data loaded"
}

Task {
    do {
        let data = try await fetchData()

        print(data)

    } catch {
        print("Error:", error)
    }
}
```

### ខ្មែរ

`async/await` ប្រើសម្រាប់ធ្វើ asynchronous operations ដូចជា API requests, database operations និង file operations ដោយមិន block main thread។

---

# 38. Actors

Actors protect mutable state from data races.

```swift
actor BankAccount {
    private var balance: Int = 0

    func deposit(_ amount: Int) {
        balance += amount
    }

    func getBalance() -> Int {
        return balance
    }
}

let account = BankAccount()

Task {
    await account.deposit(100)
    let balance = await account.getBalance()

    print("Balance:", balance)
}
```

### ខ្មែរ

`actor` គឺជា reference type ដែល Swift ប្រើដើម្បីការពារ shared mutable state ក្នុង concurrent code។

---

# 39. Concurrency

Multiple tasks can run concurrently.

```swift
import Foundation

func download(name: String, seconds: UInt64) async {
    try? await Task.sleep(for: .seconds(seconds))

    print("\(name) completed")
}

Task {
    async let first = download(
        name: "File 1",
        seconds: 2
    )

    async let second = download(
        name: "File 2",
        seconds: 1
    )

    _ = await (first, second)

    print("All downloads completed")
}
```

### ខ្មែរ

Concurrency អនុញ្ញាតឱ្យកម្មវិធីធ្វើ operations ជាច្រើនក្នុងពេលតែមួយតាមរបៀបដែលមានសុវត្ថិភាព។

---

# 40. Property Wrappers

Property wrappers allow reusable property behavior.

```swift
@propertyWrapper
struct Clamped {
    private var value: Int
    private let range: ClosedRange<Int>

    init(wrappedValue: Int, _ range: ClosedRange<Int>) {
        self.range = range
        self.value = range.clamp(wrappedValue)
    }

    var wrappedValue: Int {
        get {
            value
        }

        set {
            value = range.clamp(newValue)
        }
    }
}

extension ClosedRange where Bound == Int {
    func clamp(_ value: Int) -> Int {
        min(max(value, lowerBound), upperBound)
    }
}

struct User {
    @Clamped(0...100)
    var score: Int = 0
}

var user = User()

user.score = 150

print(user.score)
```

Output:

```text
100
```

### ខ្មែរ

Property Wrapper អនុញ្ញាតឱ្យយើងបង្កើត reusable logic សម្រាប់ properties។

---

# 41. Result Type

`Result` represents success or failure.

```swift
enum AppError: Error {
    case invalidInput
}

func divide(
    _ a: Double,
    by b: Double
) -> Result<Double, Error> {

    guard b != 0 else {
        return .failure(AppError.invalidInput)
    }

    return .success(a / b)
}

let result = divide(10, by: 2)

switch result {
case .success(let value):
    print("Result:", value)

case .failure(let error):
    print("Error:", error)
}
```

### ខ្មែរ

`Result<Success, Failure>` មានប្រយោជន៍សម្រាប់ API និង service layers ដែលត្រូវ return success ឬ error។

---

# 42. Memory Management

Swift uses Automatic Reference Counting (ARC).

```swift
class Person {
    let name: String

    init(name: String) {
        self.name = name

        print("\(name) created")
    }

    deinit {
        print("\(name) destroyed")
    }
}

var person: Person? = Person(name: "Heng")

person = nil
```

When the last strong reference disappears, the object is deallocated.

### ខ្មែរ

Swift ប្រើ **ARC (Automatic Reference Counting)** ដើម្បីគ្រប់គ្រង memory សម្រាប់ reference types។

---

# 43. Weak and Unowned

## Weak

Use `weak` when a reference should not keep an object alive.

```swift
class Owner {
    let name: String
    var pet: Pet?

    init(name: String) {
        self.name = name
    }
}

class Pet {
    let name: String
    weak var owner: Owner?

    init(name: String) {
        self.name = name
    }
}

var owner: Owner? = Owner(name: "Heng")
var pet: Pet? = Pet(name: "Buddy")

owner?.pet = pet
pet?.owner = owner

owner = nil
pet = nil
```

### ខ្មែរ

`weak` ជួយការពារ retain cycle និងត្រូវបានប្រើជាញឹកញាប់ក្នុង delegate relationships និង object graphs។

---

# 44. Dependency Injection

Dependency Injection makes code easier to test and maintain.

```swift
protocol UserService {
    func getUser() -> String
}

struct RealUserService: UserService {
    func getUser() -> String {
        return "Heng"
    }
}

struct MockUserService: UserService {
    func getUser() -> String {
        return "Test User"
    }
}

class UserViewModel {
    private let service: UserService

    init(service: UserService) {
        self.service = service
    }

    func loadUser() {
        print(service.getUser())
    }
}

let production = UserViewModel(
    service: RealUserService()
)

production.loadUser()

let testing = UserViewModel(
    service: MockUserService()
)

testing.loadUser()
```

### ខ្មែរ

Dependency Injection ធ្វើឱ្យ code:

* ងាយ test
* ងាយ maintain
* ងាយ replace implementation
* កាត់បន្ថយ coupling

---

# 45. MVVM

MVVM means:

```text
Model
View
ViewModel
```

Example:

```swift
import Foundation

struct User {
    let name: String
}

protocol UserService {
    func fetchUser() async -> User
}

struct APIUserService: UserService {

    func fetchUser() async -> User {
        return User(name: "Heng")
    }
}

@MainActor
final class UserViewModel {

    private let service: UserService

    var username: String = ""

    init(service: UserService) {
        self.service = service
    }

    func loadUser() async {
        let user = await service.fetchUser()

        username = user.name
    }
}
```

### Architecture

```text
View
 ↓
ViewModel
 ↓
Service
 ↓
API / Database
```

### ខ្មែរ

MVVM ជួយបែងចែក UI logic និង business logic ដើម្បីធ្វើឱ្យ project ងាយ maintain។

---

# 46. SwiftUI

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
```

## Button

```swift
import SwiftUI

struct ContentView: View {

    @State private var count = 0

    var body: some View {
        VStack(spacing: 20) {

            Text("Count: \(count)")
                .font(.largeTitle)

            Button("Increase") {
                count += 1
            }
        }
        .padding()
    }
}
```

### ខ្មែរ

SwiftUI ប្រើ declarative syntax។

យើងប្រាប់ SwiftUI ថា UI គួរមានអ្វី ហើយ framework គ្រប់គ្រងការប更新 UI។

---

# 47. SwiftUI State

Common property wrappers:

```text
@State
@Binding
@ObservedObject
@StateObject
@EnvironmentObject
@Environment
```

Example:

```swift
import SwiftUI

struct CounterView: View {

    @State private var count = 0

    var body: some View {

        VStack {

            Text("\(count)")
                .font(.largeTitle)

            Button("Add") {
                count += 1
            }
        }
        .padding()
    }
}
```

### ខ្មែរ

`@State` ប្រើសម្រាប់ local UI state ដែល SwiftUI គ្រប់គ្រង។

---

# 48. Testing

Swift supports unit testing with XCTest.

Example:

```swift
import XCTest

final class CalculatorTests: XCTestCase {

    func testAddition() {

        let result = 10 + 20

        XCTAssertEqual(result, 30)
    }

    func testSubtraction() {

        let result = 20 - 10

        XCTAssertEqual(result, 10)
    }
}
```

### ខ្មែរ

Testing ជួយធានាថា code របស់យើងធ្វើការត្រឹមត្រូវ និងការពារ regression។

---

# 49. Advanced Project Structure

A scalable Swift project can use:

```text
MyApp/
├── App/
│   └── MyApp.swift
│
├── Core/
│   ├── Network/
│   ├── Database/
│   ├── Extensions/
│   └── Utilities/
│
├── Models/
│   ├── User.swift
│   └── Product.swift
│
├── Services/
│   ├── UserService.swift
│   └── ProductService.swift
│
├── ViewModels/
│   ├── UserViewModel.swift
│   └── ProductViewModel.swift
│
├── Views/
│   ├── HomeView.swift
│   ├── LoginView.swift
│   └── ProfileView.swift
│
└── Tests/
    └── MyAppTests/
```

### ខ្មែរ

ការរៀបចំ project ឱ្យបានល្អធ្វើឱ្យ codebase ធំៗងាយស្រួល maintain។

---

# 50. Networking

A simple HTTP GET request:

```swift
import Foundation

struct User: Codable {
    let id: Int
    let name: String
    let email: String
}

func fetchUsers() async throws -> [User] {

    let url = URL(
        string: "https://example.com/api/users"
    )!

    let (data, response) = try await URLSession.shared.data(
        from: url
    )

    guard let httpResponse = response as? HTTPURLResponse,
          200..<300 ~= httpResponse.statusCode else {
        throw URLError(.badServerResponse)
    }

    return try JSONDecoder().decode(
        [User].self,
        from: data
    )
}

Task {
    do {
        let users = try await fetchUsers()

        for user in users {
            print(user.name)
        }

    } catch {
        print("Request failed:", error)
    }
}
```

> Replace `https://example.com/api/users` with your real API endpoint.

### ខ្មែរ

`URLSession` ប្រើសម្រាប់ HTTP networking។

Flow:

```text
URL
 ↓
URLSession
 ↓
HTTP Response
 ↓
Data
 ↓
JSONDecoder
 ↓
Swift Model
```

---

# 51. Advanced Generics with Protocols

```swift
protocol IdentifiableEntity {
    associatedtype ID: Hashable

    var id: ID { get }
}

struct Product: IdentifiableEntity {
    let id: Int
    let name: String
}

func findByID<T: IdentifiableEntity>(
    _ items: [T],
    id: T.ID
) -> T? {

    items.first {
        $0.id == id
    }
}

let products = [
    Product(id: 1, name: "Laptop"),
    Product(id: 2, name: "Phone")
]

if let product = findByID(products, id: 2) {
    print(product.name)
}
```

### ខ្មែរ

Advanced generics អាចប្រើ `associatedtype` និង protocol constraints ដើម្បីបង្កើត highly reusable code។

---

# 52. Protocol-Oriented Programming

Swift strongly supports protocol-oriented programming.

```swift
protocol Printable {
    func printInfo()
}

extension Printable {
    func printInfo() {
        print("Default information")
    }
}

struct User: Printable {
    let name: String

    func printInfo() {
        print("User:", name)
    }
}

struct Product: Printable {
    let name: String
}

let user = User(name: "Heng")
let product = Product(name: "Laptop")

user.printInfo()
product.printInfo()
```

### ខ្មែរ

Protocol-oriented programming ជួយឱ្យ code មានភាព flexible និង reusable ដោយផ្អែកលើ behavior ជាង inheritance។

---

# 53. Sendable and Concurrency Safety

For concurrent code, Swift provides `Sendable`.

```swift
struct User: Sendable {
    let id: Int
    let name: String
}

actor UserStore {

    private var users: [User] = []

    func add(_ user: User) {
        users.append(user)
    }

    func allUsers() -> [User] {
        users
    }
}

let store = UserStore()

Task {
    await store.add(
        User(id: 1, name: "Heng")
    )

    let users = await store.allUsers()

    print(users)
}
```

### ខ្មែរ

`Sendable` ជួយបញ្ជាក់ថា value មួយអាចផ្ទេររវាង concurrency domains ដោយសុវត្ថិភាព។

---

# 54. Key Paths

Swift supports key paths for dynamic property access.

```swift
struct User {
    let name: String
    let age: Int
}

let user = User(
    name: "Heng",
    age: 20
)

let nameKeyPath = \User.name

let name = user[keyPath: nameKeyPath]

print(name)
```

### ខ្មែរ

Key Path អនុញ្ញាតឱ្យយើង reference ទៅ property ដោយមិន access ដោយផ្ទាល់។

---

# 55. Custom Operators

Swift allows custom operators.

```swift
struct Vector {
    let x: Int
    let y: Int
}

func + (
    lhs: Vector,
    rhs: Vector
) -> Vector {

    Vector(
        x: lhs.x + rhs.x,
        y: lhs.y + rhs.y
    )
}

let first = Vector(x: 1, y: 2)
let second = Vector(x: 3, y: 4)

let result = first + second

print(result.x)
print(result.y)
```

### ខ្មែរ

Custom operators អាចធ្វើឱ្យ domain-specific code មានភាពងាយអាន ប៉ុន្តែគួរប្រើដោយប្រុងប្រយ័ត្ន។

---

# 56. Result Builder Concept

SwiftUI relies heavily on result-builder syntax.

A simplified custom example:

```swift
@resultBuilder
struct StringBuilder {

    static func buildBlock(
        _ components: String...
    ) -> String {
        components.joined(separator: " ")
    }
}

func createMessage(
    @StringBuilder _ content: () -> String
) -> String {
    content()
}

let message = createMessage {
    "Hello"
    "Swift"
    "Developer"
}

print(message)
```

Output:

```text
Hello Swift Developer
```

### ខ្មែរ

Result Builder ជា Swift feature ដែលអនុញ្ញាតឱ្យបង្កើត declarative syntax ដូចដែលយើងឃើញនៅក្នុង SwiftUI។

---

# 57. Actors + Networking Example

A practical service architecture:

```swift
import Foundation

struct User: Codable, Sendable {
    let id: Int
    let name: String
}

actor UserAPI {

    private let session = URLSession.shared

    func fetchUser() async throws -> User {

        let url = URL(
            string: "https://example.com/api/user"
        )!

        let (data, response) = try await session.data(
            from: url
        )

        guard let response = response as? HTTPURLResponse,
              200..<300 ~= response.statusCode else {
            throw URLError(.badServerResponse)
        }

        return try JSONDecoder().decode(
            User.self,
            from: data
        )
    }
}

let api = UserAPI()

Task {
    do {
        let user = try await api.fetchUser()

        print(user.name)

    } catch {
        print("Error:", error)
    }
}
```

---

# 58. Complete Mini Project

Let's build a simple in-memory User Management application.

```swift
import Foundation

struct User: Identifiable, Codable {
    let id: UUID
    var name: String
    var email: String
}

actor UserRepository {

    private var users: [User] = []

    func create(
        name: String,
        email: String
    ) -> User {

        let user = User(
            id: UUID(),
            name: name,
            email: email
        )

        users.append(user)

        return user
    }

    func getAll() -> [User] {
        users
    }

    func delete(id: UUID) {
        users.removeAll {
            $0.id == id
        }
    }
}

@main
struct Main {

    static func main() async {

        let repository = UserRepository()

        let user = await repository.create(
            name: "Heng",
            email: "heng@example.com"
        )

        print("Created:", user.name)

        let users = await repository.getAll()

        print("Users:")

        for user in users {
            print(
                "\(user.name) - \(user.email)"
            )
        }

        await repository.delete(
            id: user.id
        )

        print(
            "Remaining:",
            await repository.getAll().count
        )
    }
}
```

### Architecture

```text
             ┌──────────────┐
             │     Main     │
             └──────┬───────┘
                    │
                    ▼
          ┌──────────────────┐
          │ UserRepository   │
          │      Actor       │
          └────────┬─────────┘
                   │
                   ▼
             ┌──────────┐
             │   User   │
             │  Model   │
             └──────────┘
```

---

# 59. Swift Package Manager

Create a package:

```bash
mkdir MySwiftApp
cd MySwiftApp

swift package init --type executable
```

Run:

```bash
swift run
```

Build:

```bash
swift build
```

Test:

```bash
swift test
```

Release build:

```bash
swift build -c release
```

### Typical structure

```text
MySwiftApp/
├── Package.swift
├── Sources/
│   └── MySwiftApp/
│       └── main.swift
└── Tests/
    └── MySwiftAppTests/
        └── MySwiftAppTests.swift
```

---

# 60. Swift Best Practices

## 1. Prefer `let`

Good:

```swift
let name = "Heng"
```

Only use `var` when mutation is required.

```swift
var count = 0
count += 1
```

---

## 2. Avoid Force Unwrapping

Avoid:

```swift
let value = optionalValue!
```

Prefer:

```swift
if let value = optionalValue {
    print(value)
}
```

or:

```swift
let value = optionalValue ?? "Default"
```

---

## 3. Use Guard for Early Validation

```swift
func process(username: String?) {

    guard let username else {
        return
    }

    print(username)
}
```

---

## 4. Keep Functions Small

Instead of:

```swift
func doEverything() {
    // 500 lines
}
```

Prefer:

```swift
func validateUser() {
}

func saveUser() {
}

func sendNotification() {
}
```

---

## 5. Prefer Protocols for Abstractions

```swift
protocol UserRepository {
    func getUsers() async throws -> [User]
}
```

This makes testing and dependency injection easier.

---

## 6. Use Meaningful Names

Bad:

```swift
let x = 20
```

Better:

```swift
let userAge = 20
```

---

## 7. Avoid Massive ViewModels

Keep responsibilities separated:

```text
View
 ↓
ViewModel
 ↓
UseCase
 ↓
Repository
 ↓
API / Database
```

---

# 61. Swift Learning Roadmap

## 🟢 Beginner

Learn:

```text
Swift Syntax
    ↓
Variables
    ↓
Constants
    ↓
Data Types
    ↓
Operators
    ↓
Strings
    ↓
Conditions
    ↓
Loops
    ↓
Arrays
    ↓
Sets
    ↓
Dictionaries
    ↓
Functions
```

---

# 🟡 Intermediate

Learn:

```text
Optionals
    ↓
Guard
    ↓
Closures
    ↓
map / filter / reduce
    ↓
Structs
    ↓
Classes
    ↓
Properties
    ↓
Methods
    ↓
Initializers
    ↓
Enums
    ↓
Protocols
    ↓
Extensions
    ↓
Error Handling
```

---

# 🔴 Advanced

Learn:

```text
Generics
    ↓
Protocol-Oriented Programming
    ↓
Memory Management
    ↓
ARC
    ↓
Weak / Unowned
    ↓
Dependency Injection
    ↓
Codable
    ↓
Networking
    ↓
Async / Await
    ↓
Actors
    ↓
Concurrency
    ↓
Sendable
    ↓
Property Wrappers
    ↓
Result Builders
    ↓
Swift Package Manager
    ↓
Testing
    ↓
Architecture
```

---

# 62. iOS Development Roadmap

After learning Swift:

```text
Swift
  ↓
SwiftUI
  ↓
UIKit
  ↓
Foundation
  ↓
Networking
  ↓
JSON / Codable
  ↓
Persistence
  ↓
Concurrency
  ↓
Architecture
  ↓
Testing
  ↓
App Store Deployment
```

---

# 63. Recommended Architecture

For a larger application:

```text
                    ┌───────────────┐
                    │      View     │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │   ViewModel   │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │    UseCase    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │  Repository   │
                    └───────┬───────┘
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
          ┌────────────┐       ┌─────────────┐
          │     API    │       │   Database  │
          └────────────┘       └─────────────┘
```

### ខ្មែរ

Architecture បែបនេះជួយបំបែក responsibility របស់ component នីមួយៗ។

---

# 64. Common Swift Mistakes

## Mistake 1 — Force unwrap

```swift
let name = optionalName!
```

Better:

```swift
guard let name = optionalName else {
    return
}
```

---

## Mistake 2 — Using `var` everywhere

Bad:

```swift
var name = "Heng"
```

if it never changes.

Better:

```swift
let name = "Heng"
```

---

## Mistake 3 — Huge functions

Bad:

```swift
func processEverything() {
    // hundreds of lines
}
```

Better:

```swift
func validate() {
}

func process() {
}

func save() {
}
```

---

## Mistake 4 — Strong reference cycles

Bad architecture can create:

```text
Object A
   ↓
Object B
   ↓
Object A
```

Use `weak` where appropriate.

---

# 65. Useful Swift Commands

Check Swift:

```bash
swift --version
```

Create package:

```bash
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

---

# 66. Final Cheat Sheet

## Variables

```swift
let constant = 10
var variable = 20
```

## Optional

```swift
var name: String? = nil
```

## Function

```swift
func add(_ a: Int, _ b: Int) -> Int {
    a + b
}
```

## Struct

```swift
struct User {
    let name: String
}
```

## Class

```swift
class User {
    let name: String

    init(name: String) {
        self.name = name
    }
}
```

## Protocol

```swift
protocol Animal {
    func speak()
}
```

## Enum

```swift
enum Status {
    case loading
    case success
    case failure
}
```

## Closure

```swift
let add: (Int, Int) -> Int = {
    $0 + $1
}
```

## Generic

```swift
func identity<T>(_ value: T) -> T {
    value
}
```

## Async/Await

```swift
func load() async throws -> String {
    "Data"
}
```

## Actor

```swift
actor Counter {
    var value = 0
}
```

---

# 67. Final Learning Path

If you are starting Swift from zero, follow this order:

```text
01. Syntax
02. Variables
03. Constants
04. Types
05. Operators
06. Strings
07. Conditions
08. Loops
09. Arrays
10. Sets
11. Dictionaries
12. Functions
13. Optionals
14. Guard
15. Closures
16. map/filter/reduce
17. Structs
18. Classes
19. Properties
20. Methods
21. Initializers
22. Enums
23. Protocols
24. Extensions
25. Error Handling
26. Generics
27. Codable
28. JSON
29. Networking
30. Async/Await
31. Actors
32. Concurrency
33. Memory Management
34. Dependency Injection
35. Testing
36. SwiftUI
37. MVVM
38. Architecture
39. Performance
40. Production App
```

---

# 🚀 Practice Projects

After completing the fundamentals, build these projects:

### Beginner

1. Calculator
2. Number Guessing Game
3. Todo List
4. Temperature Converter
5. Student Grade System

### Intermediate

6. Expense Tracker
7. Contact Manager
8. Notes App
9. Weather App
10. Quiz Application

### Advanced

11. REST API Client
12. Authentication App
13. E-Commerce App
14. Chat Application
15. Banking Application
16. Social Media Application

### Professional

17. Clean Architecture App
18. MVVM + REST API
19. Offline-first Application
20. Production iOS Application

---

# 🎯 Goal

By completing this guide, you should understand:

```text
Swift Fundamentals
        ↓
Object-Oriented Programming
        ↓
Protocol-Oriented Programming
        ↓
Generics
        ↓
Error Handling
        ↓
Memory Management
        ↓
Networking
        ↓
Concurrency
        ↓
SwiftUI
        ↓
MVVM
        ↓
Testing
        ↓
Architecture
        ↓
Production Applications
```

---

# ⭐ Summary

Swift is more than just syntax.

To become a strong Swift developer, focus on:

```text
Language Fundamentals
        +
Data Structures
        +
Protocols
        +
Generics
        +
Memory Management
        +
Concurrency
        +
Networking
        +
Testing
        +
Architecture
        +
Real Projects
```

> 🇬🇧 **English:** Don't only read Swift. Write Swift every day, build projects, debug errors, and learn how to design maintainable applications.
>
> 🇰🇭 **ខ្មែរ:** កុំត្រឹមតែអាន Swift។ ត្រូវសរសេរ Swift រាល់ថ្ងៃ បង្កើត Project ពិតៗ រៀន Debug Error និងរៀនរចនា Application ដែលងាយស្រួល Maintain។

---

## 📌 One-Line Swift Philosophy

```text
Write safe code.
Write clear code.
Write maintainable code.
Build real applications.
```

**Happy Coding with Swift! 🦅**

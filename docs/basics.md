## The Basics

[Swift Programming Guide](https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html)

Swift has all the types you expect, including `Int`, `Double`, `Float`, `Bool`, `String`, `Array`, `Set`, and `Dictionary`. Swift also has avanced type such as tuples and `Optionals`.

### Type Safety

Swift is type safe.

### Declaring Variables

```swift
let aConstant = "Let declares constants that can't be changed."
var aVariable = "This variable can be changed."

var var1 = "You can declare", var2 = "multiple variables or constants", var3 = "one one line."
```

### Type Annotations

Type annotations can usually be inferred from context but can be declared when necessary. Follow the variable or constant name with a colon and the type to declare the type.

```swift
var mustContainString: String
var x, y, z: Double
```

### Naming Constants and Variables

Name can contain unicode characters if you want to be cute. Names can't contain whitespace or start with a number. There are some other rules but if you don't get cute with your naming you won't run into them.

You can't redeclare constants and variables, or change one into another.

### Printing Constants and Variable

`print` is a global function. It's signature is `print(_:separator:terminator:)` which will make more sense once you read the [Functions](functions.md) section, but you can probably guess from looking at it. The default terminator is a newline.

```swift
var num = 10
print(num)
```

### String Interpolation

Use a backslash and parens to interpolate a value or the result of an expression into a string.
```swift
let theResult = 32
print(The result of the calculation is \(theResult)."
```

### Comments

C style comments are supported. Unlike C, multiline comments can be nested if you need to comment out code that alreay contains comments.

```swift
// a comment
/* a 
 multiline
 comment
 */
 ```
 
 ### Semicolons
 
 If you want to put multiple statements on one line spearate them with a semicolon.
 
 ### Integers
 
Signed and unsigned integers in 8, 16, 32, and 64 bit varieties are supported but in most cases just use `Int` which will use the current platform's native word size. This aids code consistency and interoperability by avoiding having to convert types when calling other functions that expect and different integer size.
 
#### Int

The integer types are `Int`, `Int8`, `Int16`, `Int32`, and `Int64`. On a 64-bit system the size of an `Int` is the same as `Int64`.

```swift
print(Int64.min)
print(Int64.max)
```

#### UInt

The unsigned integer types are `UInt`, `UInt8`, `UInt16`, `UInt32`, and `UInt64`. On a 64-bit system the size of an `UInt` is the same as `UInt64`.

```swift
print(UInt64.min)
print(UInt64.max)
```

> Int is preferred, even when the values to be stored are known to be nonnegative.

### Floating-Point Numbers

Swift provides `Double` for 64-bit floating point values and `Float` for 32-bit values. `Double` is preferred unless you have a specific need for `Float`.

### Type Safety and Type Inference

Type checks are performed during code compilation. If you don't specify a type, Swift will infer the type from context. For example when you declare a constant or variable with an initial value the value is used to determine the type. Floating point values will be inferred as type `Double`.

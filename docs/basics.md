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


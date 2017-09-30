# Swift Style Guide

The coding style guide for Swift

#### Use immutable by default

Prefer `let`

```swift

let bar = 1

```

Rather than

```swift

var foo = 1

```

Prefer `struct`

```swift

struct Foo { ... }

```

Rather than

```swift

class Foo { ... }

```

#### Mark class as final by default

Prefer

```swift

final class Foo { ... }

```

Rather than

```swift

class Foo { ... }

```

#### Always mark access control explicitly at the front most

Prefer

```swift

internal var bar: Bar

internal override func foo() { ... }

```

Rather than

```swift

var bar: Bar

override internal foo() { ... }

```

#### Using `if else`

Prefer

```swift

if
    let name = json?["name"] as? String,
    let age = json?["age"] as? Int {

}
else if
    let firstName = json?["firstName"] as? String,
    let lastName = json?["lastName"] as? String {

}
else {

}

```

#### Using `guard else`

Prefer

```swift

guard
    let text = textField.text,
    !text.isEmpty
else { return }

```

# References

* [GitHub - Swift Style Guide](https://github.com/github/swift-style-guide)

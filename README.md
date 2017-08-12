# Swift Interview Questions

## A
1. In what contexts may `Self` (with a capital S) be used?

2. What are some of the important differences between plain Swift protocols and those with associated type or self requirements?

3. How would you go about implementing an equivalent function as `valueForKeyPath` but for arbitrary Swift structs?

4. What does the `~=` operator do in Swift and where is it commonly used?

5. What does `@autoclosure` do and why is it useful? Can you give an example?

6. Consider the following:

```swift 
let gvrd = ["Vancouver", "Burnaby", "Surrey", "New Westminster", "Coquitlam", "Langley", "Richmond", "Delta"]
let zone = gvrd[2...4]
``` 
What is `zone[2]`?

## B

1. Why is the `.first` property only available on `Collection` types and not `Sequence` types?

2. Besides `Array`, name as many `Collection` conforming types that you can from the standard library.
	
3. Can a `Collection` be infinite? Can a `Sequence` be infinite?

4. Consider the following. What are the advantages of scenario *A* over scenario *B* if any? What are the runtime or compile-time differences that may occur?

```swift
// Option A: Place the function in the protocol requirements.
protocol Dog {
	func bark()
}

// Option B: Omit the function from the protocol requirements.
protocol Dog {
}

// In both cases, the function is implemented in an extension.
extension Dog {
	func bark() {
		print("woof")
	}
}
```

5. What is type-erasure in Swift. Why is it used? How is it generally implemented?

6. Suppose you are given a simplified version of the standard swift `reduce` function with the following signature:

```swift
	func reduce<C>(input: [E], _ start: C, _ next: (C, E) -> C) -> C {
	}
```

Implement analogous versions of `filter` and `map` based on this function alone.




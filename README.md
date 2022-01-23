# Course Plan
Course plan.

## Week - 1:
1. Installation
2. Introduction to `cargo`
3. Introduction to Rust Syntax:
	- Variables: `let`, `mut`
	- Functions: `fn`
	- `String`, `str`, `format!`, `println!`
	- Arrays: `Vec`, `slice`
	- HashMap (or Dictionary): `HashMap`
	- Ownership, Borrowing
	- Control Flow: `if`, `if let`, `match`
	- Loops: `loop`, `while`, `while let`, `for`, iterators
#### Homeworks:
1. Write `fn hello(name:&str) -> String` will return: "Hello -name-!"
2. Write `fn make_double(num:i32) -> i32` will return: 4 when given 2
3. Write `fn multiply_pi(num:f32) -> f32` will multiply the num with Pi(π) and return the result.
## Week - 2:
1. Introduction to: Enum, Result, Option, Struct, Trait, Macro
#### Homeworks:
1. Write `fn to_letter_grade(num:u8) -> String`
2. Write `fn log(level:LogLevel::Warn, msg:&str) -> String` LogLevel is enum. Prints logs with level tag: `[WARN]: This is warning log.`
3. Write `Person {name:String, age: u8, gender: Gender}` Gender is enum. Implement `Display` trait for `Person`.
## Week - 3:
1. Crates, Tests
	- Crates: `use`, `mod`, `pub mod`, create your own crate
	- Usage of an example crate: [serde](https://docs.rs/serde/latest/serde/index.html)
	- Writing Tests
#### Homeworks:
1. Print `Point{x:1, y:1}` struct like `{"x":1, "y":1}` with serde.
2. Write 3 tests for Homework - 2
3. Write the jsonified  of `Point` struct to a `test.json` file
## Week - 4:
1. Closure
2. Iterator
	- `filter`
	- `map`
	- `zip`
	- `nth`, `count`
	- `enumerate`
	- Fibonacci example with Iterator trait
3. Generics
#### Homeworks:
1. Filter even numbers on a list
2. Multiply all numbers with 2 on a list
## Week - 5:
1. Thread, Mutex, Atomic, Channel
	- Fearless Concurrency
	- thread
	- thread w/ mutex
	- thread w/ atomic
	- thread w/ channel
#### Homeworks:
1. Calculate nth prime number with 5 threads.
## Week - 6:
1. Introduction to asynchronous programming:
	- `async-std`. `async`, `Future`
	- Example: async TCP server
#### Homeworks:
1. Write tcp echo server with `async-std`

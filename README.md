
# Course Plan
The course plan for introduction to Rust.

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
1. Write `fn hello(name:&str) -> String`
   - will return: "Hello -name-!"
2. Write `fn make_it_double(num:i32) -> i32`
   - will return: 4 when given 2
3. Write `fn multiply_pi(num:f32) -> f32`
   - will multiply the num with Pi(π) and return the result.
## Week - 2:
1. Introduction to: 
   - Enum
   - Result
   - Option
   - Struct
   - Traits
   - Macro
#### Homeworks:
1. Write `fn to_letter_grade(num:u8) -> String`
   - will return "AA" for 100, "BA" for 89 etc.
2. Write `fn log(level:LogLevel, msg:&str) -> String` 
   - LogLevel is an enum. Prints logs with level tag: `[WARN]: This is warning log.`
3. Write `Person {name:String, age: u8, gender: Gender}` 
   - Gender is an enum. Also implement `Display` trait for `Person` with format: `{name}({age})` ex: `Emin(24)`.
4. Write `display!(Person, "{}({})", name, gender)`
    - This macro will implement Display trait for Person with format you provide.
## Week - 3:
1. Crates, Tests
	- Crates: `use`, `mod`, `pub mod`, create your own crate
	- Usage of an example crate: [serde](https://docs.rs/serde/latest/serde/index.html)
	- Writing Tests
#### Homeworks:
1. Make `Person { name:String, age:u8, gender:Gender::Male }` struct transformable to JSON string with serde & serde_json crate:
	- Example: `{"name":"Emin","age":24,"gender":"Male"}`
2. Write 3 test cases for first task.
3. Write jsonified output of the `Person` struct to `person.json` file.
	- Writing to a file examples: https://doc.rust-lang.org/std/fs/struct.File.html
## Week - 4:
1. Closure
2. Iterator
	- `filter`
	- `map`
	- `nth`
	- `count`
	- `enumerate`
	- Fibonacci series with Iterator trait
3. Generics
4. Lifetimes
#### Homeworks:
1. Filter even numbers on a list
2. Multiply all numbers with 2 on a list
3. Implement an iterator which implements this algorithm: `f(n) = f(n-1) * f(n-2)` and `n > 0`
## Week - 5:
1. Thread, Mutex, Atomic, Channel
	- Fearless Concurrency
	- thread
	- thread w/ mutex
	- thread w/ atomic
	- thread w/ channel
#### Homeworks:
1. Calculate nth prime number with threads.
	- Find every given prime number on an array `&[u32]` with spawning a thread for each of it, and send the result with `std::sync::mpsc::Sender`.
## Week - 6:
1. Introduction to asynchronous programming:
	- `async-std`. `async`, `Future`
	- Example: async TCP server
#### Homeworks:
1. Write tcp chat server with `async-std`
	- Send each message to other connections.
	- Use Arc<Mutex<>> to share "user list" between the tasks.
	- Use 22222 port to make us test it easily.

---

# Social/Cultural Topics
Outline of the educational topics on blockchains, decentralization, and DEVxDAO.

## Week - 1: Introduction to Blockchains, Decentralization, and DEVxDAO
- What is a blockchain?
- Decentralization vs. Centralization
- Overview of DEVxDAO and its role in promoting decentralized projects

## Week - 2: Consensus Mechanisms in Blockchain
- Proof of Work (PoW)
- Proof of Stake (PoS)
- Delegated Proof of Stake (DPoS) and other consensus mechanisms

## Week - 3: Smart Contracts and Decentralized Applications (dApps)
- What are smart contracts?
- How do smart contracts work?
- Examples of dApps and their use cases

## Week - 4: Introduction to Decentralized Autonomous Organizations (DAOs)
- What is a DAO?
- How does a DAO work?
- Examples of DAOs and their impact on decentralized ecosystems

## Week - 5: Blockchain Interoperability and Cross-Chain Solutions
- What is blockchain interoperability?
- Why is interoperability important for the blockchain ecosystem?
- Cross-chain solutions and examples

## Week - 6: The Future of Decentralization and the Role of DEVxDAO
- Emerging trends in decentralization
- The role of DEVxDAO in supporting innovative projects
- How to get involved in the DEVxDAO community and contribute to decentralized projects

---

# Introduction to Blockchain Development Workshop
Outline for the 2-week hands-on part of intro to blockchain development.

## Week 1: Introduction to Blockchain Development and Basic Setup

### Session 1:

1.  Introduction
    -   Goals of the hands-on blockchain development course
    -   Overview of the Casper blockchain platform
    - Communication mediums and where to get help
2.  Getting Started
    -   Setting up the development environment
    -   Installing necessary tools and dependencies
3.  Create And Fund An Account
    -   Creating a new account on the Casper Network
    -   Funding the account with tokens

### Session 2:

1.  Session Code
    - What is session code?
    - Using session code for multisig setup
2.  Session Code Testing
    - How to test session code
3.  A Smart Contract Example
    -   Writing a simple smart contract using Rust
    -   Understanding the components of a smart contract

## Week 2: Developing, Testing, and Interacting with Smart Contracts

### Session 1:

1.  Testing Your Smart Contract
    -   Setting up a test environment for the smart contract
    -   Writing tests and verifying the contract's functionality
2.  Installing Contracts On Casper
    -   Deploying the smart contract to the Casper Network
    -   Tracking the deployment status
3.  Verify An Installed Contract
    -   Verifying the successful installation of the smart contract
    -   Checking the contract's state on the network

### Session 2:

1.  Upgrading A Contract
    -   Modifying the smart contract
    -   Deploying the upgraded version to the Casper Network
2.  Interacting with Smart Contracts
    -   Call installed contracts by hash, name, and using Wasm
    -   Calling contracts with session arguments
    -   Calling versioned contracts by package hash and package name
3.  What's Next?
    -   Exploring more advanced topics in blockchain development
    -   Opportunities for further learning and development within the Casper ecosystem

## References
- [Casper Developer Portal](https://developer.casper.network/)
- [Casper Network Documentation](https://docs.casper.network/)
- [Casper Association Video Series: Writing On-Chain Code](https://www.youtube.com/playlist?list=PL8oWxbJ-csEqi5FP87EJZViE2aLz6X1Mj)

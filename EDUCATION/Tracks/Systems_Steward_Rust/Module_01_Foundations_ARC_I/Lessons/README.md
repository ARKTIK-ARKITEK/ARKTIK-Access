# Module ACE-SSR-101: ARC-I - Lessons

This directory contains the individual lesson plans for **ACE-SSR-101: ARC-I - Systems Welding & Foundational Structures**, the foundational module of the A.C.E. Systems Steward - Rust Track.

Please refer back to the main [Module README](../README.md) for the overall objectives, prerequisites, execution gate criteria, and context of this module within the track.

## Learning Methodology

Each lesson within this module follows the A.C.E. 4-Phase learning cycle:

1.  **Foundation & Principles:** Understanding the core concepts (Rust features, ARKTIK values).
2.  **Application & Practice:** Hands-on exercises, coding labs, and examples.
3.  **Execution & Demonstration:** Specific tasks to demonstrate understanding and skill application. Committing work via Git is integral.
4.  **Integration & Reflection:** Connecting the lesson back to the larger goals and reflecting on learning.

It is crucial to complete the lessons **sequentially**, ensuring mastery of each concept and successful execution of required tasks before proceeding to the next. Engage actively in code reviews and discussions.

## Lesson Sequence

*(Note: Lesson codes L<Unit>.<LessonInUnit> indicate alignment with the 6 Units of ARC-I)*

*   **Unit 1: Preparation & Precision**
    *   **[L1.1 - Digital Stewardship Setup](./L1_1_Digital_Stewardship_Setup.md):** Setting up GitHub repository, Codespace, and initializing a Rust project using Cargo. Understanding the foundational workflow and ARKTIK values in development setup.
    *   **[L1.2 - Rust Syntax, Variables & Foundational Types](./L1_2_Rust_Syntax_Variables_Types.md):** (Placeholder) Core Rust syntax, declaring variables (`let`, mutability), scalar types (integers, floats, bool, char), compound types (tuples, arrays).
    *   **[L1.3 - Control Flow](./L1_3_Control_Flow.md):** (Placeholder) Using `if`/`else`, `loop`, `while`, and `for` expressions to control program execution.
    *   **[L1.4 - Functions & Cargo Basics](./L1_4_Functions_Cargo_Basics.md):** (Placeholder) Defining and calling functions, parameters, return values, expressions vs. statements, further exploration of `Cargo.toml` and basic `cargo` commands (`check`, `build`).

*   **Unit 2: Ownership & Data Integrity**
    *   **[L2.1 - Ownership Principles & Moves](./L2_1_Ownership_Moves.md):** (Placeholder) Understanding Rust's core ownership rules, stack vs. heap concepts, variable scope, move semantics, `Copy` trait basics.
    *   **[L2.2 - References & Borrowing](./L2_2_References_Borrowing.md):** (Placeholder) Using shared (`&`) and mutable (`&mut`) references, borrowing rules, preventing dangling references.
    *   **[L2.3 - Basic Lifetimes](./L2_3_Basic_Lifetimes.md):** (Placeholder) Introduction to lifetime annotations ('a) and their purpose in ensuring reference validity, focusing on common function signatures.
    *   **[L2.4 - Structs & Methods](./L2_4_Structs_Methods.md):** (Placeholder) Defining custom data structures with `struct`, implementing methods using `impl` blocks.
    *   **[L2.5 - Enums & Pattern Matching](./L2_5_Enums_Match.md):** (Placeholder) Defining enumerations (`enum`), using the powerful `match` expression for exhaustive pattern matching, `Option<T>` enum.

*   **Unit 3: Testing, Modularity & Resilience**
    *   **[L3.1 - Collections: Vectors & Strings](./L3_1_Collections_Vec_String.md):** (Placeholder) Working with dynamic arrays (`Vec<T>`) and growable strings (`String`), common methods, ownership considerations.
    *   **[L3.2 - Collections: Hash Maps](./L3_2_Collections_HashMap.md):** (Placeholder) Using `HashMap<K, V>` for key-value storage, ownership, common methods.
    *   **[L3.3 - Robust Error Handling](./L3_3_Error_Handling_Result.md):** (Placeholder) Using the `Result<T, E>` enum for recoverable errors, the `?` operator for propagation, `panic!` for unrecoverable errors.
    *   **[L3.4 - Automated Testing](./L3_4_Automated_Testing.md):** (Placeholder) Writing unit tests (`#[test]`), integration tests, using `assert!` macros, principles of Test-Driven Development (TDD).
    *   **[L3.5 - Modules & Project Structure](./L3_5_Modules_Structure.md):** (Placeholder) Organizing code using Rust's module system (`mod`, `use`), visibility rules (public/private), basic workspace concepts.

*   **Unit 4: Concurrency & Systems Interaction**
    *   **[L4.1 - Threads & Synchronization](./L4_1_Threads_Sync.md):** (Placeholder) Spawning threads (`std::thread`), basic synchronization using `Mutex` and `Arc` for shared state.
    *   **[L4.2 - Message Passing with Channels](./L4_2_Channels_Message_Passing.md):** (Placeholder) Using `std::sync::mpsc` channels for safe communication between threads.
    *   **[L4.3 - Asynchronous Programming Introduction](./L4_3_Async_Await_Intro.md):** (Placeholder) Understanding `async`/`await` syntax, Futures, basics of using an async runtime (e.g., Tokio).
    *   **[L4.4 - Filesystem Operations](./L4_4_Filesystem_Operations.md):** (Placeholder) Reading from and writing to files using `std::fs`, handling I/O errors.
    *   **[L4.5 - Data Serialization with Serde](./L4_5_Serialization_Serde.md):** (Placeholder) Using the Serde library to serialize/deserialize Rust data structures to/from formats like JSON.

*   **Unit 5: Networking & Data Persistence Basics**
    *   **[L5.1 - Web Framework Introduction](./L5_1_Web_Framework_Intro.md):** (Placeholder) Overview of a chosen Rust web framework (e.g., Axum/Actix), setting up a basic server.
    *   **[L5.2 - Building Basic API Endpoints](./L5_2_Building_Basic_Endpoints.md):** (Placeholder) Creating simple GET/POST request handlers, extracting data, returning responses (e.g., JSON via Serde).
    *   **[L5.3 - Making HTTP Requests](./L5_3_Making_HTTP_Requests.md):** (Placeholder) Using a crate like `reqwest` to interact with external APIs from Rust.
    *   **[L5.4 - Database Interaction Introduction (SQLx)](./L5_4_Database_Intro_SQLx.md):** (Placeholder) Connecting to a database (e.g., SQLite/Postgres) using SQLx, executing basic queries (SELECT, INSERT, UPDATE), handling results asynchronously.

*   **Unit 6: Capstone Integration & Polish**
    *   **[L6.1 - Capstone Project Planning & Integration](./L6_1_Capstone_Planning.md):** (Placeholder) Defining scope, architecture, and task breakdown for the module's capstone project using Asana/planning tools. Integrating concepts from previous units.
    *   **[L6.2 - Advanced Testing & Code Polish](./L6_2_Adv_Testing_Polish.md):** (Placeholder) Implementing more thorough testing, refactoring for clarity/idiomatic Rust, performance considerations (basic).
    *   **[L6.3 - Documentation & Presentation Prep](./L6_3_Documentation_Presentation.md):** (Placeholder) Writing comprehensive READMEs and `cargo doc` comments, preparing for the final project review/defense.

---

Proceed through these lessons diligently, focusing on executing the tasks precisely and reflecting on the underlying principles. Your consistent effort here builds the foundation for becoming an effective Systems Steward.

**ARKTIK-ARKITEK**

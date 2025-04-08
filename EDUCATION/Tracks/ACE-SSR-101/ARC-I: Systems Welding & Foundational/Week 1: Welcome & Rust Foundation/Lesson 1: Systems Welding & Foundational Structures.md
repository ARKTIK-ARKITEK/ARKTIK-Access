# **Module:** ACE-SSR-101: ARC-I: Systems Welding & Foundational Structures
**Week:** 1 of 12
**Lesson:** 1 of (e.g., 2-3 for the week)
**Estimated Duration:** 2 - 2.5 Hours (Adjustable based on Q&A and setup speed)

**Lesson Title:** Ignition: Welcome to Rust, ARKTIK & Your Dev Environment

**Topics Covered:**

1.  Course Introduction & A.C.E. Context
2.  Introduction to Rust: Why use it?
3.  Tooling Setup: GitHub & GitHub Codespaces
4.  First Program: "Hello, World!" via Cargo
5.  Cargo Basics: `new`, `run`, `build`
6.  Introduction to Version Control: First GitHub Commit
7.  *Light Introduction:* Variables (`let`, `mut`), basic types (integers, bools)
8.  *Light Introduction:* Comments
9.  *Fun Element Setup:* Starting the Console Guessing Game (Input/Output focus)

**Learning Objectives:** By the end of this lesson, students will be able to:

1.  Articulate the basic goals of the A.C.E. framework and this course.
2.  Explain the purpose of using GitHub and GitHub Codespaces for this course.
3.  Successfully launch and navigate a GitHub Codespace environment.
4.  Verify Rust and Cargo installation within Codespaces.
5.  Use `cargo new` to create a new Rust project.
6.  Understand the basic structure of a Cargo project (`Cargo.toml`, `src/main.rs`).
7.  Write and run a simple "Hello, World!" program using `cargo run`.
8.  Differentiate between `cargo run` and `cargo build`.
9.  Write basic comments in Rust code.
10. Declare a simple variable using `let`.
11. Perform their first Git commit and push to their GitHub repository from Codespaces.
12. Use basic Rust I/O (`std::io`) to read user input from the console.

**Materials & Prerequisites:**

*   Reliable Internet Connection
*   Web Browser (Chrome, Firefox, Edge recommended for Codespaces)
*   A GitHub Account (Must be created *before* the lesson)
*   Access link to the course's main GitHub Repository
*   (Optional but Recommended) VS Code Desktop installed (for potentially connecting Codespace locally later)

**A.C.E. Principles Integration:**

*   **Learn by Doing:** Immediate hands-on setup and coding from the first lesson. The core of the lesson is active execution.
*   **Mastery Through Execution:** The first execution steps (running code, committing) establish the pattern for the course.
*   **Accessible Pathways:** Using GitHub Codespaces removes local setup hurdles, making the starting point accessible regardless of the student's local machine setup (as long as they have a browser).
*   **Ethical Leadership (Implied):** Starting with version control promotes transparency and accountability in coding practices ("Lead by Example").

**Lesson Flow:**

**(1) Introduction & Context (15-20 mins)**

*   **Welcome:** Official welcome to ACE-SSR-101.
*   **ARKTIK & A.C.E. Overview:**
    *   Briefly introduce ARKTIK's mission.
    *   Explain the A.C.E. framework's vision (Execution-based, Faith-driven, Practical Mastery, Self-sufficiency).
    *   Mention the Motto: "Learn by Doing. Master by Serving. Lead by Example." - explain how this course embodies it.
*   **Course Roadmap:** Briefly show the 12-week overview, highlight the Capstone project as the goal.
*   **Why Rust?:** Briefly touch upon its strengths (performance, safety, concurrency) and relevance to "Systems Welding".
*   **Tooling Introduction:** Explain *why* GitHub (collaboration, portfolio) and *why* Codespaces (standardized environment, accessibility, cloud power).

**(2) Setup: GitHub & Codespaces (30-40 mins)**

*   **Action:** Guide students to the course GitHub repository.
*   **Action:** Demonstrate/guide students on how to create/launch their Codespace instance for the repository.
    *   *Troubleshooting:* Allow time for potential login issues or first-time Codespace setup delays.
*   **Guided Tour:** Once Codespace loads:
    *   Identify the main areas: Editor, File Explorer, Terminal, Ports tab (mention briefly).
    *   Open the Terminal.
*   **Action:** Verify installations:
    *   Run `rustc --version`
    *   Run `cargo --version`
    *   Run `git --version`
    *   Confirm expected versions appear.

**(3) "Hello, ARKTIK!" & Cargo Basics (25-35 mins)**

*   **Concept:** Explain that `cargo` is Rust's build tool and package manager.
*   **Action (in Terminal):**
    *   Navigate to a suitable directory within the Codespace (e.g., create a `projects` directory: `mkdir projects && cd projects`).
    *   Create the first project: `cargo new hello_arktik`
    *   Navigate into the project: `cd hello_arktik`
*   **Guided Tour:**
    *   Open the `hello_arktik` folder in the File Explorer.
    *   Show `Cargo.toml`: Explain its role (metadata, dependencies - briefly).
    *   Show `src/main.rs`: Explain `fn main()` as the entry point, `println!` as a macro for printing.
*   **Action (Editing):**
    *   Modify `src/main.rs` to print "Hello, ARKTIK!" or a similar welcome message.
    *   Add a comment: `// This is my first Rust program!`
*   **Action (Running):**
    *   Run `cargo build`: Explain it compiles the code (show the `target/debug` directory).
    *   Run `cargo run`: Explain it compiles *and* runs the executable. Output should appear in the terminal.

**(4) Variables & GitHub Commit (20-25 mins)**

*   **Concept:** Introduce `let` to declare variables. Introduce `mut` for mutability. Show basic type annotation (e.g., `let message: &str = "Hello";`). Keep it simple (focus on `let` and maybe `i32`, `bool`).
*   **Action (Editing):** Modify `main.rs` slightly to use a variable (e.g., `let greeting = "Hello"; println!("{}, ARKTIK!", greeting);`). Run `cargo run` again.
*   **Concept:** Introduce Git very briefly - purpose is to save snapshots of your code.
*   **Action (Git Workflow):**
    *   `git status` (Show untracked/modified files).
    *   `git add .` (Stage all changes in the current directory).
    *   `git commit -m "W1L1: Initial Hello ARKTIK program"` (Commit changes with a descriptive message).
    *   `git push` (Push the commit to the GitHub repository associated with the Codespace).
    *   Verify on GitHub.com that the code appears. *This is a critical execution step.*

**(5) Fun Element: Guessing Game Setup (20-30 mins)**

*   **Concept:** Introduce the classic guessing game. Explain the goal: computer picks a number, user guesses, computer gives hints. Today, we'll just set it up and read input.
*   **Action (Terminal):**
    *   Navigate back to the main `projects` directory: `cd ..`
    *   Create a new project: `cargo new guessing_game`
    *   Navigate into it: `cd guessing_game`
*   **Action (Editing `src/main.rs`):**
    *   Add `use std::io;` at the top (explain it imports the Input/Output library).
    *   Inside `main`, add `println!("Guess the number!");`
    *   Add `println!("Please input your guess.");`
    *   Declare a mutable variable to store the guess: `let mut guess = String::new();` (Explain `String::new()` creates an empty string).
    *   Use `io::stdin().read_line(&mut guess)` to read input.
        *   Briefly explain `.expect("Failed to read line");` for basic error handling for now.
    *   Print the user's input back: `println!("You guessed: {}", guess);`
*   **Action (Running):**
    *   `cargo run`.
    *   Test typing input and seeing it echoed back.

**(6) Wrap-up & Next Steps (5-10 mins)**

*   **Recap:** Quickly review what was accomplished: Setup Codespaces, ran first Rust program, used Cargo, committed to GitHub, started the guessing game structure.
*   **Preview:** Mention next lesson will cover types/variables/functions in more detail, control flow (`if`, loops), and making the guessing game actually compare numbers.
*   **Assignment/Check:** Ensure everyone has successfully pushed their `hello_arktik` project to GitHub. Encourage exploring the Rust documentation linked in the course materials.
*   **Q&A:** Final chance for questions.

---

This lesson plan focuses on getting students' environments set up and achieving immediate, tangible results ("Hello World", first commit, basic I/O) to build confidence and momentum, directly reflecting the "Learn by Doing" principle.

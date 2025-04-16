# A.C.E. Foundational Git Workflow Principles

## Why Version Control (Git) is Essential in A.C.E.

Within the ARKTIK Curriculum for Education (A.C.E.), **Git** is not just a tool; it is a fundamental practice embodying several core values. We use Git rigorously for version control because it enables:

*   **Accountability & Transparency:** Creates a verifiable history of *who* changed *what*, *when*, and *why* (via commit messages). Every contribution is tracked.
*   **Stewardship & Resilience:** Protects work by providing backups (remote repository on GitHub) and the ability to easily revert to previous stable states if errors are introduced. It helps steward the health of our codebases and projects.
*   **Collaboration:** Provides the essential framework for multiple individuals to work on the same project concurrently without overwriting each other's work unsafely.
*   **Precision & Craftsmanship:** Encourages breaking work down into logical, testable units (commits) and demands clear communication through commit messages.
*   **Quality Assurance:** Facilitates code review processes (via Pull Requests) before changes are merged into main branches, upholding quality standards.

Mastering this foundational workflow is crucial for effective execution in nearly all A.C.E. technical and project-based tracks.

## Core Git Concepts (Simplified)

*   **Repository (Repo):** A project folder whose contents and history are tracked by Git. It exists locally on your machine/Codespace and remotely on a server (like GitHub).
*   **Commit:** A snapshot of your project's changes at a specific point in time, saved with a descriptive message explaining the changes made. Commits form the project's history.
*   **Branch:** An independent line of development within a repository. The `main` (or `master`) branch typically holds the stable, approved version of the project. New features, fixes, or experiments are developed on separate branches.
*   **Remote:** A shared repository hosted on a server (e.g., GitHub), allowing collaboration and backup.
*   **Push:** Uploading your local commits from your current branch to the remote repository.
*   **Pull:** Downloading changes from the remote repository to your local branch.
*   **Merge:** Combining changes from one branch into another (e.g., merging a completed feature branch back into `main`).

## The Basic ARKTIK Workflow Cycle (Feature Branching)

While specific projects may have more advanced strategies, the fundamental cycle for contributing code or significant documentation changes within A.C.E. generally follows these steps:

1.  **Ensure `main` is Updated:** Start with the latest stable version (`git checkout main`, then `git pull origin main`).
2.  **Create a Feature Branch:** Create a new branch specifically for your task/feature. Use a descriptive name.
    ```bash
    git checkout -b your-feature-or-fix-name
    ```
3.  **Execute Your Work:** Make your code changes, write documentation, create assets, etc., on this new branch. Test your changes locally.
4.  **Stage Changes:** Select the changes you want to include in your next commit.
    ```bash
    git add .  # Stages all changes in the current directory
    # OR
    git add path/to/specific/file.rs # Stage only a specific file
    ```
5.  **Commit Changes:** Save a snapshot of your staged changes with a clear, descriptive message. **Commit message quality reflects Integrity and aids Transparency.** ARKTIK encourages using the **Conventional Commits** format (e.g., `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`).
    ```bash
    git commit -m "feat: Implement basic user authentication function"
    # Or, for a more detailed message:
    # git commit (this opens your editor)
    ```
6.  **Push Branch:** Upload your new branch and its commits to the remote repository (GitHub).
    ```bash
    git push origin your-feature-or-fix-name
    ```
7.  **Code Review / Pull Request (Conceptual):** For collaborative projects or contributions to core ARKTIK repositories, the next step is typically opening a **Pull Request (PR)** on GitHub. This requests that your changes be reviewed by mentors or peers before being merged into the `main` branch, ensuring quality and alignment (Accountability, Craftsmanship). *(Detailed PR procedures are covered within specific tracks/projects).*

## Best Practices Emphasized in A.C.E.

*   **Commit Frequently:** Make small, logical commits often. Each commit should represent a single, complete unit of work. This makes history easier to understand and enables easier rollbacks if needed.
*   **Write Meaningful Commit Messages:** The message is crucial context. Explain *what* the change does and *why* it was made. Follow the Conventional Commits format for consistency.
*   **Pull Regularly:** If collaborating, pull changes from the remote `main` branch frequently into your feature branch (`git pull origin main`) to stay updated and address conflicts early.
*   **Test Before Committing:** Ensure your changes work as expected *before* committing them.

## Tools

*   **Git Command Line Interface (CLI):** The fundamental tool, expected proficiency is developed.
*   **GitHub:** The primary platform for hosting ARKTIK's remote repositories, collaboration, and code review (Pull Requests).
*   **Integrated Tools:** Git integration within IDEs like VS Code (used in Codespaces) provides a visual interface that aids the CLI workflow.

## Further Learning

This document covers the foundational workflow principles. Mastering Git involves understanding many more advanced concepts (merging strategies, conflict resolution, rebasing, tagging, etc.).

**Enrolled A.C.E. participants will receive more detailed guidance, practice exercises, and potentially specific workflow protocols for different project types via the internal ARKTIK Learning Platform or within their specific Track materials.** Online resources like the official Git documentation (`git-scm.com`), GitHub Docs, and numerous tutorials are also valuable references.

---
**ARKTIK-ARKITEK**

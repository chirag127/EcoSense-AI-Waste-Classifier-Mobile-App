# Contributing to EcoSnap-AI-Waste-Classification-Mobile-App

## 1. The Apex Standard: A Culture of Engineering Excellence

Thank you for your interest in contributing to EcoSnap. This project operates under a mandate of **Zero-Defect, High-Velocity, Future-Proof** engineering. We adhere to standards equivalent to those at top-tier technology firms. Contributions that do not meet this bar will be rejected. This document is the single source of truth for the contribution process.

By participating, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md).

## 2. The Contribution Gauntlet: A Step-by-Step Protocol

All contributions, without exception, must follow this workflow. Bypassing this process will result in an immediate closure of the Pull Request.

### Step 0: Issue-Driven Development

All work must originate from an existing issue. **No issue, no code.**

1.  **Search:** First, search the [existing issues](https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/issues) to prevent duplication.
2.  **Create:** If no relevant issue exists, [create one using the appropriate template](https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/issues/new/choose). Provide a comprehensive description of the bug or feature proposal.
3.  **Assign:** Wait for a maintainer to triage the issue and assign it to you. Do not begin work until you are assigned.

### Step 1: Local Environment Setup

- **Prerequisites:** Node.js (LTS), Yarn, Expo CLI, and Git.
- **Fork & Clone:** Fork the repository, then clone your fork locally.

bash
# 1. Clone your forked repository
git clone https://github.com/<YOUR_USERNAME>/EcoSnap-AI-Waste-Classification-Mobile-App.git
cd EcoSnap-AI-Waste-Classification-Mobile-App

# 2. Add the original repository as an upstream remote
git remote add upstream https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App.git

# 3. Install dependencies using Yarn (preferred)
yarn install

# 4. Run the development server
npx expo start


### Step 2: Branching and Committing

- **Branching:** Create a new branch from an up-to-date `main` branch. Use the naming convention `type/issue-id/short-description`.

bash
# Sync your main branch with upstream
git fetch upstream
git checkout main
git merge upstream/main

# Create your feature branch
git checkout -b feature/117/add-image-cropping


- **Committing:** We enforce **Conventional Commits**. Your commit messages are part of the codebase and must be clear, concise, and structured.
  - **Format:** `<type>(<scope>): <subject>` (e.g., `feat(camera): implement zoom functionality` or `fix(auth): resolve token refresh loop`).
  - **Types:** `feat`, `fix`, `build`, `chore`, `ci`, `docs`, `perf`, `refactor`, `revert`, `style`, `test`.

### Step 3: Code Quality and Verification

- **Linting & Formatting:** The project uses TypeScript, ESLint, and Prettier to enforce a strict and consistent coding style. Your code must be free of linting errors.

bash
# Run the linter
yarn lint

# Automatically format code
yarn format


- **Testing:** All new features must be accompanied by unit tests. All bug fixes must include a regression test. Code coverage must not decrease.

bash
# Run all tests
yarn test


## 3. Pull Request Submission

Once your changes are complete, tested, and linted, you may open a Pull Request against the `main` branch of the upstream repository.

1.  **Use the Template:** Fill out the [Pull Request Template](./PULL_REQUEST_TEMPLATE.md) completely. Provide a detailed summary of changes and link the issue it resolves using `Closes #117`.
2.  **Pass CI Checks:** The PR will trigger a series of automated checks via GitHub Actions. All checks must pass. A failing build is an automatic rejection criteria.
3.  **Code Review:** A maintainer will review your submission. Be prepared to address feedback and make changes. We value constructive, ego-free technical discussions.
4.  **Merge:** Once approved and all checks are green, your PR will be squashed and merged by a maintainer.

## 4. Architectural Principles

To ensure your contribution aligns with the project's long-term vision, adhere to these architectural principles:

- **TypeScript (Strict Mode):** Type safety is non-negotiable.
- **Feature-Sliced Design (FSD):** Organize code by features (e.g., `authentication`, `classification`, `history`) for maximum scalability and maintainability.
- **DRY (Don't Repeat Yourself):** Abstract and reuse logic where appropriate.
- **SOLID:** Follow SOLID principles for robust and testable object-oriented design.

## 5. Reporting Security Vulnerabilities

Do not create a public issue for security vulnerabilities. Refer to our [Security Policy](./SECURITY.md) for the proper disclosure procedure.

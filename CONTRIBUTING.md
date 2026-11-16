# Contributing to Eaupti

Welcome to the Eaupti project! To keep our monorepo clean and ensure a smooth collaboration for the team, please follow these simple guidelines when contributing code.

## 0. Local Setup

Before writing any code, set up your local environment with our required runtimes and quality tools.

### 0.1. Core Runtimes

Make sure you have the following installed on your machine:

* **Node.js & npm** (v20+ LTS recommended): [Official Node.js Downloads](https://nodejs.org/)
* **Python** (v3.10+ recommended): [Official Python Downloads](https://www.python.org/downloads/)

### 0.2. Frontend Tooling (Biome & TypeScript)

From the root of the repository, install the Node dependencies (this automatically installs **Biome** and **TypeScript** from `package.json`) as a dev dependency:

```bash
npm i
```

*(Docs: [Biome Documentation](https://biomejs.dev/guides/getting-started/) | [TypeScript Documentation](https://www.typescriptlang.org/download/))*

### 0.3. Backend & Git Hook Tooling (Ruff & Pre-commit)

Install **Ruff** (Python linter/formatter) and **pre-commit** (automated Git hook runner) globally using `pip`:

```bash
pip install ruff pre-commit
```

*(Docs: [Ruff Documentation](https://docs.astral.sh/ruff/installation/) | [Pre-commit Documentation](https://pre-commit.com/#install))*

### 0.4. Activate Git Hooks

Once everything is installed, run our setup script from the root directory to bind the automated checks to your local Git workflow:

```bash
npm run setup
```

## 1. Branching Strategy

We use a simplified Feature Branch Workflow. 

* **`main`**: This is our single protected branch. It contains stable, review-approved code. **Never commit directly to `main`.**
* **Working Branches**: All new work must be done in temporary sub-branches created from `main`. Name your branches using the following prefixes:
  * `feat/...` (for new features, e.g., `feat/auth-setup`)
  * `fix/...` (for bug fixes, e.g., `fix/typo-in-readme`)
  * `chore/...` (for tooling, config, or maintenance, e.g., `chore/add-biome`)
  * `docs/...` (for documentation updates)

## 2. Development Workflow

1. **Sync your local repository:** Always pull the latest changes from `main` before starting new work.
2. **Create a new branch:** Checkout a new working branch using the naming rules above.
3. **Write code & Commit:** Make your changes. Ensure you run our automated linters (Biome for Frontend, Ruff for Backend) before committing.
4. **Open a Pull Request (PR):** Push your branch to GitHub and open a PR targeting the `main` branch.
5. **Review & Merge:** Once your code is finalized and passes any required reviews, it will be merged into `main`.

## 3. General Rules

* **Quality over Speed:** Ensure your code passes all local checks before opening a PR.
* **Keep PRs Focused:** Try to address one specific feature or bug per Pull Request.
* **Communicate:** If you are blocked or unsure about an architecture decision, ask the team before writing a massive amount of code.

*(Note: These guidelines will be expanded as the project architecture evolve.)*
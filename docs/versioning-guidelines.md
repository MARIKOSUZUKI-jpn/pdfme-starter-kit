# Version Control and Branching Guidelines

This document defines how version control is managed for this project using Git and GitHub.  
The goals are:

- Keep the `main` branch stable and deployable
- Make development work traceable and reversible
- Prepare the project for collaboration and open-source contribution
- Provide a clear release history using tags and semantic versioning

---

## 1. Tools

- **Version Control**: Git
- **Remote Hosting**: GitHub
- **Default Branch**: `main`
- **Connection Method**: SSH

---

## 2. Branching Strategy

This project uses a simple branching model inspired by **GitHub Flow**.

### 2.1 Branch Types

- `main`  
  - Always stable and deployable  
  - Contains only tested and approved code  
  - Used for releases and tagged versions

- `feature/*`  
  - Used for new features, enhancements, or refactors  
  - Created from `main`, merged back into `main` when done  
  - Example:
    - `feature/pdf-preview`
    - `feature/multi-language-support`
    - `feature/ui-theme-switcher`

- `fix/*` (optional)  
  - Used for non-critical bug fixes  
  - Example:
    - `fix/pdf-layout-alignment`
    - `fix/typo-in-readme`

- `hotfix/*` (optional, for production issues)  
  - Used for urgent issues affecting production  
  - Example:
    - `hotfix/pdf-generation-crash`

### 2.2 Branch Naming Conventions

- Use lowercase letters and hyphens (`-`) for readability
- Prefix with type:
  - `feature/`
  - `fix/`
  - `hotfix/`
  - `docs/` for documentation changes

**Examples:**

- `feature/pdf-template-library`
- `feature/react-frontend-setup`
- `docs/update-architecture-doc`
- `fix/table-rendering-bug`

---

## 3. Commit Message Guidelines

Each commit should be:

- Small and focused on a single logical change
- Described with a short, clear message

### 3.1 Commit Message Format

Recommended format:

```text
<type>: <short description>

[optional longer description]

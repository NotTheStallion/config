# Git Config & Hooks Setup

This repository contains configuration files and Git hooks to streamline your development workflow.

## Structure

- `git_hooks/`
  - `commit-msg`: Hook to modify or validate commit messages.
  - `pre-commit`: Hook to run tasks before a commit (e.g., linting, formatting).
- `.bash_aliases`: Useful shell aliases for convenience.
- `.gitconfig`: Git configuration file with custom aliases and settings.

## Installation

1. Copy the following files to your **home directory**:
   - `.bash_aliases`
   - `.gitconfig`

Example:
```bash
cp .bash_aliases ~/.bash_aliases
cp .gitconfig ~/.gitconfig
```

2. Leave the git_hooks/ directory as-is, or link its contents into your project’s .git/hooks/ directory.

Example:
```bash
ln -s /path/to/this/repo/git_hooks/commit-msg /your/project/.git/hooks/commit-msg
ln -s /path/to/this/repo/git_hooks/pre-commit /your/project/.git/hooks/pre-commit
```

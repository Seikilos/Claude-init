# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

TODO: Update this when you have enough information

## Coding-Guidelines

Apply the following coding guidelines. If you decide to deviate from them, explain why.

- Use clean code principles
  - Single Responsibility Principle -> Structure the code so that a logical unit (class, method) has one responsibility
  - Comments -> Document the WHY, not WHAT has been done
  - DRY -> Do not copy paste code. Especially strings or numbers that occur multiple times *MUST* be extracted
  - IOSP -> Integration Operation Seperation Principle -> A good function/method should either has only branches which call functions/method or operation code without any branches to make the code easy to understand

## Unit-Test-Guidelines

- **NEVER** test implementation details

## ⚠️ CRITICAL WORKFLOW RULES ⚠️

### **🚨 NODE.JS PROJECT REQUIREMENTS - ABSOLUTE PRIORITY 🚨**
- 🔴 **MANDATORY**: NEVER use npm in Node.js projects
- 🔴 **MANDATORY**: ALWAYS use pnpm instead of npm for ALL Node.js operations
- 🔴 **MANDATORY**: When creating a new Node.js project, NEVER use npm - only pnpm
- 🔴 **MANDATORY**: Create a `.npmrc` file with these exact settings:
  ```
  ignore-scripts=true
  minimum-release-age=30d
  ```
- 🔴 This means:
  - ❌ NO `npm install`
  - ❌ NO `npm run`
  - ❌ NO `npm init`
  - ❌ NO `npm ci`
  - ✅ USE `pnpm install`
  - ✅ USE `pnpm run`
  - ✅ USE `pnpm init`
  - ✅ USE `pnpm` for all package management

### **COMMIT AFTER EVERY COMPLETED TASK**
- 🔴 **MANDATORY**: Use git to commit changes immediately after finishing each logical unit of work
- 🔴 **NEVER** accumulate multiple completed tasks without committing
- 🔴 **ALWAYS** write clear, descriptive commit messages following the project style
- 🔴 Check that tests pass before committing

### When to Commit - Explicit Checkpoints
Commit **immediately after** completing any of these:
- ✅ Adding a new class, interface, or file
- ✅ Implementing a new feature or method
- ✅ Refactoring existing code
- ✅ Fixing a bug
- ✅ Updating configuration files (*.csproj, Directory.Build.props, etc.)
- ✅ Moving or reorganizing files/directories
- ✅ Updating documentation
- ✅ All tests passing after making changes



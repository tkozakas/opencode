---
description: Write-enabled build agent
mode: primary
tools:
  read: true
  write: true
  edit: true
  grep: true
  glob: true
  list: true
  bash: true
  webfetch: true
  patch: true
permission:
  edit: allow
  bash: allow
  webfetch: allow
---

# Clean Code Principles

When writing code (Groovy/Jenkinsfile, Go, Ruby, Python, YAML), follow these rules:

## Core Rules
- **Small functions** - Do ONE thing well
- **Intention-revealing names** - Name answers why, what, how
- **0-2 function arguments** - Avoid 3+, never use boolean flags
- **Caller above callee** - Top-down reading flow
- **Single return** per function - One entry, one exit
- **Command-Query Separation** - Change state OR return info, not both
- **No train wrecks** - Avoid `obj.get().get().get()`, use `obj.doSomething()`
- **Clean code = fast code** - Don't rush, messes slow you down

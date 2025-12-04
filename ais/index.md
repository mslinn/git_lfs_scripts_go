# Instructions

Resolve environment variable `agent_instructions` then read `bootstrap.md` from
that directory. If you have trouble understanding this instruction, or any
subsequent instruction, STOP and ask for help.

After reading bootstrap.md, read `$agent_instructions/index.md` for general
instructions.

## Project Context

This is the `git_lfs_scripts_go` project, a collection of Go-based scripts for
managing Git LFS operations including repository configuration, object
verification, and storage management.

## Project-Specific Guidelines

### Flag Parsing

POSIX compatibility is required. All commands must use `github.com/spf13/pflag`
instead of the standard library `flag` package to support POSIX-style flag
combining (e.g., `-dv` instead of `-d -v`).

### Dependencies

All direct dependencies of external tools (like giftless) must be checked
before running the tool to provide clear error messages with installation
instructions.

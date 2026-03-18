# laravel-prod-ready

A Claude Code skill that runs a comprehensive production readiness audit on Laravel applications. Evaluates your project across 6 dimensions — Security, Scalability, Reliability, Hardening, Code Quality, and Operational Readiness — and produces a scored report with actionable, Laravel-specific fixes.

## What it does

- **6-dimension audit** — systematically checks security vulnerabilities, N+1 queries, missing error handling, exposed debug tools, test coverage, and CI/CD gaps
- **Scored report** — each dimension scored 0-10 with an overall READY / ALMOST / NOT READY rating
- **Actionable fixes** — concrete Laravel code, Artisan commands, and config changes — not generic advice
- **Read-only** — never modifies your project files

## Install

**Claude Code CLI:**
```bash
claude skill add --from meirdick/laravel-prod-ready
```

**Laravel Cloud (Boost):**
```bash
php artisan boost:add-skill meirdick/laravel-prod-ready
```

**Manual:**
Copy the `skills/laravel-prod-ready/` directory into your Claude Code skills directory (`~/.claude/skills/` or `.claude/skills/` in your project).

## Prerequisites

- A Laravel application (8.x through 12.x)
- PHP/Composer project

## Usage

Invoke the skill in any Laravel project:

```
/laravel-prod-ready
```

Or ask naturally: "Is this ready for production?", "Run a security check", "Audit my project before deploy"

## License

MIT

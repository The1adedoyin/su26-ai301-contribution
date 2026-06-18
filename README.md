# AI301 Open Source Contribution Log
**Adedoyin Mogaji** | CodePath AI301 — Summer 2026 | Section 1A | Wednesdays 4–6PM PT

---

## Current Status
**Phase II — Reproduce & Plan** | Last Updated: June 14, 2026

---

## My Issue

| Field | Details |
|---|---|
| **Issue Title** | python: Add comprehensive Google-style docstrings to telegram_bot.py helpers |
| **Repository** | openalgo |
| **Organization** | marketcalls |
| **Issue Link** | https://github.com/marketcalls/openalgo/issues/897 |
| **Language** | Python |
| **Status** | Claimed — Phase I |

---

## Problem Summary

Two helper functions in `telegram_bot.py` have minimal docstrings. The `run_async()` function bridges async and sync contexts — a non-trivial pattern that deserves proper documentation. The goal is to add comprehensive Google-style docstrings with Args, Returns, Raises, and Example sections to both functions in `restx_api/telegram_bot.py` (lines 92 and 263).

## Why I Chose This Issue

I chose this issue because it is clearly scoped, directly explained, and points to exact files and line numbers — leaving no ambiguity about what needs to be done. It is a pure Python task that aligns with my goal of re-sharpening my Python skills through a real contribution. The repository is actively maintained and the maintainer has provided an example of exactly what the finished output should look like, making this an ideal first open source contribution.

---

## Phase I — Issue Selection
**Status: In Progress** | Deadline: June 8, 2026

| Deliverable | Status |
|---|---|
| GitHub account active | ✅ Complete |
| Issue selected from approved list | ✅ Complete |
| Comment left on GitHub issue | ✅ Complete |
| Comment left on course Google Sheet | ✅ Complete |
| Contribution README created | ✅ Complete |
| Issue link + problem summary in README | ✅ Complete |
| Repo forked | ⬜ Pending |
| Check-in form submitted | ⬜ Pending |
| Announced in Slack | ⬜ Pending |

---

## Phase II — Reproduce & Plan
**Status: Complete** | Completed: June 17, 2026

### Environment Setup
Cloned the forked repository locally using Git and PowerShell. Opened the project in VS Code using the `code .` command. No dependency errors or setup issues encountered. Environment was running and ready within 10 minutes.

### Steps to Reproduce
1. Navigate to `restx_api/telegram_bot.py` in the repository
2. Locate the `run_async()` function (around line 92)
3. Observe the docstring is a single line: `"Helper to run async coroutine in sync context"` — no Args, Returns, Raises, or Example sections
4. Locate the `get_webhook_secret()` function (around line 263)
5. Observe the docstring has a two-line description only — no Args, Returns, Raises, or Example sections
6. **Expected:** both functions have comprehensive Google-style docstrings
7. **Actual:** both functions have minimal docstrings that do not meet Google-style standards

### Branch Link
https://github.com/The1adedoyin/openalgo/tree/fix-issue-897

### Implementation Plan

**Understand:** Two helper functions in `restx_api/telegram_bot.py` — `run_async()` and `get_webhook_secret()` — have minimal docstrings that do not meet Google-style standards. They are missing Args, Returns, Raises, and Example sections. The goal is to add comprehensive Google-style docstrings to both functions.

**Match:** Google-style docstrings follow a consistent format used across Python open source projects. The format includes a one-line summary, optional extended description, and clearly labeled sections for Args, Returns, Raises, and Example.

**Plan:**
1. Replace the single-line docstring in `run_async()` with a full Google-style docstring documenting the `coro` parameter (Coroutine type), the return value (Any), potential exceptions (RuntimeError, Exception), and a usage example
2. Replace the two-line docstring in `get_webhook_secret()` with a full Google-style docstring documenting the return value (str or None), potential exceptions (ValueError, Exception), and a usage example
3. Verify formatting matches Google-style conventions throughout

**Implement:** Changes committed to fix-issue-897 branch — https://github.com/The1adedoyin/openalgo/tree/fix-issue-897

**Review:** Will review against the openalgo repository's contribution guidelines and existing code style before opening a pull request.

**Evaluate:** Manually verify both functions display complete Google-style docstrings with all required sections. Confirm no other code in the file was accidentally modified.

---

## Phase III — Build
**Status: Not Started**

*(To be filled in during Weeks 3+)*

---

## Phase IV — Submit & Iterate
**Status: Not Started**

*(To be filled in during Weeks 4+)*

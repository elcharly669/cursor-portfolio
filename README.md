# Cursor Portfolio — Setup Steps

This repository documents the first step of the portfolio project process: installing the required tools, creating a public GitHub repo, and pushing this README.

## Tools installed

| Tool | Version / ID | Notes |
|------|----------------|-------|
| **Cursor IDE** | 3.5.38 | Installed at `/usr/bin/cursor` on Linux (x64) |
| **Claude Code** (extension) | `anthropic.claude-code` v2.1.153 | Installed via `cursor --install-extension anthropic.claude-code` |
| **Codex** (extension) | `openai.chatgpt` v26.519.32039 | Marketplace name: *Codex – OpenAI's coding agent*; installed via `cursor --install-extension openai.chatgpt` |
| **GitHub CLI** (`gh`) | Authenticated as **elcharly669** | Used to create the public repo and push |

## Steps completed

1. Installed **Cursor IDE** from [cursor.com](https://cursor.com/).
2. Installed the **Claude Code** add-on in Cursor (Extensions → search "Claude Code", publisher: Anthropic).
3. Installed the **Codex** add-on in Cursor (Extensions → search "OpenAI Codex" / "Codex", publisher: OpenAI).
4. Created a public GitHub repository: [elcharly669/cursor-portfolio](https://github.com/elcharly669/cursor-portfolio).
5. Opened the repository in Cursor at `~/Documents/cursor-portfolio`.
6. Created this `README.md` with tools, steps, and issues documented.
7. Committed and pushed to GitHub.
8. Ready to reply to the email with the link below.

## Issues encountered and how they were solved

### 1. Codex extension ID was not obvious

**Issue:** Running `cursor --install-extension openai.codex` failed with "extension not found."

**Solution:** Queried the VS Code Marketplace API and found the official extension ID is `openai.chatgpt` (display name: *Codex – OpenAI's coding agent*). Installed with:

```bash
cursor --install-extension openai.chatgpt
```

### 2. Claude Code may not appear in Cursor's search on some setups

**Issue:** The assignment says to search Extensions for "Claude Code"; on some Cursor builds it does not show in the UI search even though the marketplace has it.

**Solution:** Installed from the terminal, which works reliably:

```bash
cursor --install-extension anthropic.claude-code
```

If that fails, Anthropic documents a manual VSIX install from the local Claude Code CLI path (`~/.claude/local/node_modules/@anthropic-ai/claude-code/vendor/claude-code.vsix`).

### 3. Extension sign-in (login)

**Issue:** Installing an extension does not log you in automatically; each add-on needs an account (Anthropic for Claude Code, ChatGPT or OpenAI API for Codex).

**Solution:** After install, open each extension from the sidebar and complete sign-in in the browser or in-editor prompt. This README only confirms installation; login is done once per machine in the Cursor UI.

### 4. Empty workspace / new folder

**Issue:** The project folder started with no files and was not yet a git repository.

**Solution:** Initialized git locally, created this README, then used `gh repo create` to create the public remote and pushed `main`.

## Link for the application reply

**README on GitHub:** https://github.com/elcharly669/cursor-portfolio/blob/main/README.md

---

*Repository created as part of the portfolio onboarding step. The project itself will be built in later steps.*

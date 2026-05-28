# Cursor Portfolio — Setup

Onboarding step for the portfolio process: confirm the toolchain, open a public repo, push this file.

## Tools

| Tool | Version / ID |
|------|----------------|
| Cursor | 3.5.38 |
| Claude Code | `anthropic.claude-code` |
| Codex (OpenAI) | `openai.chatgpt` |
| Git + `gh` | `elcharly669` |

## Steps completed

1. Cursor — already on the machine.
2. Extensions — `cursor --install-extension anthropic.claude-code` and `openai.chatgpt` (store name: *Codex – OpenAI's coding agent*).
3. Repo — `git init`, README, `gh repo create cursor-portfolio --public --push`.

## Issues (only worth noting)

- **`openai.codex` is not the extension ID.** Marketplace publishes Codex as `openai.chatgpt`.
- **Claude Code may not show in Cursor's extension search.** CLI install works; VSIX from the local Claude install is the fallback.
- **Fresh folder** — not a git repo until `git init`; remote via `gh repo create`.

**README link:** https://github.com/elcharly669/cursor-portfolio/blob/main/README.md

## Notes

Cursor is the editor; Claude Code and Codex are agent panes on the same tree and terminal. In day-to-day work that means one checkout, one diff history, and model choice by task—not re-uploading context per tool. Git and `gh` are what make the repo step fast; the extensions are the part that actually ships changes when you're already living in the terminal and in PRs.

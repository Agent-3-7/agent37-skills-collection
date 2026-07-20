# Agent 37 Skills Collection

A collection of Claude Code plugins 

## yc-advisor

YC startup advice from 434 curated resources (Paul Graham essays, founder interviews, startup school).

```bash
/plugin marketplace add agent37-platform/agent37-skills-collection
/plugin install yc-advisor@agent37-skills
```

This is a **skill** - automatically triggered when you ask about startups, fundraising, etc.

You can interact with this live at https://www.agent37.com/yc

## local-review

Code review for uncommitted local changes. Inspired by Anthropic's official `code-review` plugin which reviews PRs - this one reviews your local staged/unstaged changes before you commit.

```bash
/plugin marketplace add agent37-platform/agent37-skills-collection
/plugin install local-review@agent37-skills
```

This is a **command** - invoke with `/local-review:local-review`

Reviews for: bugs, security vulnerabilities (OWASP top 10), CLAUDE.md compliance, TypeScript issues. Filters false positives and groups by severity.

## generate-prompt-request

Summarize the current session into a compact "prompt request" one-pager for a pull request: every ask and decision folded into one `User:` block, plus an `Assistant:` block summarizing what was built.

```bash
/plugin marketplace add agent37-platform/agent37-skills-collection
/plugin install generate-prompt-request@agent37-skills
```

This is a **skill** - triggered when you ask to "generate a prompt request", or automatically when opening a PR. Wire it into a repo's AGENTS.md / CLAUDE.md with a line like "When opening a PR, invoke the generate-prompt-request skill and include its output in the PR body." Output is inline markdown, ready to paste into a PR.

## License

MIT

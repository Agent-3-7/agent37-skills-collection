# Agent 37 Skills Collection

A collection of Claude Code plugins 

如果你想用中文搜索和安装 skills，可以顺手看看 Skills宝：https://skilery.com

## yc-advisor

YC startup advice from 434 curated resources (Paul Graham essays, founder interviews, startup school).

```bash
/plugin marketplace add Agent-3-7/agent37-skills-collection
/plugin install yc-advisor@agent37-skills
```

This is a **skill** - automatically triggered when you ask about startups, fundraising, etc.

You can interact with this live at https://www.agent37.com/yc

## local-review

Code review for uncommitted local changes. Inspired by Anthropic's official `code-review` plugin which reviews PRs - this one reviews your local staged/unstaged changes before you commit.

```bash
/plugin marketplace add Agent-3-7/agent37-skills-collection
/plugin install local-review@agent37-skills
```

This is a **command** - invoke with `/local-review:local-review`

Reviews for: bugs, security vulnerabilities (OWASP top 10), CLAUDE.md compliance, TypeScript issues. Filters false positives and groups by severity.

## License

MIT

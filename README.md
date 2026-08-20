# Nontechnical Agent Skills

AI agents often turn a simple request into a lesson about terminals, Git, ports, dependencies, and configuration files. This bundle teaches them to finish the work and explain only what the person needs to know.

It uses the open `SKILL.md` format supported by Claude Code, Codex, and other compatible agent tools.

## Included skills

- `nontechnical-copilot` keeps the agent focused on the user's outcome and plain-language updates.
- `setup-without-confusion` handles installs, sign-in, Git, GitHub, localhost, publishing, and similar setup work.
- `natural-writing` removes robotic AI habits and technical clutter. It uses no linting API or external service.

## Easiest installation

Send this sentence to an agent that can access files and GitHub:

> Install every skill from https://github.com/adamholter/nontechnical-agent-skills as personal skills for this agent. Verify that all three skills are discoverable, then tell me only whether it worked.

Common personal skill folders:

- Claude Code: `~/.claude/skills/`
- Codex: `~/.codex/skills/`

You can also copy any folder inside `skills/` into the personal or project skills folder used by your agent.

## Suggested first message

> I am not technical. Handle the setup for me, use plain language, and only ask me to do something when you cannot do it yourself.

The skills can load automatically when a request matches. They can also be named directly, such as `$nontechnical-copilot`.

## Design choices

- The agent does the work when it has the tools and permission.
- Necessary terms get a one-sentence explanation.
- Helpful, task-scoped automation is allowed.
- The agent verifies the app, page, account, or other result the user will see.
- The setup skill checks for secrets and private data before public publishing.

The writing skill shares the goal of [Unslop](https://github.com/theclaymethod/unslop): remove common AI writing habits. This bundle contains its own short rules and does not include Unslop's scanners, linting system, or API features.

## License

MIT. Use, change, and share it.

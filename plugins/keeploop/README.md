# Keeploop commands for Claude

[Keeploop](https://keeploop.app) is the personal context layer for your AI: a Mac menu bar app
that lets the AI apps you already use read your Mail, Messages, Calendar, Notes and Slack, right
on your Mac. Everything stays on your Mac, and you decide what each AI can see and do.

This repository is the plugin marketplace for the Keeploop commands in Claude chat: the Claude
app, claude.ai and the Claude phone app. The plugin holds only the `/keep-` commands, as plain
Markdown. It has no server, no hooks and no code. The mail tools come from the Keeploop app
itself, through its Claude extension on your Mac or the Keeploop Remote connector on the web
and your phone.

| Command | What it does |
|---|---|
| `/keep-brief` | Unread mail, what needs a reply, and today's monitor hits |
| `/keep-reply` | Threads where someone is waiting on you, with a suggested next step each |
| `/keep-thread` | Summarize a whole conversation: decisions and open questions |
| `/keep-draft` | Draft a threaded reply that sounds like you. Saves a draft only |
| `/keep-find` | Find a file someone sent you by describing it |
| `/keep-waiting` | Mail you sent that nobody has answered yet, oldest first |
| `/keep-help` | List the commands |

## Install

The easiest route is Keeploop > Settings > Connect > Claude > Install, which opens Claude's
Add plugin dialog with this plugin filled in. Or in Claude: Customize > Plugins > Add, then
add the marketplace `keeploopapp/keeploop` and the plugin `keeploop`.

Claude Code users get the same commands, plus the local tools, from the
[Claude Code plugin](https://github.com/keeploopapp/claude-plugin) instead.

## Privacy and support

- Privacy: <https://keeploop.app/privacy>
- Terms: <https://keeploop.app/terms>
- Support: <https://keeploop.app/support> or help@keeploop.app

## License

The files in this repository are MIT licensed (see `LICENSE`). The Keeploop app itself is
separate, proprietary software and is not part of this repository.

This repository is generated from the Keeploop release build; please send changes as issues
rather than pull requests.

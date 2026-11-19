# Afterchat for Claude

Afterchat is a customer support chat for software teams: the chat on your site, the inbox behind it, and a knowledge vault the chat answers from. This plugin connects Claude to your Afterchat workspace and adds skills for the work around it: answering the inbox, filling what the vault couldn't answer, keeping the vault in shape, and building what customers ask for.

## Install

In Claude Code:

```
/plugin marketplace add sebastianveeti/afterchat-plugin
/plugin install afterchat@afterchat
```

Then run `/mcp`, choose afterchat and sign in. Signing in makes an Afterchat account if you don't have one, and you pick the workspace and untick anything Claude should not do. Afterchat is free while in early access.

## Skills

Claude uses these by itself when a task fits, or you run them by name:

- `/afterchat:inbox` works the chats waiting on the team, technical ones first.
- `/afterchat:investigate <conversation id>` digs into one chat with the code.
- `/afterchat:gaps` answers what the vault couldn't, from the code.
- `/afterchat:review` checks unchecked drafts and Tidy up's suggestions against the code.
- `/afterchat:vault` builds or reorganizes the vault.
- `/afterchat:triage` weighs what customers asked for against the codebase.
- `/afterchat:build <request>` builds a request from its brief.
- `/afterchat:ship <request>` tells everyone who asked and updates the vault.

`build` and `ship` only run when you ask for them.

## What it runs and sends

The plugin runs no code on your computer. It is a set of instructions and one connection: Afterchat's MCP server at https://afterchat.chat/mcp, which you sign in to. What Claude reads and writes goes between Claude and your Afterchat workspace, as the person who signed in. Replies to customers wait for a person's approval unless a workspace owner lets them go out at once, and everything Claude changes is in the workspace's log with an undo. Privacy policy: https://afterchat.chat/privacy

## License

MIT

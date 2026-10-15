# Opal for Claude

Opal looks after your membership website: she checks your sites, proposes plans, and opens changes for your approval. This plugin lets you talk to her from Claude.

Once it's installed, you can ask things like:

- What's waiting on me?
- How are my sites doing?
- What has Opal done lately?
- Approve the plan for my homepage.

## What it connects to

The plugin adds one remote connector, Opal's own server at `https://opalagent.app/mcp`. It runs nothing on your computer and installs no packages.

The first time Claude uses it, you sign in to Opal in your browser and choose what Claude may do: look, talk with Opal, or act for you. Claude then sends your questions to that server and shows you what Opal answers. Opal reads only your own Opal account. Anything that changes something, like approving a plan or undoing a change, asks you first.

You can disconnect at any time in the Opal app: Memory, then Connected assistants, then Revoke.

## Install

In Claude Code:

```
/plugin install opal-agent --marketplace sethshoultes/opal-plugins
```

## You need

An Opal account. Sign up at [opalagent.app](https://opalagent.app).

## Privacy and help

- Privacy: [opalagent.app/privacy](https://opalagent.app/privacy)
- Help: [opalagent.app/support](https://opalagent.app/support)
- Connecting step by step: [opalagent.app/docs/connect-claude](https://opalagent.app/docs/connect-claude/)

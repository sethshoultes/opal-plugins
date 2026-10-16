# Opal for ChatGPT: the app's listing kit

ChatGPT apps aren't installed from a repository. An app is submitted in the OpenAI platform with the address of its server and the listing fields below. This folder holds those fields and the two icons, so the listing can be checked in public.

## The app

Opal looks after membership websites. The ChatGPT app connects to Opal's own server:

- **MCP URL:** https://opalagent.app/mcp
- **Sign in:** OAuth. The first time ChatGPT uses Opal, you sign in to Opal in your browser and choose what ChatGPT may do: look, talk with Opal, or act for you. You can disconnect at any time in the Opal app: Memory, then Connected assistants, then Revoke.

## Name

Opal

## Short description

ChatGPT caps it at 30 characters:

I look after your website

## One line description (80 characters or fewer)

I look after your website and tell you what is waiting on you.

## Long description

I am Opal, and I look after membership websites. I watch your sites, run checks on them every day and suggest fixes when something is wrong. When a change needs your OK, I wait for you. Here you can ask me how your sites are doing, what I have done lately and what is waiting on you. If you allow it, you can also chat with me as you would in the Opal app, and say yes or no to the plans and changes I bring you. Nothing I do from here can pay for anything or change your subscription, and you can disconnect me at any time in the Opal app.

## Starter prompts

1. What is waiting on me in Opal?
2. How are my sites doing?
3. What has Opal done on my site this week?

## Category

Productivity

## Icons

- [`icon-512.png`](icon-512.png): 512 by 512, the directory logo.
- [`icon-64.png`](icon-64.png): 64 by 64, the composer icon.

Both are the Opal stone on Opal's night background (#08091e), full bleed.

## Links

- Website: https://opalagent.app
- Privacy policy: https://opalagent.app/privacy
- Support: https://opalagent.app/support

## What the person allows

You choose one of three levels on the sign in screen:

- **Look** (the default): read only. Your sites and their checks, what is waiting on you, what Opal has done lately, what she remembers, your projects, ideas, brand kit and forms, whether Google is connected, and the searches a site is close to ranking for.
- **Talk with Opal:** send her a message as in the app's chat, and read your chat with her.
- **Act for you:** say yes or no for you: approve, decline or choose a plan, approve or undo a change, start a project and decide its proposal, style, review rounds and launch, the content plan, ideas, check in times, correcting or forgetting a memory, and the brand kit.

The read tools are marked read only. Talking to Opal and the tools that change a site or delete something are marked as needing your OK, so ChatGPT asks you first. On every level, Opal can't pay for anything or change your subscription.

## Test cases

Five that should work:

1. "What is waiting on me in Opal?" shows the waiting card with each plan or change, its site and how long it has waited.
2. "How are my sites doing?" shows the sites card with each site's health and last check.
3. "What has Opal done on my site this week?" answers from her recent activity.
4. "What does Opal remember about me?" answers from her memory of you.
5. Asked before signing in, any of the above shows the sign in button, and works after signing in.

Three that should not:

1. With only Look allowed, "Approve the change on my site" is refused: approving needs Act for you, and ChatGPT says so.
2. "Show me another customer's sites" shows nothing of anyone else's.
3. "Upgrade my plan" or "pay my invoice" is not done at any level.

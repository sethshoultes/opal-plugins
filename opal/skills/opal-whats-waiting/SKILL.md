---
name: opal-whats-waiting
description: Use when the person asks what is waiting on them in Opal, what needs their OK, or wants to approve, decline or undo something Opal proposed or changed on their website. Also use when they ask how to talk to Opal herself, or what Opal can do for a MemberPress or CreatorPress membership site.
---

# What's waiting on the person, and how they answer it

Opal looks after the person's website. She proposes plans (a fix, a new page, an improvement) and opens changes for them to approve. Nothing she proposes goes live until the person says yes.

## Find out what's waiting

Call `whats_waiting` first whenever the person asks what needs them, what Opal wants, or "anything new?". It lists two kinds of thing:

- **Plans** Opal has proposed and is waiting to build. A plan can offer more than one way to build it.
- **Changes** ready for approval: work Opal has done, with a preview link where there is one.

Show each item in plain words: what it is, which site, and the preview link if there is one. Don't paste ids or raw fields unless the person asks.

If nothing is waiting, say so in one line. `get_activity` shows what Opal has done lately, if they want to know what happened instead.

## Answer it, only with the person's yes

These all change something, so ask the person first and act only on a clear yes for that exact item. Never approve, decline or undo on your own judgment, and never several items at once unless the person named them.

- `approve_plan`: Opal builds the plan. If it offers more than one way, ask which; `chosen` is that way's index as `whats_waiting` showed it.
- `choose_plan_option`: pick one way without approving yet.
- `decline_plan`: Opal builds nothing.
- `approve_change`: Opal puts the change live (she merges it).
- `undo_change`: Opal reverts a change she made.
- `dismiss_repo_offer`: say no thanks to a code repository Opal offered as a site.

After acting, tell the person what happened in one line, and what Opal does next if she said.

## Talk to Opal herself

`chat_with_opal` sends a message to Opal, as in the app's chat, and returns her answer and any cards she shows. Use it when the person wants Opal to do something the other tools don't cover, like starting a site review or asking her a question about their site. It counts against their AI allowance, so ask before sending, and send their words, not your own plan. `get_chat_history` shows the conversation so far.

## MemberPress and CreatorPress site owners

Opal works on membership websites, including sites built on MemberPress or CreatorPress. She looks after the website itself: its pages, speed, links, search, content and design. She has no tools yet for members, memberships, payments or subscriptions, so she can't look up a member, change a plan's price or refund a payment. Say that plainly if asked, and point them to their site's own admin for it.

## Help

- What Opal is: https://opalagent.app
- Help: https://opalagent.app/support
- Privacy: https://opalagent.app/privacy

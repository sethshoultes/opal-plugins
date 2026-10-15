---
name: opal-projects-and-content
description: Use when the person asks about an Opal project (a new site or a redesign), its proposal, style, review rounds or launch, or wants to start one. Also use for their ideas, a site's monthly content plan, their brand kit, their forms, or what Opal remembers about them, including correcting or forgetting something.
---

# Projects, content, brand and memory

Reading is always fine. Anything that changes something asks the person first: say what you will do, and act only on a clear yes for that exact thing.

## Projects: a new site or a redesign

- `list_projects`, then `get_project` for one: its brief, stage, style directions, proposal, review rounds, launch ask and preview link. `get_project` also gives the ids and version numbers the actions below need.
- `start_project` (ask first): start a project from the person's goal. Only the goal is needed; Opal asks for the rest.
- `decide_proposal` (ask first): approve the proposal, or send it back with the person's comment.
- `pick_style` (ask first): pick one of the style directions; Opal builds in it.
- `decide_review_round` (ask first): approve the round, or ask for changes with their comment.
- `decide_launch` (ask first): approving puts the site live; declining keeps it waiting at launch.

Share the preview link before asking someone to approve a proposal, a round or a launch.

## Ideas

- `list_ideas`: the person's ideas, with status, steps, cost so far, and any "still worth it?" question Opal is waiting on.
- `update_idea` (ask first): pause, resume or drop an idea. Dropping stops it for good, so say so.
- `answer_still_worth` (ask first): keep an idea going, or stop it.
- `set_checkin` (ask first): how often Opal checks in on a site's ideas: never, with each plan, or weekly.

## Content plan

- `get_content_plan`: one site's topics for a month, in order, and the rejected ones.
- `edit_content_topic` (ask first): pin, unpin, reject or move one topic.
- `refresh_content_plan` (ask first): rebuild the month from fresh numbers. Pinned and rejected topics are kept.

## Brand kit

- `get_brand`: the brand kit as it is now (colours, fonts, voice), its history, and the logo and brief files.
- `save_brand_kit` (ask first): save a new version. Read `get_brand` first and send the whole kit with the change, not only the changed part.
- `undo_brand_kit` (ask first): go back to the version before the newest.
- `delete_brand_file` (ask first): delete one logo or brief file.

## Forms

`list_forms` lists the person's forms: kind, title, site, whether each is live, how entries are delivered, and how many there are. It never shows the entries themselves. To change a form, the person asks Opal (see the opal-whats-waiting skill on talking to Opal).

## What Opal remembers

- `get_memory`: what Opal keeps about the person: their decisions, preferences, ideas, facts and promises.
- `correct_memory` (ask first): fix one item, in the person's own words.
- `forget_memory` (ask first): have Opal forget one item.
- `list_connections`: the assistants connected to their Opal account. Disconnecting happens in the Opal app, under Memory, then Connected assistants.

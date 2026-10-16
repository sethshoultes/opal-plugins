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

- `list_forms`: the person's forms: kind, title, site, whether each is live, how entries are delivered, and how many there are. It never shows the entries themselves.
- `form_create` (ask first): make a contact, quote or signup form. It is saved, but it is on no site and takes no entries yet.
- `form_edit` (ask first): change a form. A form not on a site changes at once. On a live form, a change to its title or fields opens a change on the site that waits for the person's approval (see `whats_waiting`).

Both take the person's ask, which Opal writes down: `request` is what they asked, in their own words exactly as they said it to you; `restatement` is what you understood; `done_means` is how you will both know it is done.

Some form changes happen only in the Opal app: putting a form on a site, where a live form's entries go, its thank-you, and the address of a CRM entries are sent to. Reading entries happens there too. If the person asks for one of these, say so and point them to the app.

## What Opal remembers

- `get_memory`: what Opal keeps about the person: their decisions, preferences, ideas, facts and promises.
- `correct_memory` (ask first): fix one item, in the person's own words.
- `forget_memory` (ask first): have Opal forget one item.
- `list_connections`: the assistants connected to their Opal account. Disconnecting happens in the Opal app, under Memory, then Connected assistants.

---
name: opal-sites
description: Use when the person asks how their websites are doing in Opal, about uptime, speed, SSL, broken links or SEO checks, what Opal has done on a site lately, a site review, how far along their first site's setup is, or which Google searches a site is close to ranking for. Also use for the site logins they stored in Opal, revoking one, or choosing or disconnecting the Google account a site reads.
---

# The person's sites and how they are doing

Most tools here only read and change nothing, so you can call them without asking. The ones marked (ask first) change something: say what you will do, and act only on a clear yes for that exact thing.

## How a site is doing

- `list_sites`: every site Opal looks after, with the latest result of each check (uptime, speed, SSL, links, SEO). Start here for "how are my sites?". Lead with anything failing or getting worse, then say the rest is fine in one line.
- `get_activity`: what Opal has done lately, newest first: checks run, changes opened, merged or undone. Pass `site_id` for one site. For older items, pass the `nextBefore` value from the last page as `before`.
- `get_site_review`: the latest site review for one site, or whether one is running. Only Opal starts a review. If the person wants a new one, ask before sending the request to Opal with `chat_with_opal` (see the opal-whats-waiting skill).
- `get_onboarding`: where the person is in setting up their first site (adding the domain, proving they own it, installing, the first check, or done), and which domain. Use it when they ask why a site isn't showing yet.

## Search

- `google_status`: whether Google Search Console and Analytics are connected for each site, and which properties. Opal only reads Google's data.
- `get_striking_queries`: searches where a site is close to page one, the striking-distance list. It needs Google connected for that site. If it isn't, say so and point the person to connecting Google in the Opal app.
- `google_pick_property` (ask first): when more than one Google property matches a site. Called with no property, it lists the ones that match; ask which, then call it again with that one to save it.
- `google_disconnect` (ask first): stop Opal reading Google for one site. She asks Google to remove her access and deletes her key for it.

Connecting Google happens in the Opal app, which shows Google's own consent screen.

## Stored logins

- `list_logins`: the site logins the person stored in Opal's locked store: site, label, when it was stored, and its login_id for `revoke_login`. It never shows the login itself.
- `revoke_login` (ask first): delete one stored login from the store. Opal can no longer use it, and the person would have to give it again.

Giving Opal a login happens only in the Opal app's secure form, never in chat.

## Passing the person's ask

The ask-first tools above that change Google (`google_pick_property`, `google_disconnect`) also take the person's ask, which Opal writes down: `request` is what they asked, in their own words exactly as they said it to you; `restatement` is what you understood; `done_means` is how you will both know it is done.

## How to answer

Use plain words. Say "the site was down for 4 minutes on Tuesday", not the raw check record. Give numbers the person can act on, and name the site. If a check failed and Opal has already proposed a fix, say so and offer to show it with `whats_waiting`.

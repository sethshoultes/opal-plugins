---
name: opal-sites
description: Use when the person asks how their websites are doing in Opal, about uptime, speed, SSL, broken links or SEO checks, what Opal has done on a site lately, a site review, how far along their first site's setup is, or which Google searches a site is close to ranking for.
---

# The person's sites and how they are doing

Every tool here only reads. None of them changes the site, so you can call them without asking.

## How a site is doing

- `list_sites`: every site Opal looks after, with the latest result of each check (uptime, speed, SSL, links, SEO). Start here for "how are my sites?". Lead with anything failing or getting worse, then say the rest is fine in one line.
- `get_activity`: what Opal has done lately, newest first: checks run, changes opened, merged or undone. Pass `site_id` for one site. For older items, pass the `nextBefore` value from the last page as `before`.
- `get_site_review`: the latest site review for one site, or whether one is running. Only Opal starts a review. If the person wants a new one, ask before sending the request to Opal with `chat_with_opal` (see the opal-whats-waiting skill).
- `get_onboarding`: where the person is in setting up their first site (adding the domain, proving they own it, installing, the first check, or done), and which domain. Use it when they ask why a site isn't showing yet.

## Search

- `google_status`: whether Google Search Console and Analytics are connected for each site, and which properties. Opal only reads Google; she never changes anything there.
- `get_striking_queries`: searches where a site is close to page one, the striking-distance list. It needs Google connected for that site. If it isn't, say so and point the person to connecting Google in the Opal app.

## How to answer

Use plain words. Say "the site was down for 4 minutes on Tuesday", not the raw check record. Give numbers the person can act on, and name the site. If a check failed and Opal has already proposed a fix, say so and offer to show it with `whats_waiting`.

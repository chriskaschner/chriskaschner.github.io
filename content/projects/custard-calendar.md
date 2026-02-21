---
title: "Custard Calendar"
date: 2026-02-21
summary: "Full-stack Culver's Flavor of the Day tracking — calendar sync, Cloudflare Worker API, and Tidbyt pixel art"
tags: ["javascript", "python", "starlark", "cloudflare-workers", "tidbyt"]
weight: 1
---

A system for tracking Culver's Flavor of the Day across 1,071 locations.

![Tidbyt 3-day flavor forecast](/images/projects/example.gif)

*3-day flavor forecast on a 64x32 pixel Tidbyt LED display — 29 flavor profiles with unique color-coded scoops, ribbons, and toppings.*

![Tidbyt scrolling location name](/images/projects/example-long.gif)

*Scrolling marquee for long location names.*

**What it does:**
- Scrapes flavor schedules and syncs them to Google Calendar with emoji and descriptions
- Cloudflare Worker serves a public subscribable `.ics` calendar with store search API for all 1,071 locations
- Tidbyt LED display app shows a 3-day forecast with pixel-art ice cream cones
- Store manifest built from OpenStreetMap data + Culver's slug probing

**Tech:** JavaScript, Python, Starlark, Cloudflare Workers, Google Calendar API

[custard-calendar](https://github.com/chriskaschner/custard-calendar) | [custard-tidbyt](https://github.com/chriskaschner/custard-tidbyt)

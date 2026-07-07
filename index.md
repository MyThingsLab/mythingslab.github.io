---
title: Home
layout: home
nav_order: 1
---

# MyThingsLab

MyThingsLab is an SDK, [`my-things-core`](https://github.com/MyThingsLab/my-things-core),
plus a fleet of small autonomous **My[X]** tools. Each tool follows the same
shape: read a GitHub issue, do deterministic pre-work, make one LLM call, and
open a PR — never a merge. A human always merges.

See the [architecture overview](https://github.com/MyThingsLab/my-things-core/blob/main/docs/ARCHITECTURE.md)
in `my-things-core` for how the harness and its five contracts fit together.

## Tools

{% assign tools = site.tools | sort: "title" %}
{% for tool in tools %}
- [{{ tool.title }}]({{ tool.url | relative_url }})
{% endfor %}

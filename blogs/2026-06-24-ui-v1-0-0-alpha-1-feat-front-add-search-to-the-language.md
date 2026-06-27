---
title: "ui/v1.0.0-alpha.1: feat(front): add search to the language picker (#22095)"
url: "https://github.com/twentyhq/twenty/releases/tag/ui%2Fv1.0.0-alpha.1"
date: "2026-06-24"
author: "FelixMalfait"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
What Adds a search bar to the Settings → Experience → Language picker, and makes languages searchable across languages. Each option is matched against: its displayed label (the name in the current UI language) its name in English — typing chinese finds "Chinois — Simplifié" its native name — typing 中文 finds the same option Matching is also accent-insensitive ( francais finds "Français"). How The shared Select already supports search via withSearchInput (used by the currency/country pickers) — the picker just opts in.

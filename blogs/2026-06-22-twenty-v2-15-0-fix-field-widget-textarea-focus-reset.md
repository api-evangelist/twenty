---
title: "twenty/v2.15.0: Fix field widget textarea focus reset (#21959)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.15.0"
date: "2026-06-22"
author: "Bonapara"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Release v2.15.0 keeps the field widget textarea on a local draft value while focused so record-store rewrites do not reset the active caret. Typing in editor-mode text fields previously lost caret position during external record updates.

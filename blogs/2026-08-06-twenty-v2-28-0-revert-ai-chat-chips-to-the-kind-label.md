---
title: "twenty/v2.28.0: Revert AI chat chips to the [[kind:...:label]] syntax (#23852)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.28.0"
date: "2026-08-06"
author: "bosiraphael"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Removes the [[kind:...:label[[/kind]] closing-tag syntax and goes back to the simpler [[kind:...:label]] form for all four chip kinds (record, object, field, view). The parser is now a single regex pass instead of a two-pass scan with a per-reference closing-tag search, a legacy fallback and surplus-bracket handling. That removes 11 files.

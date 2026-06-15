---
title: "twenty/v2.13.0: [Experiment] perf(front): cache-first currentUser bootstrap (#21532)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.13.0"
date: "2026-06-13"
author: "FelixMalfait"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Experiment — not for merge as-is A perf experiment for discussion. Opening as a draft to gather feedback and let CI run. Problem On a warm (returning) load, the app gate ( MinimalMetadataGater ) blocks first paint until both object/view metadata and currentUser are ready.

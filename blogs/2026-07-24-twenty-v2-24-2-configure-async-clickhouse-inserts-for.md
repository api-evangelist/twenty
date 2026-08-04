---
title: "twenty/v2.24.2: Configure async ClickHouse inserts for pageview events (#23274)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.24.2"
date: "2026-07-24"
author: "Weiko"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Context Pageview tracking goes through the trackAnalytics mutation on the metadata API and is persisted through the unified event pipeline before the mutation resolves. ClickHouse inserts already use: async_insert = 1 wait_for_async_insert = 1 async_insert lets ClickHouse buffer and batch small inserts, but wait_for_async_insert = 1 still keeps the API request open until that buffer is flushed successfully. For sparse pageview inserts, the buffer timeout can therefore account for most of the request duration and contribute to metadata API tail latency.

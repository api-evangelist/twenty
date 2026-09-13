---
title: "twenty/v2.39.1: Restore workflowRun.updated webhooks for explicit subscriptions (#25601)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.39.1"
date: "2026-09-08"
author: "thomtrp"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Context Follow-up to #25599 , which merged the emergency version of the mitigation: the webhook fan-out enqueue is skipped entirely for workflowRun.updated , so even webhooks explicitly subscribed to that operation receive nothing. Change Replaces the blanket skip with an opt-in matching rule: The listener enqueues webhook fan-out jobs for workflowRun.updated batches again (revert of the #25599 listener change). Operation matching for workflowRun.updated is restricted to the exact subscription string via the new computeWebhookOperationsToMatch util: explicit subscribers (settings UI picking Wo

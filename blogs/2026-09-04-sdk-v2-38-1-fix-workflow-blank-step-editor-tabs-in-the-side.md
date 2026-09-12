---
title: "sdk/v2.38.1: fix(workflow): blank step-editor tabs in the side panel (#25318)"
url: "https://github.com/twentyhq/twenty/releases/tag/sdk%2Fv2.38.1"
date: "2026-09-04"
author: "thomtrp"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
What happened Since #25141 ("Unify workspace routes across main and side panel"), the Configuration/Test tab content of the workflow step editors renders blank in the side panel. No error anywhere: the tabs display and highlight on click, but the panel below stays empty. Root cause #25141 made TabList store activeTabIdComponentState under the workspace-surface-scoped instance id ( useWorkspaceSurfaceScopedComponentInstanceId ), but did not update the components that read that state with their raw component ids.

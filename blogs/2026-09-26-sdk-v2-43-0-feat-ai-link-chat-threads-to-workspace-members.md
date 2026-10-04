---
title: "sdk/v2.43.0: feat(ai): link chat threads to workspace members (expand step) (#26564)"
url: "https://github.com/twentyhq/twenty/releases/tag/sdk%2Fv2.43.0"
date: "2026-09-26"
author: "FelixMalfait"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Problem Since 2.42, agentChatThread lives in the workspace schema, but its owner is still userWorkspaceId , a UUID that points at core.userWorkspace . That cross-schema reference led to the per-workspace FKs on core tables that #26547 removed. Since then nothing enforces it.

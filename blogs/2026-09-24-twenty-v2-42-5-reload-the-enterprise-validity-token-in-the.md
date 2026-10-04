---
title: "twenty/v2.42.5: Reload the enterprise validity token in the server process (#26449)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.42.5"
date: "2026-09-24"
author: "ijreilly"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Problem A self-hosted customer reported that their license "stops renewing", and because SSO is their login method, expiry locks everyone out. Their workaround is to disable SSO, log in with a password, reload the license, then re-enable SSO. The token is renewing fine.

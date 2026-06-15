---
title: "sdk/v2.13.0: Fix record index sync when view fields arrive via SSE (#19069)"
url: "https://github.com/twentyhq/twenty/releases/tag/sdk%2Fv2.13.0"
date: "2026-06-14"
author: "channi23"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Fixes #19023 What changed This updates the record index/view field state flow so the current view can react to late-arriving viewFields coming from SSE without requiring a page refresh. Changes: extracted a narrower syncRecordIndexViewFields path in useLoadRecordIndexStates kept the initial full record-index load for first entry into a view added a follow-up sync in RecordIndexLoadBaseOnContextStoreEffect when the same view receives updated viewFields updated ViewBarRecordFieldEffect so it re-syncs current record fields when currentView.viewFields changes instead of only initializing once Why 

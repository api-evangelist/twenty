---
title: "twenty/v2.42.1: Put the record creation form back behind a feature flag (#26472)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.42.1"
date: "2026-09-23"
author: "thomtrp"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
Puts the record creation form back behind IS_RECORD_CREATION_FORM_ENABLED , removed in #25907 . With the flag off, creating a record is the pre-form behaviour again: the record is created immediately, then opened (side panel or record page, label identifier in edit mode) as before. Changes FeatureFlagKey.IS_RECORD_CREATION_FORM_ENABLED restored: shared enum, admin panel flag metadata, dev seed (on, so local dev and the e2e create-record spec keep using the form), generated front enums and the SDK metadata client.

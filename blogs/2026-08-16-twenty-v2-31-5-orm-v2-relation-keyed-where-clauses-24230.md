---
title: "twenty/v2.31.5: ORM v2: relation-keyed where clauses (#24230)"
url: "https://github.com/twentyhq/twenty/releases/tag/twenty%2Fv2.31.5"
date: "2026-08-16"
author: "charlesBochet"
feed_url: "https://github.com/twentyhq/twenty/releases.atom"
---
What ORM v2 resolved every top-level key of a where object as a column on the main table, so a relation-keyed filter threw before any SQL ran: where: { calendarEventParticipants: { personId: Any(personIds) } } → Column "calendarEventParticipants" does not exist on "calendarEvent" applyWhere handed the object straight to queryBuilder.where() . #24225 taught the order path about relation keys ( isRelationOrderEntry → applyRelationOrderEntry ) but the where path never learned. The reference consumer is the record Timeline panel: timeline-calendar-event.service.ts filters that way in both its coun

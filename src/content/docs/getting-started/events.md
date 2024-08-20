---
title: "Events"
linkTitle: "Events"
weight: 3
categories: [Events, Getting Started]
tags: [docs]
description: Managing Events
---

Events in SpreaView represent various types of gatherings, including conferences, meetups, workshops, and other similar occasions. These events are designed to be flexible, accommodating everything from single-day meetups to multi-day conferences with multiple sessions. Each event is tied to an Organization, ensuring that all activities within the event are managed under a specific organizational entity.

## Structure of an Event

### 1. **Event Properties**

- **Name**: The name of the event.
- **Event Code**: This is a read-only generated code that can be used in public links to gather information about the conference, for example a Rooms view
- **Date range**: These are the start- and end date of your event
- **Default Session Length**: This is the default length of a session in minutes. When sessions are created manually, this setting is used to calculate end dates and review periods.
- **Default Review Length**: This is the duration of the review window in hours. The default value is 24, meaning that the session can be reviewed from the time it is scheduled to start, until exactly 24 hours later.
- **Reviews Required**: This setting allows conference organizers to draw prices between attendees who have reviewed x or more settings. This feature is enabled when a value is entered and the value is higher than 0.
- **Sessionize API ID**: When a valid Sessionize API ID is entered, this event [integrates with Sessionize](/docs/integrations/sessionize/) and allows for importing speakers and sessions from the Sessionize Schedule Builder.
- **Event theme background**: The background color of the event theme. This color is used to generate reports for speakers.
- **Event theme foregroudn**: The foreground color of the event theme. This color is used to generate reports for speakers.
- **Enable free comments**: When enabled, a free comment text field is shown for attendees on the session review page. When disabled, the comments textbox is hidden. The textbox is never a required field.

### 2. **Organization**

Each event is associated with an Organization, which serves as the host or organizer. The Organization manages the overall coordination of the event, including logistics, promotion, and participant engagement.

## Summary

SpreaView's Event feature is designed to be a versatile tool for managing and organizing a wide range of gatherings. By structuring events with clear associations to organizations and breaking down content into manageable sessions, SpreaView ensures that both organizers and participants have a streamlined and engaging experience.

---
title: "Conference Content"
linkTitle: "Content"
weight: 4
categories: [Conferences]
tags: [docs]
description: Adding a meaning to your conferences
---

# Managing Conference Content in SpreaView

The **Conference Content** section in SpreaView enables organizers to manage the essential elements of a conference, including speakers, tracks, and presentations. This functionality provides flexibility while ensuring data consistency.

> **Tip** read on to the end of the page and learn how to synchronize your conference content with Sessionize.

## Managing Speakers

Organizers can add and edit speakers for the conference.

### Key Points:

- **Adding Speakers**: New speakers can be added to the conference through this section.
- **Editing Speakers**: Speaker details can be updated as necessary.
- **Restrictions**:
  - Speakers who are assigned to one or more presentations **cannot be deleted**. This ensures the integrity of presentation data.

## Managing Tracks

Tracks represent the divisions or categories of sessions within a conference.

### Key Points:

- **Adding Tracks**: Organizers can create new tracks to categorize sessions.
- **Editing Tracks**: Existing tracks can be updated.
- **Deleting Tracks**:
  - Tracks can only be deleted if **no presentations are assigned** to them.

## Managing Presentations

![Creating a conference](/images/spreaview-conference-presentations.png)

Presentations are the core components of a conference, linking speakers and tracks to the conference schedule.

### Key Points:

- **Adding Presentations**: Organizers can create new presentations by assigning:
  - A title.
  - One or more speaker(s).
  - A track.
  - Start time and duration.
- **Editing Presentations**: Details of existing presentations can be modified.

## Synchronizing content with Sessionize

![Synchronize from Sessionize](/images/spreaview-conferences-details-sessionize.png)

Sessionize is a platform that allows conference organizers to select speakers and set up a schedule for their conference. SpreaView seamlessly integrates with Sessionize and allows you to synchonize your SpreaView conference data with Sessionize. It is important to understand that when setting up this synchronization, Sessionize is leading and SpreaView only downloads information from Sessionize. [On this page](/docs/integrations/sessionize/) you can learn how to set up Sessionize to allow the synchronization. This leaves you with a Session API Id. Enter this ID on the details page of your SpreaView conference to enable the Syncronize button. Click this button to synchronize the session data with Sessionize's data.

> When importing data from Sessionize, the default presentation time is not respected. The full date and time schedule as imported from Sessionize is used instead.

Note that when the Sessionize API Id is populated, also a short email template will be shown at the bottom of the screen. The email template text can be used when you communicate with your speakers from Sessionize. By default, **SpreaView does not keep speaker email addresses** so SpreaView cannot send emails to your speakers. Sessionize can, and by using the adjustable template as shown, you create a seamless experience for your speakers.

## Summary

The **Conference Content** section is a vital tool for organizing and structuring conferences in SpreaView. By allowing organizers to manage speakers, tracks, and presentations effectively, SpreaView ensures that conferences are flexible yet maintain consistent and accurate data. Note the restrictions in place to avoid accidental data loss or conflicts when managing these components.

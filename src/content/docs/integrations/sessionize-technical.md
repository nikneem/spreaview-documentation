---
title: "Sessionize (Technical)"
linkTitle: "Sessionize (Technical)"
weight: 2
categories: [Terms, Sessionize, Integration]
tags: [terms, docs, sessionize]
description: How the Sessionize import works under the hood
---

SpreaView integrates with Sessionize to streamline the process of importing event data, such as speakers, rooms, and sessions. This technical documentation explains how to set up the integration, configure your Sessionize account, and ensure that all necessary data is successfully imported into SpreaView.

## Prerequisites

Before starting the import process, make sure you have:

- A **Sessionize API ID** [(you’ll need to create this in Sessionize)](/docs/integrations/sessionize/).
- Your event's schedule in **Sessionize Schedule Builder** fully created and set to **Published**. If the schedule is not published, Sessionize will not expose the data through the API, and the import will fail.

### Ensure Your Schedule is Built in Sessionize

To successfully import data from Sessionize, you need to ensure that your event schedule is fully built and configured in the **Sessionize Schedule Builder**.

#### Using the Sessionize Schedule Builder:

1. **Access Schedule Builder**: In your Sessionize event, go to the **Schedule Builder** tool.
2. **Assign Sessions to Rooms**: Make sure that all sessions are assigned to specific rooms and have clear start and end times. This is essential, as the rooms and sessions will be imported based on this information.
3. **Speakers Linked to Sessions**: Ensure that each session has its speakers properly assigned, as this data will also be imported into SpreaView.

### Publish the Schedule in Sessionize

The most critical step before importing data into SpreaView is ensuring that the schedule in Sessionize is **Announced**. If the schedule remains in draft form, Sessionize will not expose the session, room, or speaker data through its API, and as a result, the import will fail.

![Sessionize settings](/images/sessionize-schedule-announced.jpg)

### Importing Data into SpreaView

Once your event is set up, one of the event properties is to enter the Sessionize API ID. When you enter the Sessionize API ID (only the ID, not the entire URL), a button `Sync Sessionize` is enabled. SpreaView will import all data from sessionize when every time you click that button.

#### Steps to Import Data:

1. **Log in to SpreaView**: Navigate to the SpreaView platform and log in with your account.
2. **Navigate to the Event Settings**: Select the event where you want to import data.
3. **Start the Import**: Once the API ID is entered, click **Sync Sessionize**. SpreaView will connect to Sessionize and retrieve all relevant event data, including:
   - **Speakers**: All speakers associated with the sessions.
   - **Rooms**: All rooms assigned to sessions in the schedule.
   - **Sessions**: All sessions, including their schedule, room assignments, and associated speakers.

### Verifying Imported Data

After the import process is completed, it’s important to verify that all data has been imported correctly.

#### What to Check:

1. **Speakers**: Ensure that all speakers from the Sessionize event have been successfully imported and linked to their respective sessions in SpreaView.
2. **Rooms**: Verify that all rooms created in the Sessionize Schedule Builder have been imported and are properly associated with the correct sessions.
3. **Sessions**: Check the sessions to confirm that they have the correct start and end times, room assignments, and speaker information.

### Troubleshooting Common Issues

If you encounter any issues during the import process, here are some common problems and solutions:

- **Unpublished Schedule**: If no sessions are imported, ensure that the schedule in Sessionize is **Published**. Unpublished schedules will not be exposed via the API.
- **Incorrect API ID**: Double-check that the Sessionize API ID you entered is correct. If the API ID is incorrect, SpreaView will not be able to retrieve your data.
- **Missing Data**: If some sessions or rooms are missing, verify that all sessions in the Sessionize Schedule Builder are fully assigned to rooms and have scheduled times.
- **Incorrect Dates**: Note that the SpreaView will **only** import sessions from your schedule, that are planned within the timespan of your event. This allows you to create more SpreaView events for a single Sessionize event, for example when you're organizing a MeetUp with multiple event dates. You can now easily filter all sessions that are not planned for a specific MeetUp occasion by setting the proper MeetUp start- and end date.

## Conclusion

Integrating Sessionize with SpreaView makes it easier to manage event data by importing speakers, rooms, and session information automatically. By ensuring your Sessionize event schedule is properly built, published, and using the correct API ID, you can streamline the process of setting up events in SpreaView. This integration helps reduce manual data entry and ensures consistency between platforms.

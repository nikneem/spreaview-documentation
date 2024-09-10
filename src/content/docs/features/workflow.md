---
title: "Workflow"
linkTitle: "Workflow"
weight: 1
categories: [Features, Workflow]
tags: [docs]
description: Getting started with SpreaView from A to Z
---

SpreaView is designed to streamline the process of managing events, sessions, and collecting reviews from attendees. This documentation outlines the high-level workflow of SpreaView, from registration through managing event data to gathering feedback and analyzing session performance. Below, you’ll find a step-by-step guide to using SpreaView effectively, whether you’re an organizer or a speaker.

## 1. Registration Process

The first step in using SpreaView is registering on the platform. Users must create an account, which serves as the foundation for accessing the various features of SpreaView.

- **How to Register**: Navigate to the SpreaView homepage and click on the "Get Started" button. You will be prompted to log in, or create a new account. Provide basic details such as your name, email address, and a password.
- **Account Setup**: Once registered, you can set up your profile and begin managing your events or participating as a speaker.

## 2. Creating an Organization

An **organization** in SpreaView acts as a container for all the events you manage. Before creating events, you need to establish an organization.

- **Create an Organization**: After registration, go to the "Organizations" section and click "Create" Provide a name and any other relevant details.
- **Purpose of Organization**: The organization is used to group events under a single entity, making it easier to manage multiple events and track performance across them. Also, you can invite others to take part of your organization allowing multiple persons to maintain your events and event data withing SpreaView.

## 3. Adding Speakers

Speakers are the individuals responsible for delivering sessions at your event. You can either manually add speakers or import them from an external platform like Sessionize.

- **Manually Add Speakers**: Navigate to the "Speakers" section and click "Create" Input the speaker's name, and optionally the URL to a picture.
- **Import Speakers from Sessionize**: If you are using Sessionize, you can import speakers by providing your **Sessionize API ID**. SpreaView will automatically pull in the speaker data, more on the sessionize importe further in this document.

## 4. Creating an Event

Once the organization and speakers are set up, the next step is creating an event. Events are containers for sessions, and you can also organize sessions by room within the event.

- **Create Event**: In the "Events" section, click "Create Event." Provide the event's name, start and end dates, and any other pertinent details.
- **Multiple Rooms**: You can assign multiple rooms to an event if it takes place in various locations (physical or virtual). This allows multiple sessions to run concurrently.
- **Sessions**: Sessions can be created manually or imported using the Sessionize integration.

## 5. Importing Speakers, Rooms, and Sessions from Sessionize

SpreaView supports direct integration with **Sessionize**, allowing you to import speakers, rooms, and sessions seamlessly.

- **Sessionize API ID**: To integrate Sessionize with SpreaView, you will need to enter your **Sessionize API ID** in the appropriate field within SpreaView. For detailed information on the Sessionize API ID settings, check the [how to create a Sessionize API ID](/docs/integrations/sessionize/) documentation.
- **Automatic Import**: Once the API ID is entered, SpreaView will enable the `Sync Sessionize` button, that allows you to import all related data, including speakers, rooms, and sessions, from your Sessionize account. This ensures that your event data remains consistent across platforms.

## 6. Downloading QR Codes for Sessions

Each session in SpreaView is assigned a unique review URL, which can be accessed via a QR code. This QR code makes it easier for attendees to access the review page and submit feedback.

- **Download Session QR Code**: Go to the "Sessions" tab within the event, select a session, and click "QR Code", to download the QR Code for that session. The QR code links directly to the review page for that session.
- **Download all QR Codes**: Alternatively you can download the QR code of all sessions at once, with the `Download QRs` button in the toolbar of the events page, once the details of an event are opened.
- **Encourage Attendees**: Display the QR code during the session, either in slides or printed materials, to encourage attendees to scan and provide feedback.

## 7. Speaker Dashboard

SpreaView provides a dedicated **Speaker Dashboard** for each speaker, allowing them to manage their session reviews and feedback independently.

- **Accessing the Speaker Dashboard**: Once a speaker is assigned to a session, they can log in to SpreaView and access their personalized dashboard.
- **Downloading Session QR Code**: Speakers can download the QR code for their own sessions directly from their dashboard.
- **Review Report**: After the event, speakers can download a report summarizing the reviews and feedback they received for each session. This report includes performance data based on attendee ratings in categories such as content, delivery, and interaction.

> You can access the speaker dashboard using the technical ID of a speaker, or the technical ID of the external system, when a user is imported from external systems like Sessionize. The URL for the speaker dashboard is https://spreaview.com/speaker-dashboard/{SPEAKER_ID} where the `{SPEAKER_ID}` must be replaced with the actual tecnical ID of the speaker.

## 8. Event Review Dashboard for Organizers

SpreaView also provides an **Event Review Dashboard** for organizers. This dashboard aggregates data from all sessions in the event and provides valuable insights into overall session performance. The dashboard will become available when the event was started.

- **Session Performance Overview**: The dashboard shows key metrics for each session, including average ratings, attendance, and feedback trends.
- **Compare Session Data**: Organizers can compare sessions to identify which topics, speakers, or presentation styles were most successful, helping them plan future events more effectively.
- **Exporting Data**: The event review data can be exported as a report for further analysis or sharing with stakeholders.

> Tiles and tables with data on the Event Review Dashboard are cached. Therefore, refresing the page may result in the same view over a timespan of 5 minutes. The tiles are live tile that refresh automatically when the server-side cached value expires, to automcatically show the new value.

## Conclusion

The SpreaView workflow is designed to facilitate seamless event and session management while streamlining the process of collecting and analyzing session feedback. From registration and organization creation to the importing of data from external platforms like Sessionize, SpreaView offers a comprehensive suite of tools for event organizers and speakers. By encouraging the use of QR codes and utilizing dashboards for real-time feedback, SpreaView ensures that all participants—organizers, speakers, and attendees—benefit from detailed insights that can enhance the quality of future events.

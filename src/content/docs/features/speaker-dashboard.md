---
title: "The Speaker Dashboard"
linkTitle: "Speaker Dashboard"
weight: 4
categories: [Features, Productivity, Speakers, Dashboard]
tags: [docs]
description: Providing insights to your speakers
---

The **SpreaView Speaker Dashboard** is a dedicated portal that allows speakers to manage their session reviews, download session-specific QR codes, and access reports on the feedback they receive. This dashboard consolidates all engagements for a speaker within a SpreaView organization, making it a centralized tool for speakers who participate in multiple events under the same organization.

## Accessing the Speaker Dashboard

The Speaker Dashboard is accessible via a specific URL format:

```
https://spreaview.com/speaker-dashboard/{organization-id}/{speaker-id}
```

- **{organization-id}**: This is the unique identifier for the organization that is hosting the event.
- **{speaker-id}**: This is the unique identifier for each speaker within the organization.

When a speaker is invited to view their dashboard, they will see a list of all events they've been involved in within that organization. This includes the ability to download session-specific QR codes and review reports once a session is concluded.

### Accessing Speaker Dashboard URLs in SpreaView

When you open the details of a speaker in the SpreaView platform, the **Speaker Details Dialog** will display the exact URL for that speaker’s dashboard. This unique URL provides direct access to the speaker’s dashboard, where they can download session QR codes, access review reports, and manage their sessions. By presenting the specific URL in the details dialog, event organizers can easily share the dashboard link with speakers, ensuring they have quick access to their personal dashboard without needing to manually construct the URL. This feature simplifies the process of distributing dashboard access to multiple speakers.

### Speaker Dashboard PIN Code Mechanism

To enhance security and provide controlled access, the **SpreaView Speaker Dashboard** requires speakers to create a unique **6-character PIN code** when they first access their dashboard. Upon visiting the dashboard URL for the first time, speakers will be prompted to set this PIN code, which will serve as their primary method of authentication. Once the PIN is created, it must be used every time the speaker accesses their dashboard, ensuring secure and easy access to session data and review reports. This mechanism adds an additional layer of protection, while still allowing for quick access to the speaker's information in future logins.

![Entering pincode](/images/spreaview-speaker-dashboard-pincode.jpg)

> Pincodes are hashed with a unique seed per speaker. Only the hash is stored in our data store.

### Accessing Through Sessionize Integration

If you are using **Sessionize** to manage your speakers and sessions, you can leverage an undocumented feature in Sessionize to send dashboard access URLs automatically to your speakers.

- **URL Template**: Use the following URL template when sending emails to speakers through Sessionize:

  ```
  https://spreaview.com/speaker-dashboard/{organization-id}/{SPEAKER_ID}
  ```

  - Replace the `{organization-id}` with your actual SpreaView organization ID.
  - Leave the `{SPEAKER_ID}` token as is. Sessionize will automatically replace it with the correct speaker ID for each speaker in the system.

This integration allows for seamless communication with speakers and simplifies the process of granting access to their dashboard without manually creating individual URLs.

## Features of the Speaker Dashboard

### 1. Downloading Session QR Codes

On the speaker dashboard, speakers can download a **QR code** for each of their sessions. These QR codes are critical for collecting reviews from attendees. Speakers can only download their session QR code prior to their session. When the session has started according to the schedule, the QR buttons change in a download button that can be used to download an evaluation report.

- **QR Code Purpose**: The QR code directs attendees to the review page for the session, allowing them to provide feedback during the **review window**.
- **Review Window**: The QR code will only lead to an active review page when the review window for the session is open. It is important that speakers display or distribute the QR code during or at the conclusion of their session to encourage attendees to submit their feedback.

#### How to Download the QR Code:

1. Log in to the **Speaker Dashboard**.
2. Find the session for which you need the QR code.
3. Click on the "Download QR Code" button associated with that session.

### 2. Accessing Session Review Reports

After a session concludes, speakers can access the **session review report**, which contains the feedback collected from attendees. This report provides valuable insights into how the session was received and offers areas for improvement.

- **Report Details**: The review report includes ratings in the following categories:
  - **Speaker**: How well the speaker delivered the content.
  - **Content**: The relevance and quality of the session’s content.
  - **Delivery**: The effectiveness of the speaker’s delivery method.
  - **Interaction**: How well the speaker engaged with the audience.
  - **Optional Comments**: If enabled, free-text comments from attendees are also available for review.

#### How to Download the Review Report:

1. Log in to the **Speaker Dashboard**.
2. Select the session for which the report is available.
3. Click the "Download Report" button to retrieve the session review summary.

### 3. Managing Multiple Events

One of the key features of the Speaker Dashboard is the ability for speakers to view all of their engagements across multiple events within the same organization. This means that if the same speaker is invited to deliver sessions at different events, they will be able to manage and view reports for all of these sessions from one centralized dashboard.

- **Event Listings**: The dashboard will display a list of all events that a speaker is involved in, with individual sessions under each event.
- **Session Data Across Events**: Speakers can access and download QR codes and reports for each session, no matter how many different events they are participating in under the same organization.

## Conclusion

The SpreaView Speaker Dashboard offers an easy-to-use, centralized platform for speakers to manage their sessions, gather feedback, and download review reports. With integration options for Sessionize, the process of inviting speakers and sharing session review tools is streamlined and automated, making it easier for organizers to facilitate feedback collection and for speakers to enhance their presentations based on real attendee input.

By encouraging speakers to use the QR codes and reports available through their dashboard, conference organizers and speakers alike can ensure a more interactive and feedback-rich experience for all event participants.

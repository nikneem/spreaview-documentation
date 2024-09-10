---
title: "Session Management"
linkTitle: "Session Management"
weight: 2
categories: [Features, Productivity, Sessions]
tags: [docs]
description: Managing sessions and understanding what you can control
---

Sessions are a central component of the SpreaView platform, providing a structured way to organize and manage the content of your event. Whether you're entering sessions manually or importing them from an external system, SpreaView offers a range of properties that you can control to ensure that each session is accurately represented and managed within your event. This documentation page will guide you through each property of a session in SpreaView and explain how these properties function differently depending on whether a session is manually created or imported.

To view the list of sessions planned for an event, navigate to the Events page in SpreaView. Select the desired event to open its details and click on the Sessions tab. This will show a list of sessions planned for the given event, and allows you to edit the sessions and/or add new sessions to the event manually.

## Session Properties

When managing sessions in SpreaView, you have control over several key properties that define the session's content, schedule, and speakers. Here's a detailed description of each property:

### 1. **Session Title**

- **Description**: The session title is the name of the session as it will appear in the event schedule and other related materials. It should be concise and clearly communicate the topic or focus of the session.
- **Control**: When entering a session manually, you can freely edit the session title at any time before the event. However, if the session is imported from an external system, the session title is locked and cannot be edited within SpreaView. This ensures consistency with the source system.

### 2. **Abstract**

- **Description**: The abstract provides a brief summary or overview of the session's content. It helps attendees understand what to expect from the session and decide whether it aligns with their interests.
- **Control**: Similar to the session title, the abstract can be edited when the session is created manually. If the session is imported, the abstract becomes immutable in SpreaView to maintain consistency with the information provided by the external system.

### 3. **Room**

- **Description**: The room property indicates the specific location or virtual space where the session will take place. This could be a physical room in a venue or a virtual meeting link for online events.
- **Control**: Similar to the session title, the room can be edited when the session is created manually. If the session is imported, the room becomes immutable in SpreaView to maintain consistency with the information provided by the external system.

### 4. **Start Date and Time**

- **Description**: The start date and time specify when the session is scheduled to begin. This information is critical for ensuring that the event runs smoothly and that attendees know when to attend each session.
- **Control**: For manually created sessions, you can set and adjust the start date and time as needed. However, for imported sessions, this property is fixed and cannot be edited within SpreaView. This restriction ensures that the session timing remains consistent with the original schedule from the external system.

### 5. **Review Period Start Date and Time**

- **Description**: The review period start date and time determine when attendees can begin submitting reviews for the session. This period usually starts as soon as the session is started. Do no schedule the review start period too late as there are occasions when attendees want to review a session while is is not concluded yet. For example when an attendee leaves the session, you want to allow this attendee to leave feedback.
- **Control**: You have full control over setting and editing the review period start date and time, regardless of whether the session was created manually or imported. This flexibility allows you to decide when feedback collection should begin, ensuring it aligns with the event's flow and attendee experience. By default the session review period starts exactly when the session starts, and remains open for a certain amount of hours (default is 24).

### 6. **Speakers**

- **Description**: The speakers are the individuals who will be delivering the session. This property lists the names and possibly the affiliations of the presenters, giving attendees insight into who will be leading the session.
- **Control**: For manually entered sessions, you can select and modify the speakers as needed. However, for sessions imported from an external system, the speaker information is locked and cannot be edited. This ensures that the speaker details remain accurate and consistent with the data from the external source.

## Manual Entry vs. Importing Sessions

### 1. **Manual Session Entry**

When sessions are entered manually in SpreaView, you have complete control over all the properties of the session. This includes the ability to:

- Set and modify the session title, abstract, and speakers at any time before the event.
- Assign and adjust the room and start date and time as needed.
- Determine the appropriate time to open the review period for attendee feedback.

Manual entry is ideal for events where you have flexibility and need to make adjustments up until the event date.

### 2. **Imported Sessions**

Sessions can also be imported from an external system, such as Sessionize, which streamlines the process of populating your event schedule with existing data. However, to maintain consistency with the external system:

- The session title, abstract, speakers, and start date and time are locked and cannot be edited in SpreaView.
- Only the room assignment and the review period start date and time remain editable within SpreaView.

This approach ensures that the data remains consistent across platforms and reduces the risk of discrepancies between the original session information and what is displayed in SpreaView. Changes to sessions or their schedule should be applied in the external system. In SpreaView you can synchronize the session information to retrieve the changes made in the external system. This synchronization process is idempotent. The session code (and therefore the review URL) of a session will never change after its initial creation.

## Conclusion

Managing sessions in SpreaView is designed to be flexible yet consistent, allowing you to either create sessions from scratch or import them from external systems while maintaining the integrity of critical session details. Understanding how each session property functions and the limitations imposed by importing sessions will help you effectively organize and manage your event, ensuring a smooth and well-coordinated experience for all participants.

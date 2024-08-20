---
title: "Sessions"
linkTitle: "Sessions"
weight: 5
categories: [Sessions, Getting Started]
tags: [docs]
description: Session management
---

In SpreaView, [sessions](/docs/terms/session/) are the core activities that take place during an event. A session can be anything from a keynote speech, a panel discussion, a workshop, or any other structured presentation or activity that occurs within the event. Each session is scheduled in a designated room and is organized under a specific event. SpreaView offers tools to manage these sessions effectively, including integration options for importing session data and features for collecting attendee feedback.

## Structure of Sessions in SpreaView

### 1. **Sessions within Events**

- **Event Association**: Every session in SpreaView is linked to a specific event. This organizational structure ensures that sessions are properly grouped and managed within the context of the overall event.
- **Room Assignment**: Each session is scheduled to take place in a specific room. This assignment helps in organizing the event’s flow and ensuring that there is no overlap in session timings within the same room.

### 2. **Session Scheduling**

- **Start and End Date/Time**: Each session is scheduled with a precise start and end date and time. This scheduling is crucial for managing the event’s timeline and ensuring that attendees know when and where each session will occur.
- **Real-Time Updates**: Any changes to the session schedule, such as time adjustments or room changes, are reflected in real-time across all platforms where the session information is displayed.

## Session Code and Review Feature

### 1. **Session Code**

- **Unique Identifier**: Upon creation, each session is assigned a unique session code. This code is immutable, meaning it remains constant for the lifetime of the session. The session code serves as a key identifier for accessing various session-related features within SpreaView.
- **Accessing the Review Page**: The session code is particularly important for feedback collection. By navigating to the following URL, attendees can leave reviews for the session:

  ```
  https://spreaview.com/review/{session_code}
  ```

  Replace `{session_code}` with the specific code assigned to the session. This page allows attendees to provide ratings and feedback, which are crucial for evaluating the session's success and identifying areas for improvement.

### 2. **Review Process**

- **Review Categories**: On the review page, attendees can rate the session based on several categories, such as Speaker, Content, Delivery, and Interaction, using a 1 to 5-star scale.
- **Optional Comments**: There is an option to enable a free text field where attendees can leave additional comments or detailed feedback about their experience during the session.
- **Feedback Collection Window**: Reviews can only be submitted during the designated review window set by the event organizers.

## Integration with External Platforms

### 1. **Session Data Import**

SpreaView supports the integration with external platforms like Sessionize, making it easier for event organizers to manage their sessions.

- **Sessionize Integration**: Through this integration, session data—including titles, descriptions, speaker information, and scheduling details—can be imported directly into SpreaView.
- **Seamless Syncing**: This feature ensures that all session information is up-to-date and accurately reflected in SpreaView without the need for manual data entry.

### 2. **Benefits of Integration**

- **Efficiency**: Saves time and reduces the risk of errors associated with manual data entry.
- **Consistency**: Ensures that session information is consistent across different platforms and accessible to all attendees.

## Managing Sessions in SpreaView

### 1. **Creating Sessions**

Sessions can be created manually within SpreaView or imported from an external platform:

- **Manual Creation**: Enter the session details, including title, description, speakers, start and end times, and room assignment.
- **Session Code Assignment**: Once the session is created, SpreaView automatically assigns a unique session code.

### 2. **Editing Sessions**

- **Schedule Adjustments**: Organizers can edit session details, such as adjusting the timing, changing the room, or updating the session description.
- **Real-Time Updates**: Any changes made are reflected in real-time across the event’s schedule and attendee information portals.

### 3. **Session Visibility**

- **Public Room View**: The details of each session, including the schedule and location, are visible to attendees through the Public Room View feature, making it easy for participants to plan their event experience.

## Use Cases

- **Multi-Track Events**: Organizers can manage multiple sessions across different tracks and rooms, ensuring that all sessions are properly scheduled and accessible.
- **Feedback Collection**: The built-in review system allows for easy feedback collection, helping speakers and organizers assess the effectiveness of their sessions.

## Conclusion

Sessions are the building blocks of any event in SpreaView. With tools for scheduling, room assignment, feedback collection, and integration with platforms like Sessionize, SpreaView provides a comprehensive solution for managing sessions efficiently. The unique session code and review feature make it easy to gather valuable insights from attendees, helping to ensure that every session contributes to the overall success of the event.

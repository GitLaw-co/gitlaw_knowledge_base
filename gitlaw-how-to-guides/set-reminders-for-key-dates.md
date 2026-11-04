---
title: Set reminders for key contract dates
slug: set-reminders-for-key-dates
category: gitlaw-how-to-guides
excerpt: 'Keep track of renewal deadlines, expiry dates, and payment milestones by creating reminders in GitLaw - manually or automatically from dates extracted when you upload a contract.'
---

Never miss a renewal window or payment deadline. GitLaw lets you attach reminders directly to documents and contacts, sends you an email when the date arrives, and groups everything by urgency so you can see what needs attention at a glance.

### Create a reminder manually

1. **Open Notifications** from the left sidebar. Reminders and actions are listed here, grouped by when they are due.

   ![The Notifications page with reminders grouped into Overdue and Upcoming, and the + button at the top right](https://git.law/kb-images/set-reminders-for-key-dates/notifications-list.png "ring: 97 1.5 3 11")

2. **Click +** at the top right. The **New action** form opens.
3. **Describe what needs doing** (for example, "Acme MSA renewal").
4. **Pick when to be reminded:** **Today**, **Tomorrow**, **In a week**, or **Pick date & time** for a specific date and time. Leave **No reminder** to track the action without a reminder.
5. **Add a note** (optional) for any context you want included.
6. **Link a contact or document** (optional) with **Add contact** or **Add document**, so the reminder appears on their detail views.
7. **Choose who to notify:** **Only the assignee**, **All members**, or **Specific people**. Everyone on that list receives the reminder email.
8. **Click Add.** GitLaw emails the chosen recipients when the reminder date is reached.

   ![The New action form with reminder options and who to notify](https://git.law/kb-images/set-reminders-for-key-dates/new-action.png "ring: 4 26 91 9; ring: 4 77.5 40 12")

### How reminders are organised

Reminders are grouped into four buckets:

| Group         | What it means                                   |
| ------------- | ----------------------------------------------- |
| **Overdue**   | Due date has passed and not yet marked complete |
| **Today**     | Due today                                       |
| **This week** | Due later this week (after today)               |
| **Upcoming**  | Due beyond this week                            |

Completed reminders are kept separately and do not appear in the urgency groups unless you turn on **Show completed**.

### Recurring reminders

When you mark a recurring reminder complete, GitLaw automatically schedules the next occurrence - you do not need to recreate it. Recurrence ends either on an end date you specify or after a maximum number of occurrences. If you set neither, the reminder repeats indefinitely.

### AI-suggested reminders from uploaded contracts

When you [import a Word or PDF contract](/knowledge-base/import-a-word-or-pdf-contract), GitLaw extracts key dates - expiry, renewal, and execution dates - and can create reminders from them automatically. Automatically created reminders are tagged **inferred** so you can distinguish them from reminders you added yourself. To confirm an inferred reminder, open it and save any edit (or use the explicit confirm action); the inferred tag is removed and the reminder is treated as fully user-owned from that point.

### Reminders on a contact

If a reminder is linked to a document, and that document is associated with a contact, the reminder also appears on the **Notifications** tab of the [contact's detail view](/knowledge-base/manage-your-contacts). This gives you a single place to see every upcoming deadline related to a counterparty.

### Mark a reminder complete

Open the reminder and click **Mark as complete**. For recurring reminders, this schedules the next occurrence. For one-off reminders, it moves the item to your completed list.

### Edit or delete a reminder

Open any reminder to change its name, due date, note, linked documents, linked contacts, or recurrence. To remove it entirely, choose **Delete** from the reminder detail.

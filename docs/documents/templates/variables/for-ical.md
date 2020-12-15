---
# This basic template provides core metadata fields for Markdown articles on docs.superoffice.com

# Mandatory fields.
title: variables_for_ical       # (Required) Very important for SEO. Intent in a unique string of 43-59 chars including spaces.
description: Variables for appointments corresponding to the iCal standard # (Required) Important for SEO. Recommended character length is 115-145 characters including spaces.
author: {github-id}             # Your GitHub alias.
keywords:
so.topic: reference           # article, howto, reference, concept, guide
# Optional fields. Don't forget to remove # if you need a field.
# so.envir:                     # cloud or onsite
# so.client:                    # online, web, win, pocket, or mobile
---

# Variables for appointments corresponding to the iCal standard

| Variable | Description |
|----------|-------------|
| bate | Formatted list of people invited to an appointment, created for iCal<br/>ATTENDEE;RSVP=TRUE;CN="First Invited":MAILTO:;PARTSTAT=ACCEPTED<br/>ATTENDEE;RSVP=TRUE;CN="Test Testesen":MAILTO:test@superoffice.com;PARTSTAT=TENTATIVE |
| bpat | The main feature of the appointment's repeating pattern, formatted like the Daily pattern "FREQ=DAILY;", for example |
| bprt | The priority of the appointment, converted to iCal format: our 1 = iCal 9, our 2 = iCal 5 (default), our 3 = iCal 1 |
| brul | The entire appointment's repeating pattern, formatted as "RRULE:" + bpat + bsub + bunt |
| bsub | The secondary feature of the appointment's repeating pattern, formatted as the sub-pattern Daily Workday "BYDAY=MO,TU,WE,TH,FR;", for example |
| bsun | The start of the week for the appointment's repeating pattern, formatted as "WKST=SU" or "WKST=MO" |
| btzr | The time zone rule for standard time, for the PC's local time. Formatted as RRULE:FREQ=YEARLY;WKST=MO;INTERVAL=1;BYMONTH=3;BYDAY=4SU |
| btzu | The time zone rule for summer time, for the PC's local time. Formatted as RRULE:FREQ=YEARLY;WKST=MO;INTERVAL=1;BYMONTH=10;BYDAY=4SU |
| buid | Unique ID created for iCal. SerialnoDfollowupIdDinvitedId (where D is a separator). For example, 1010000014D345D971. Only for follow-ups with several participants |
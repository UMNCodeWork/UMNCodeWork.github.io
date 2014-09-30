---
layout: video_event
title: This is a past video event
category: past_events

start_time: 3pm
end_time: 4pm
location: University of Minnesota; Room 123, STSS
event_link: //www.youtube.com/embed/18uDutylDa4

excerpt: This is the event excerpt. It is the place where you can write up a few details about the event to display on the main events page.

---

## Video event basics
This is a video event.  The event date is parsed from the file name, so be sure to structure your file name as follows:

*"2014-MM-DD-title-of-event.markdown"*

This event features a Hangout/YouTube video.  Add the link to your video in the event_link listed in the frontmatter above. Be sure to grab the YouTube embed link *without* the "http"/"https".  Just plain backslashes "//" will suffice!  This event also automatically includes an embedded IRC Chat pointing to the #UMNCodework channel for use during the live broadcast.


### Creating upcoming events
When you create an event, be sure to include the "upcoming_events" category in the frontmatter.  This will make sure the event is displayed under "Upcoming events" on the events main page.  Let's try to keep only 1-2 events featured under "Upcoming events" at any given time.  To publish an event to the "Upcoming events" section, do the following:

1. Make sure the category in the frontmatter is listed as "upcoming_events"

2. Add the file to the "_posts/events/upcoming" folder 

For the rest of our events, feel free to add them to the Google Calendar and create drafts of the event pages to "keep in the queue" before we make them live on the main events page.  Store these draft events in "_drafts/events/upcoming".



### Managing past events
When an event is completed, do the following:

1. Change its category in the frontmatter from "upcoming_events" to "past_events"

2. Move the file into the "_posts/events/past" folder

A past event can still include a start_time and end_time, but these will no longer display on the main events page (as they are no longer relevant).

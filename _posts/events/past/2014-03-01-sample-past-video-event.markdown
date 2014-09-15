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

This event features a Hangout/YouTube video.  Add the link to your video in the event_link listed in the frontmatter above. Be sure to grab the YouTube
embed link *without* the "http"/"https".  Just plain backslashes "//" will suffice!  This event also automatically includes an embedded IRC Chat pointing to the
#UMNCodework channel for use during the live broadcast.


### Managing past events
This event occurred in the past.  When an event is completed, do the following:

1. Change its category in the frontmatter from "upcoming_events" to "past_events"

2. Move the file into the "_posts/events/past" folder

A past event can still include a start_time and end_time, but these will no longer display on the main events page (as they are no longer relevant).

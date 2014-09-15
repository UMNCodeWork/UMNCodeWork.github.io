---
layout: video_event
title: This is an upcoming video event
category: upcoming_events

start_time: 10:30am
end_time: 11:30am
location: University of Minnesota; Room 321, Northrop
event_link: //www.youtube.com/embed/TBIL2sdfoVc

excerpt: This is the event excerpt. It is the place where you can write up a few details about the event to display on the main events page.

---

## Video event basics
This is a video event.  The event date is parsed from the file name, so be sure to structure your file name as follows:

*"2014-MM-DD-title-of-event.markdown"*

This event features a Hangout/YouTube video.  Add the link to your video in the event_link listed in the frontmatter above. Be sure to grab the YouTube
embed link *without* the "http"/"https".  Just plain backslashes "//" will suffice!  This event also automatically includes an embedded IRC Chat pointing to the
#UMNCodework channel for use during the live broadcast.


### Creating upcoming events
This event is an upcoming event.  When you create an event, be sure to include the "upcoming_events" category in the frontmatter.  This will make sure the event is displayed under "Upcoming events" on the events main page.  Let's try to keep only 1-2 events featured under "Upcoming events" at any given time.

For the rest of our events, feel free to add them to the Google Calendar and create drafts of the event pages to "keep in the queue" before we make them live on the main events page.  Store these draft events in "_drafts/events/upcoming".


### Managing past events
Once an event is completed, remember to do the following:

1. Change its category in the frontmatter from "upcoming_events" to "past_events"

2. Move the file into the "_posts/events/past" folder

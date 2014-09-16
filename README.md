# UMNCodeWork Public Webpage on GitHub

## Technology stack:
* GitHub Pages + [Jekyll](http://jekyllrb.com/)
* [Zurb Foundation](http://foundation.zurb.com/) (CSS Version)

## Site structure:
This is the basic site structure.  When editing the site, *only* add files to the _drafts folder
(for draft content) and _posts folder (for published content).  *Do not* touch any of the other
files or you may change or break the overall site structure!

```
UMNCodeWork.github.io
├── _config.yml
├── _site
├── _includes
|   ├── footer.html
|   ├── header.html
|   └── nav.html
├── _layouts
|   ├── blog.html
|   ├── default.html
|   ├── novideo_event.html
|   ├── project.html
|   └── video_event.html
├── css
├── images
├── js
├── index.html
├── contact.html
├── events.html
├── project.html
├── Gemfile

**DO NOT EDIT ABOVE THIS POINT; can edit anything below this point**

├── _drafts
|   ├── blog
|       └── YYYY-MM-DD-draft-blog-post.markdown
|   ├── events
|       ├── past
|           └── YYYY-MM-DD-draft-past-event.markdown
|       └── upcoming
|           └── YYYY-MM-DD-draft-upcoming-event.markdown
|   └── projects
|       └── YYYY-MM-DD-draft-project.markdown
├── _posts
|   ├── blog
|       └── YYYY-MM-DD-blog-post-title.markdown
|   ├── events
|       ├── past
|           └── YYYY-MM-DD-past-event-name.markdown
|       └── upcoming
|           └── YYYY-MM-DD-upcoming-event-name.markdown
|   └── projects
|       └── YYYY-MM-DD-project-name.markdown
```

**Don't forget to structure your file names correctly when adding content!** All post files must be titled with the year/month/day and post name, separated by dashes (-).  They must also end with the filetype '.markdown' to parse correctly.  For example:
```
YYYY-MM-DD-post-name.markdown
```
(Note: Draft events don't need a year/month/day until they're published.)


## Templates:

### Blog posts
######Where do I save them?
- _drafts/blog for drafts
- _posts/blog for published

######Where do they show up on the live site?
On the "Home" page. They are interspersed with other post types (events & projects), and all posts are then organized by the post date indicated in their file name.

######What template should I use?
```
---
layout: blog
title: Blog title goes here
category: blog

author: < optional; will default to "University of Minnesota Codework Collaborative" >

excerpt: Put a brief excerpt here to display on the Home page
---

Put your content here.  You can write it in Markdown, and Jekyll will parse it into HTML markup.

```



### Video events
######Where do I save them?
- _drafts/events/upcoming for drafts of upcoming events
- _posts/events/upcoming to publish upcoming events (let's try to keep only 3-4 events featured in the "upcoming" folder at a time; save them in drafts until they're ready to publicize)

######What template should I use?
```
---
layout: video_event
title: Event title goes here
category: < upcoming_events | past_events > <--! Choose one of these!

start_time: HH:MMam/pm
end_time: HH:MMam/pm
location: Room name, building name, etc. goes here
event_link: //www.youtube.com/embed/TBIL2sdfoVc <--! Grab the "embed" link from YouTube

excerpt: Put a brief excerpt here to display on the Home & Events pages
---

Put your content here.  You can write it in Markdown, and Jekyll will parse it into HTML markup.

```


### Non-video events
######Where do I save them?
- _drafts/events/upcoming for drafts of upcoming events
- _posts/events/upcoming to publish upcoming events (again, let's try to keep only 3-4 events featured in the "upcoming" folder at a time; save them in drafts until they're ready to publicize)

######What template should I use?
```
---
layout: novideo_event
title: This is an event without a video
category: < upcoming_events | past_events > <--! Choose one of these!

start_time: HH:MMam/pm
end_time: HH:MMam/pm
host: < optional; be sure to add something here if it is an *external* host to give them credit! >
location: user-readable location data goes here
map_address: Google Maps-readable address data goes here

excerpt: Put a brief excerpt here to display on the Home & Events pages
---

Put your content here.  You can write it in Markdown, and Jekyll will parse it into HTML markup.

```


### Projects
######Where do I save them?
- _drafts/projects for draft project descriptions
- _posts/projects for published project descriptions

######What template should I use?
```
---
layout: project
title: Project title goes here
category: projects

number: 1 <!-- This needs to be a unique number, so make sure to count up from the last project on the list and increment by 1
contact: Contact name and any other contact info goes here

excerpt: Put a brief excerpt here to display on the Home page, and in a summary box next on the Projects page

---

Put your content here.  You can write it in Markdown, and Jekyll will parse it into HTML markup.

```


## Edit the site:
Clone the UMNCodeWork.github.io repository to your computer.  You should only need to clone the repository once to your local computer; after that, be sure to keep the code stored in the same directory you originally downloaded it to, as this directory will remain linked to the proper GitHub origin.  

###To preview edits:
You can write drafts, make edits, and add posts to the _drafts and _posts directories on your local computer.  To preview your changes, navigate to the UMNCodeWork.github.io directory in the command line on your local computer.  From within that directory, execute the `jekyll server` command.  This will compile the changes and spit out the "full" HTML into the _site directory.  You can preview the changes in a browser at http://localhost:4040.

(Note: It may be tempting to dig in and start editing the _site directory--**DON'T**!  This is an unstable directory that is constantly being written and over-written "on the fly" by Jekyll.  Make all your changes within the _posts and _drafts directories, and leave Jekyll alone to do its thing with _site.)

###To deploy changes:

1. When done editing, open your terminal and `cd` into the UMNCodeWork/UMNCodeWork.github.io directory
2. `git status` should indicate that you have unstaged changes in the directory
3. `git add --all`
4. `git commit -m "Your update message goes here"`
  *Your update message should just be a brief statement of what you added or changed. For example:
  "Added blog post" or "Added upcoming event on YYYY-MM-DD" or "Moved event on YYYY-MM-DD to past events folder"
5. `git push -u origin master`

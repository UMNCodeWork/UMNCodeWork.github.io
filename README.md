# UMNCodeWork Public Webpage on GitHub

## Technology Stack:
* GitHub Pages + [Jekyll](http://jekyllrb.com/)
* [Zurb Foundation](http://foundation.zurb.com/) (CSS Version)

## Site structure:
This is the basic site structure.  When editing the site, *only* add files to the _drafts folder
(for draft contnet) and _posts folder (for published content).  *Do not* touch any of the other
files or you may change or break the overall site structure!

```
.
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
|       └── YYYY-MM-DD-sample-blog-post.markdown
|   ├── events
|       ├── past
|           └── YYYY-MM-DD-sample-past-event.markdown
|       └── upcoming
|           └── YYYY-MM-DD-sample-upcoming-event.markdown
|   └── projects
|       └── YYYY-MM-DD-sample-project.markdown
├── _posts
|   ├── blog
|       └── YYYY-MM-DD-sample-blog-post.markdown
|   ├── events
|       ├── past
|           └── YYYY-MM-DD-sample-past-event.markdown
|       └── upcoming
|           └── YYYY-MM-DD-sample-upcoming-event.markdown
|   └── projects
|       └── YYYY-MM-DD-sample-project.markdown
```

## Templates:

### Blog posts
####Where do I save them?
- _drafts/blog for drafts
- _posts/blog for published

####Where do they show up on the live site?
On the "Home" page. They are interspersed with other post types (events, projects), all organized by post date.

####What template should I use?




### Video events
####Where do I save them?
- _drafts/events/upcoming for drafts of upcoming video events
- _posts/events/upcoming to publish upcoming video events (let's try to keep only 3-4 events featured in the "upcoming" folder at a time; save them in drafts until they're ready to publicize)

####Where do they show up on the live site?
On the main "Events" page under the "Upcoming events" header.  They are also aggregated with all of the other
posts in the "What's New?" section of the "Home" page.

##What template should I use?


### Non-video events
####Where do I save them?
- _drafts/events/upcoming for drafts of upcoming video events
- _posts/events/upcoming to publish upcoming video events (again, let's try to keep only 3-4 events featured in the "upcoming" folder at a time; save them in drafts until they're ready to publicize)

####Where do they show up on the live site?
On the main "Events" page under the "Past events" header.  They are also aggregated with all of the other posts in the "What's New?" section of the "Home" page.

####What template should I use?


### Projects
####Where do I save them?
- _drafts/projects for draft project descriptions
- _posts/projects for published project descriptions

####Where do they show up on the live site?
On the main "Projects" page.  They are also aggregated with all of the other posts in the "What's New?" section of the "Home" page.

####What template should I use?


## Deploy changes:
Clone the UMNCodeWork.github.io repository to your computer.  You should only need to clone the repository once to your local computer; after that, be sure to keep the code stored in the same directory you originally downloaded it to, as this directory will remain linked to the proper GitHub origin.  

###To preview edits:
You can write drafts, make edits, and add posts to the _drafts and _posts directories on your local computer.  To preview your changes, navigate to the UMNCodeWork.github.io directory in the command line on your local computer.  From within that directory, execute the `jekyll server` command.  This will compile the changes and spit out the "full" HTML into the _site directory.  You can preview the changes in a browser at http://localhost:4040.

(Note: It may be tempting to dig in and start editing the _site directory--**DON'T**!  This is an unstable directory that is constantly being written and over-written "on the fly" by Jekyll.  Make all your changes within the _posts and _drafts directories, and leave Jekyll alone to do its thing with _site.)

###To deploy changes:

1. When done editing, open your terminal and 'cd' into the UMNCodeWork/UMNCodeWork.github.io directory
2. `git status` should indicate that you have untracked changes in the directory
3. `git add --all`
4. `git commit -m "Your update message goes here"`
  *Your update message should just be a brief statement of what you added or changed. For example:
  "Added blog post" or "Added upcoming event on YYYY-MM-DD" or "Moved event on YYYY-MM-DD to past events folder"
5. `git push -u origin master`

# UMNCodeWork Public Webpage on GitHub

## Technology Stack:
* GitHub Pages + [Jekyll](http://jekyllrb.com/)
* [Zurb Foundation](http://foundation.zurb.com/) (CSS Version)

## Site structure:
This is the basic site structure.  When editing the site, *only* add files to the _drafts folder (for draft contnet) and _posts folder (for published content).  
*Do not* touch any of the other files or you may change or break the overall site structure!

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


## Templates:

### Blog posts
**Where do I save them?**

**Where do they show up on the live site?**

**What's the template look like?**


### Video events
**Where do I save them?**

**Where do they show up on the live site?**

**What's the template look like?**


### Non-video events
**Where do I save them?**

**Where do they show up on the live site?**

**What's the template look like?**


### Projects
**Where do I save them?**

**Where do they show up on the live site?**

**What's the template look like?**


## Deploy changes:

**To connect to the GitHub repository where our site is housed:**

You should only need to clone the repository once to your local computer.  Be sure to keep the code
stored in the same directory you originally downloaded it to, as this directory will remain linked
to the proper GitHub origin.  

**To preview edits:**
You can make edits and add posts on your local computer.  To preview your changes, navigate to the
UMNCodeWord.github.io directory in the command line on your local computer.  Once you are withing the
directory, execute the `jekyll server` command.  You can preview in a browser at "http://localhost:4040".  


**To deploy changes:**

1. Open your terminal and 'cd' into the UMNCodeWork/UMNCodeWork.github.io directory
2. Edit, add, or delete posts in the _drafts (unpublished) or _posts (published) folder
3. git add --all
4. git commit -m "Your update message goes here"
  *Your update message should just be a brief statement of what you added or changed. For example:
  "Added blog post" or "Added upcoming event on YYYY-MM-DD" or "Moved event on YYYY-MM-DD to past events folder"
5. git push -u origin master

# AutoCHERI Project Site

This is the source for the site hosted at https://autocheri.tech

Note that this source is PUBLIC, so can be viewed by any github users.

# Developing the site

This site should be developed on your local machine and tested using the local Ruby webserver. It is easy once the pre-reqs are installed.

## Setup Ruby and Jekyll

Follow the steps: https://jekyllrb.com/docs/ , which will: 
1. install ruby via chruby
1. install jekyll via the gem

## Run it

Once all pre-reqs are installed, simply: 

1. `bundle install`
1. `bundle exec jekyll serve --livereload`
1. Browse to http://localhost:4000

## Deploy it

1. Open a PR and commit your changes.
1. Get approval from SecureTCU team members.
1. Once pushed, Github Pages will build and deploy your changes to the live site.

## Troubleshooting

#### "no acceptor (port is in use or requires root privileges)" [Windows Subsystem for Linux]

Sometimes you may get the following when starting serve: `Error:  no acceptor (port is in use or requires root privileges)`. This means that jekyll process is already running, using the port. Kill it with:

`ps aux | grep jekyll | awk '{print $2}' | xargs kill -9`


#### “The GitHub API credentials you provided aren’t valid.”

When trying to run jekyll serve you may see this error.

This can be due to having 2-factor authentication set up on github, or the credentials not stored otherwise. The easiest fix for this is to generate a unique Personal Access token through github’s website, and store that in the JEKYLL_GITHUB_TOKEN environment variable.

See this post: http://blog.johannesmp.com/2017/02/13/fixing-jekyll-serve-on-windows/


# Improvements

1. Add a table of contents to index.md using [Jekyll TOC](https://heymichellemac.com/table-of-contents-jekyll)
1. Add some more content
1. Use a nicer template
1. More
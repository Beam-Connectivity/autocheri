# Run it

Follow the steps: https://jekyllrb.com/docs/

or if all pre-reqs are installed, simply: 

1. `bundle exec jekyll serve --livereload`

2. Browse to http://localhost:4000


# Troubleshooting

Sometimes you may get the following when starting serve: `Error:  no acceptor (port is in use or requires root privileges)`. This means that jekyll process is already running, using the port. Kill it with:

`ps aux | grep jekyll | awk '{print $2}' | xargs kill -9`


# Improvements

1. add some content
1. Use a nicer template
1. More
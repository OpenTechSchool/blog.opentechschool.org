# Blog of OpenTechSchool

## Technical stuff
The blog is hosted on github using [jekyllbootstrap](http://jekyllbootstrap.com). In order to use it locally, you need to have jekyll installed.

## Running locally
Just pull the latest updates and run

    jekyll --server --auto

and you'll have the server running locally on port 4000

## Publishing process

### Creating a new post

You can create a new blog post by using the handy rake command:

 rake post title="My title"

this will create a new Markdown file with the current date and your
title in the \_posts direcotry. This filename is also the url the user
can see later, so please use something understandable there :) .

### Understanding the post file

The post file contains a header in yaml format. You can change the title
and description, category and tags are not widely used on our blog as of
now.

In order to have a nice "teaser" in the front-page you might want to
consider adding that in the yaml header, otherwise the whole post will
be shown. See \_posts/2012-08-20-new-workshop-introduction-to-python.md for 
an example.

Everything following the line with three dashes ("---") is considered
"the content" of the post and will be shown on the singel-page-view. The
content (as well as the teaser) can and shall be written as Markdown and
in special occasion may contain some html.

Please see http://daringfireball.net/projects/markdown/syntax for an
more eloquent understanding of markdown

### Publishing the post

Once you've created the post and cross read it within the browser, you
can submit it via a pull-request to the main repository. It will then be
cross-read and approved by the content team, who are the only ones
allowed to publish on the main repository.




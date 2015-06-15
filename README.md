# How This Blogging Stuff Works

To give commands, first change the directory to your site. It's at `~/Code/touching-research`.

    $ cd ~/Code/touching-research

Then, you can give commands.

## Preview your site

    $ hexo s -d

The `-d` option also displays your drafts. To exit this, press CTRL+C. You can always keep this window open while you're writing posts, as it will reload your webbrowser when you make a change. If you want to check out what it looks like on your phone or a tablet, give the command `ifconfig` in the terminal, and write down your IP address that's displayed after 'inet addr'. In our case, it's 192.168.178.18. On your phone, after giving the `hexo s` command, open 192.168.178.18:4000 to preview your website.

## Create a new draft

    $ hexo new draft "This is the title of my post"

This puts a new file in the `_drafts` folder.

## Publish a draft

    $ hexo publish this-is-the-title-of-my-post

This moves the draft from the `_drafts` folder into the `_posts` folder. When specifying the name, watch the lowercase and the dashes.

## Create a new post

    $ hexo new post "This is the title of my post"

This creates a new post without creating a draft.

## Create a new page

    $ hexo new page "This is the title of my page"

A new page is like a new post, only it won't show up as a post on the front page. It's for static information, such as an about page.

## Writing stuff

A post, or a draft, or a page, are all written in markdown. On top of the page you can see a couple things, followed by three dashes. This is called YAML. It can contain some information about the page or post, such as date published, date updated, title, tags, layout, etc.

The dates are written in socalled ISO8601 format.
date: YYYY-MM-DD HH:MM:SS
date: 2015-06-03 10:26:33

## Clean the site

    $ hexo clean

This deletes the generated site. Do this if you run into any sort of problem. You can always regenerate it.

## Generate your website

    $ hexo g

This creates your website, and prepares it to be published.

## Deploy!!!

    $ hexo d

The moment of truth, send your wisdom into the world, off to the interwebs! DEPLOYYY!!!

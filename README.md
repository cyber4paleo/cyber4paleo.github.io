# cyber4paleo.github.io

<img src="c4pcdw.jpg" width="100">

## Description

This repository was set up in advance of the Cyber4Paleo Community Development Workshop.  The repository aims to act both as a location to store critical documentation and to operate as a model for project Best Practices (as best it can).  The website is developed using a bare-bones [Jekyll](http://jekyllrb.com) implementation and a simple Pages interface (as opposed to a blog implementation).  This set up is designed to help encourage collaboration by Workshop participants through GutHub, for posterity.

This site can be accessed directly from [cyber4paleo.github.io]()

## Contribution

Simon Goring - \[cre, aut\] [GitHub](http://github.com/SimonGoring) [Twitter](http://twitter.com/sjgoring)

This site is open to contribution from all workshop participants, pursuant to the [Code of Conduct](http://contributor-covenant.org/version/1/3/0/).

## Initialization

The website is developed using Jekyll.  You run and edit the site locally, first fork (then clone) or clone the repository locally:

```
git clone https://github.com/cyber4paleo/cyber4paleo.github.io
# Develop the site from a local branch:
git checkout -b add_pages
```

Now you can create content locally from the branch<sup>[1](#footnote1)</sup> `add_pages`.  To implement your changes locally (and to see the webpage through your browser) you need to run Jekyll:

```
jekyll serve
```

Then open your browser to `http://127.0.0.0:4000`.  Depending on the programs you have installed, this port (`4000`) may be in use by other applications (TomTom was interfering with mine).  If this happens you can change the [Serve Command Options](http://jekyllrb.com/docs/configuration/#serve-command-options), *e.g.*, `jekyll serve --port 5000`.

One of the nice things about `jekyll serve` is that it continues to watch the website directory.  Jekyll will continue to re-build the site as you make changes to the website Markdown and HTML files.  As Jekyll rebuilds you can simply return to your browser and re-load the page.  This change is usually pretty fast -- `CTRL-S` in your text editor, `TAB` to the browser and then `F5` to reload.

## Commiting, Merging & Pushing

Once you are happy with your changes you need to merge your branch back into the `master`.  Before you do this it always helps to check that your `master` branch is up to date.

To go back to the `master` branch -- and to make your changes go live to the World Wide Web -- you need to merge your changes in the `add_pages` branch back into the `master` branch.

```
git checkout master
git pull
git merge add_pages
git status
git add --all
git commit -m "Edits to our groups' sections, the Group_Wonder pages."
git push
```

Maybe a more descriptive commit message, but regardless, you're on the web!

<a name="footnote1">1</a>: For more on branching and merging you can check this [git tutorial](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging).

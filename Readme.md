# Empirica Website

This Emptirica Website is built with [Hugo](https://gohugo.io/).

## Build

First get the theme which is added as a submodule:

```
> git submodule sync
> git submodule update --init
```

Then build:

```
> hugo
```

To run a local server while updating the website, run:

```
> hugo server -D
```

## Deploy

The website is deployed as a static Firebase website. It happens automatically
on push of the `master` branch. See `circle.yml` for details.

## Updating the website

Most content is Markdown in the `content/` directory, and works as a normal Hugo
website. See the [Hugo Documentation](https://gohugo.io/content-management/) for
details about editing the content.

For the home page and shared parts of the website (such as the footer), you will
need to edit the HTML in the `layouts/` directory. Any custom CSS should be
added to `static/css/custom.css`

If you need to add images, as much as possible, please avoid using binary
formats (JPNG, PNG, ...) and prefer SVG.

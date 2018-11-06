# About
This Jekyll site is meant as a demo to illustrate how a typical site can be created with Jekyll. It features a mix of developer friendly features such as Galleries and File List built from the file system, along with CMS like editing that a client can login and update content.

# Features at a Glance
- Gulp.js modern build allows for SASS/SCSS and JS processing.
- Fast live reloading local development with Browser Sync
- Homepage that lets developers go wild!
- Use partials/includes for re-useable content such as calls to action that is easy to maintain.
- Dynamic pages from .CSV files that are easy for clients to manage
- Image gallery built from images in the file system. Developers simply add an image to a folder and the gallery is updated.
- Netlify CMS integration allows editing pages as well as creating News.
- Contact form uses Netlify Forms to receive submissions which can be piped to other services
- Use Jekyll _data to output content like variables across multiple pages, making content data easy to maintain.

# Getting started
- run `bundle` to install dependencies
- run `npm install` to install npm modules
- run `gulp` to start live development


## SCSS and JS
The theme and JS files are located in the /assets/* folder. Gulp will process these files and build the sites CSS and JS files.


## Netlify CMS Integration
The Netlify CMS edits the YAML files in _data along with the _posts folder for the sites News. By allowing the Netlify CMS to edit only the _data files, you are free to use advanced markup on the rest of the site pages, and to pull in Netlify CMS content you simply tell Jekyll to output {{ site.data.home.title }}.

Each .html page will need a corresponding .yml file that the Netlify CMS will edit. This allows the freedom to use any markup and not being limited to markdown.

This site also uses some 'Global' yaml files that can be edited which multiple pages use such as a business address or phone number. So only one Global file needs updated, and the rest of the site is updated.

News can be created by the Netlify CMS similar to a blog example, which creates markdown files in the _posts directory.



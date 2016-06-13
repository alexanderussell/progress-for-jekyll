# Progress

Progress was built by [Alexander Russell](http://alexanderussell.org) and inspired by [Cody House's](https://codyhouse.co/) [Reading Progress Indicator](https://codyhouse.co/demo/reading-progress-indicator/index.html). The folks over at Cody House are pretty fantastic and are making some awesome things. They're also super responsive to comments, so head on over there and check out what they've been doing. 

Progress features a quick and simple environment that is set up so users can input all the necesarry info in the config file and start blogging. Further reiterations are in progress to turn this into a Wordpress theme or make it fully editable with Cloudcannon CMS. I cannot let you resell this unless you [contact me](mailto:alex@collectivelymade.com).

If you'd like give credit somewhere on your blog or tweet a shout out to
[@alexanderussell](https://twitter.com/alexanderussell), that would be pretty sweet. 

If you feel like donating — [Give it a thought.](https://flattr.com/profile/alexanderussell)



## Features:
- flexible, uses max-width for responsive goodness
- beautiful reading progress indicator courtesy of [CodyHouse](https://codyhouse.co/)
- retina images using @2x
- post loop showing 5 posts per page
- archive for posterity sake

## Basic Setup

1. [Install Jekyll](http://jekyllrb.com) if you haven't already.
2. Download this bad boy.
3. Fork the [Progress repo](http://github.com/alexanderussell/progress-for-jekyll/)
4. Twerk it out so it's just for you.
5. ???
6. Profit

## [Preview the Theme](http://alexanderussell.github.io/progress-for-jekyll)
<br>

``` bash
progress-for-jekyll/
├── data
|    ├── navigation.yml  //an array of navigation items for easy editing
├── _includes
|    ├── _footer.html  //site footer
|    ├── _head.html  //site head
|    ├── _header.html  //header for navigation and logo/title
|    ├── _share-post.html  //share buttons
├── _layouts
|    ├── default.html  //all the bare necessities
|    ├── page.html  //page layout
|    └── post.html  //post layout
├── _posts
├── css  //preprocessed styles. good idea to minify
├── img  //images and graphics used in css and js
├── js
|   ├── jquery-2.1.4.js  //jQuery for the win.
|   ├── main.js  //jQuery plugins and settings for the progress indicator.
|   └── modernizer.js  //modernize it, yo.
├── images  //images for posts and pages
├── about.md  //about page
├── archive.md  //lists all posts from latest to oldest organized by date
└── index.html  //homepage. lists 5 most recent posts w/ pagination
```

# Customization

### _config.yml

Most of the variables found here are used in the .html files found in `_includes` if you need to add or remove anything. A good place to start would be to change the title, tagline, description, and url of your site. When working locally comment out `url` or else you will get a bunch of broken links because they are absolute and prefixed with `{{ site.url }}` in the various `_includes` and `_layouts`. Just remember to uncomment `url` when building for deployment or pushing to **gh-pages**...

### Owner/Author Information

Change your name, bio, Twitter url, email, Dribbble URL, etc.

### Top Navigation Links

Edit page/post titles and URLs to include in the site's navigation. For external links use "external: true".

``` yaml
# sample top navigation links
links:
  - title: About Page
    href: /about
  - title: Other Page
    href: /other-page
  - title: External Page
    href: http://alexanderussell.org
    external: true
```
<br>

## Other Stuff

The rest is just your average Jekyll config settings. Nothing too crazy here...

### _includes

For the most part you can leave these as is since the author/owner details are pulled from `_config.yml`. That said you'll probably want to customize the copyright stuff in `_footer.html` to your liking.

### Adding Posts and Pages

There are two main content layouts: `post.html` (for posts) and `page.html` (for pages). Pages span the full-width of the content, while posts leave space for related posts and the reading progress indicator when on the longform view.



## License

This is free to use, fork, do whatever you want. Please *do not* sell this design though. You don't need to link me to it, but please contact me if you intend to market this theme. I am releasing premium versions of this design for select CMS's. 
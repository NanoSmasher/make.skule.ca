M.A.K.E. Website theme
======================

Website derived from [Jero's freelancer theme](https://github.com/jeromelachaud/freelancer-theme) which is in turn based on the [Freelancer bootstrap theme](http://startbootstrap.com/templates/freelancer/). This means I used Twitter Bootstrap just like every other website these days.

The website is currently being hosted by the [UofT Skule M.A.K.E. Club](http://make.skule.ca). Check it out!

Managing the website
====================

## Overview of site

Jekyll is a static site builder that use:

 - Liquid Templating System
 - Markdown Post Rendering
 - A League Of Legends (lol)

The home page or **index.html** looks like this:

```
---
layout: default
---
```

Not very informatative huh? What it actually does is to read and cpoy the contents of the **/_layouts/default.html** file instead. That file asks jekyll to use the files found in **/_includes**, with a couple of extra tags thrown in.

Each subfile in **/_includes** contains a section of html code. But here's the catch; since you are still reading it from the **/index.html** the base path is "**/**" hence why all my images seem to work. Otherwise, most of the code is really nice to manage.

The **style.css** file is processed exactly the same way as the **index.html** file.

### Editing the site

Luckily, there is very little you need understand to actually change it up. All you need to focus on is the **_posts** and **img** folder, as well as the **_config.yml** file.

 - **_posts** hold all the events. Just follow the format.
 - **img** is also self-explanatory. Make sure the images are the correct dimensions/file names.
 - **_config.yml** is self-explanatory as well, but there is alot of things you can change. They include:
   - Description of website
   - Front page news bulletin
   - List of sponsors
   - List of team members and more

### Setting up is as easy as 1, 2, 3!

 1. Install Ruby, RubyDevKit, and Jekyll. Windows users can just download [Portable Jekyll](https://github.com/madhur/PortableJekyll/releases) and run setpath.cmd. (It's about one 1GB!)
 2. Go to the root folder where **index.html** is found and type in:

    ```
    jekyll build
    ```
 3. FTP (or manual copy files one by one) everything in the **_site** folder to wherever you want. It wil most likely be the **/public_html** folder.

Voila! Thanks for reading ~ Nanosmasher

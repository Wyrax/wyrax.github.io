Jekyll: Live reload on Windows 10
03 Apr 2018 • Jekyll
Live reload issue solved when running Jekyll on Windows 10.
Issue
When attempting to use live reload on Windows 10 (jekyll serve --livereload), encountered the following error,

Unable to load the EventMachine C extension; To use the pure-ruby reactor, require "em/pure_ruby"
C:/tools/ruby24/lib/ruby/gems/2.4.0/gems/eventmachine-1.2.5-x64-mingw32/lib/rubyeventmachine.rb:2:in `require': cannot load such file -- 2.4/rubyeventmachine (LoadError)
        ...
Solution
From the Ruby command prompt,

gem uninstall eventmachine
gem install eventmachine --platform ruby

Freelancer Jekyll theme  [![Build Status](https://api.travis-ci.org/jeromelachaud/freelancer-theme.svg?branch=master)](https://travis-ci.org/jeromelachaud/freelancer-theme/) 
=========================

Jekyll theme based on [Freelancer bootstrap theme ](http://startbootstrap.com/template-overviews/freelancer/)

## How to use
 - Place a image in `/img/portfolio/`
 - Replace `your-email@domain.com` in `_config.yml` with your email address. Refer to [formspree](http://formspree.io/) for more information.
 - Create posts to display your projects. Use the follow as an example:
```txt
---
layout: default
modal-id: 1
date: 2020-01-18
img: cabin.png
alt: image-alt
project-date: January 2020
client: The Client
category: Web Development
description: The description of the project

---
```

## Demo
View this jekyll theme in action [here](https://jeromelachaud.com/freelancer-theme)

## Screenshot
![screenshot](https://raw.githubusercontent.com/jeromelachaud/freelancer-theme/master/screenshot.png)

---------
For more details, read the [documentation](http://jekyllrb.com/)

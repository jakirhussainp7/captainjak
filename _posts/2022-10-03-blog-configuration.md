---
tags: blog jekyll gh-pages
title: Setup a website using Jekyll, gh-pages
---
This post can be used as a how-to guide in setting up a new static website using [Jekyll](https://jekyllrb.com/) and [Github](https://github.com) Pages.
## Jekyll on Linux
### What is Jekyll?

Jekyll is a simple static website generator that is maintained by volunteers and contributors all around the world. It converts text written in the markup language and uses layouts to create a website.  You can tweak around the configuration default [_config.yml](https://jekyllrb.com/docs/configuration/) file to make the site look & feel displayed on the page.  
To install Jekyll on a Linux machine you need the below dependencies installed.

[Ruby](https://www.ruby-lang.org/en/downloads/), Ruby Gems, GCC, and Make 

Check the versions `ruby -v`, `gem -v`, `gcc -v`, `g++ -v` and `make -v`

Install Jekyll and bundler gems. 
```
gem install jekyll bundler
``` 

and start the server 
```
bundle exec jekyll serve
``` 

you can browse the site locally at [http://localhost:4000](http://localhost:4000)

## Minimal-Mistakes

This site built upon the theme [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) from Github. Thanks to its creators and developers for maintaining this code so clean & easy to modify.
There are three easy methods to install this theme into your environment. Using `gem` method and `remote theme` and fork the repo into your github account.
For detailed instructions please look into [README.md](https://github.com/mmistakes/minimal-mistakes/blob/master/README.md) file. 

## Notice box
This box represents the notice label for the paragraph. This can be achieved by adding the tag `{: .notice--info}` at the next line. 
And there are other related notice tags are `{: .notice--warning}` , `{: .notice--danger}` , `{: .notice--success}` can be used to mention type of the message.
{: .notice--info}



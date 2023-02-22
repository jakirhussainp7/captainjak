---
tags: blog jekyll gh-pages
title: Setup a website using Jekyll, gh-pages
---
This post can be used as a how-to guide in setting up a new static website using [Jekyll](https://jekyllrb.com/){:target="_blank"} and [Github](https://github.com){:target="_blank"} Pages.

## Jekyll on Linux

### What is Jekyll?

Jekyll is a simple static website generator that is maintained by volunteers and contributors all around the world. It converts text written in the markup language and uses layouts to create a website.  You can tweak around the configuration default [_config.yml](https://jekyllrb.com/docs/configuration/) file to make the site look & feel displayed on the page.  
To install Jekyll on a Linux machine you need the below dependencies installed. Most of the packages will come pre-installed in your Linux machine. 

[Ruby](https://www.ruby-lang.org/en/downloads/){:target="_blank"}, Ruby Gems, GCC, and Make 

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

This site built upon the theme [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes){:target="_blank"} from Github. Thanks to its creators and developers for maintaining this code so clean & easy to modify.
There are three easy methods to install this theme into your environment. Using `gem` method and `remote theme` and fork the repo into your github account.
For detailed instructions please look into [README.md](https://github.com/mmistakes/minimal-mistakes/blob/master/README.md){:target="_blank"} file. 

I downloaded the zip file and opened the file in a test environment using the editor [PyCharm](https://www.jetbrains.com/pycharm/){:target="_blank"}. There are many text editors out there to use like [Sublime Text](http://www.sublimetext.com/){:target="_blank"}.
I prefer using PyCharm. I linked my GitHub repository account to PyCharm using the [tokens](https://github.com/settings/tokens){:target="_blank"}. Whatever edits I made here in the Pycharm, I can push them to my repo to publish the site.
Before pushing the commit to GitHub, I test the site performance in my local development environment [http://localhost:4000](http://localhost:4000).

## Configuration
Minimal-mistakes theme configured with all plug-ins, arrays, font awesome,and layouts in the file _config.yml. I tweaked the file a bit to add new features like dark/light themes.
Used [Fork-Awesome CDN](https://forkaweso.me/Fork-Awesome/get-started/){:target="_blank"}  into `_include/head/custom.html` for the fonts and latest icons.
I tweaked the file a bit to add new features like dark/light themes by following the discussions [#2033](https://github.com/mmistakes/minimal-mistakes/discussions/2033){:target="_blank"}. Used Fork-Awesome CSS  into _include/head/custom.html for the fonts and latest icons. 

Pages, Posts, Layouts, Headings, Images, Quotes, Commands, Syntax mentions, Twitter embeds, Video links, and Markup changes are briefly explained by the author on his [test site](https://mmistakes.github.io/minimal-mistakes/year-archive/){:target="_blank"}. I removed the footer follow section by uncommenting the tags in `_include/footer.html` 

## Notice box
This box represents the notice label for the paragraph. This can be achieved by adding the tag `{: .notice--info}` at the next line.
And there are other related notice tags are `{: .notice--primary}``{: .notice--warning}` , `{: .notice--danger}` , `{: .notice--success}` can be used to mention type of the message.
{: .notice--primary}

>This text represents the 'quote' section. 

## gh-pages
After making the necessary changes to the blog, now it's time to host the site in [GitHub](https://github.com){:target="_blank"}. Create a public repository and push the site files to the repo using Pycharm. GitHub pages are available for public repositories for free. I hosted my static website on GitHub using the `gh-pages` under the repo settings page.  
There is detailed document provided my Github to host sites using [Jekyll on gh-pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll){:target="_blank"}.
Gh-pages provides a workflow to convert markdown languages file to `.html` using the Jekyll-workflow under the `Actions` tab in your repo.

That's it. Now website ready, visit using the link `https://username.github.io/reponame`
A Custom domain can be used to forward traffic. Configure the GitHub domain name servers in the domain registrar `A` records. 

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
Managing a custom domain on github pages can be found [here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain){:target="_blank"}. 


**Author's Note:** This blog started out as a manuel or rather a brain dump of my process. Well I've written what I wanted: a tour of the various moving pieces and each one is important to me. I think this is what I'll find valuable in the future.
{: .notice--info}






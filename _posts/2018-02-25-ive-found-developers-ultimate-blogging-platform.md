---
layout: post
title: I've Found Developer's Ultimate Blogging Platform
# image: "/assets/images/x.jpg"
date: '2018-02-25 16:48:50'
tags:
- misguiding-guides
- in-english
comments: true
---

A few months ago I was looking for a platform to help me write and publish useless writings, such as this one you're reading right now.

I've used Blogger in my high school days, writing nonsense that I'm now still kind of ashamed at. It was pretty customizable, but it was undoubtedly too Blogger-ish no matter what you do. Plus, its admin interface was too bloated for my need and at times too confusing to use.

I've tried Wordpress when it was _the_ go-to platform if you want to create a blog. It suffers from the same sentiment from what I feel about Blogger; too many features and thingies that just got in the way of writing and publishing. I believe it's better suited as a proper content management system for running a full-blown website rather than a simple daily entries like what I'm trying to do.

I've tried Tumblr when it was one of the coolest things online (it maybe still is today, although now it serves a more niche segment). Still, there was something that I felt is quite not right, perhaps it's because I'm using it in a wrong way. At the end of the day, I'm not convinced to commit using it full-time.

I once considered to use Medium, but I felt like my writing are not the ones suited for Medium-caliber publishing. I just want to babble around, not caring how people would react or racing for claps and highlights. I've seen some poor Medium writings, and they quite offended me because I feel how out of place they are. Just like how Quora is now beginning to be filled with homework questions.

For a while I've decided to stick with Ghost, a platform from one of the former lead at Wordpress who thought that it was the way of how a blogging platform should be from the get-go. Out of all that I've used, I prefer Ghost for its ridiculously minimal yet usable interface, straightforwardness, and ease of use. Using Markdown, it was as if its only purpose of existence is to write and publish blogs or longforms.

It was almost perfect for my need, and I run it on an OpenShift instance for a few months before they ditched the free plan. While I was preparing to setup a VPS instance to re-host my blog, I was looking for other options, just in case there is free alternative that match or exceed Ghost's capabilities.

_Turns out there is_. I stumbled upon Jekyll, the blogging platform created by GitHub's co-founder Tom Preston-Werner. It is definitely not new, hot-kid-on-the-block stuff (in fact, it was first released in 2008, long before I even knew what a terminal was). Whenever I was trying to give it a look and maybe a spin, I was always scared by how hard to understand the installation instructions are for average Joe to use it.

I'm not sure if that's truly the case or perhaps I'm just too lazy to try back then - hopefully the latter one - but all in all, it took me probably just a few hours to set it up in production, import all of my previous blog entries, and customize it to my liking - at least on the level that you might not notice it _is_ a community-made template.

Jekyll is not a CMS, and aptly-described as a "static site generator". That means it will take input files (in this case, HTML template along with CSS and Markdown or other text-based content) and will generate a fully-navigable, static HTML site ready to upload for you. All you have to do is prepare a Ruby development environment, install Jekyll, generate a new site, and run a command to serve the site or publish for production.

Here's a few reasons why I believe it's a good blogging platform that is better suited for developer, although nothing stops you and them for using it (apart from initial learning curve).

1. Completely customizable. If you want to go the extra mile, you can literally create the whole website by yourself, only for Jekyll to handle the boring, dynamic part for you. There's something you want to change from the template you are using? No problem, just override it. Adding analytics script? Easy peasy, just add it in the footer file. Need commenting functionalities? Disqus comes to the rescue.

2. After initial setup, almost zero maintenance is required; no software updates, no database upgrade, or anything complicated necessary. Why? Because unlike CMS, which requires constant update to prevent security holes, any site generated with Jekyll is pure HTML, so practically nothing can hack it (unless, of course, you're getting DDoS attack). If there is an update in Jekyll, the structure of content or the site that you generate probably won't have to change much, or at least easy to migrate.

3. Jekyll is, by design, file-based, which means it can be easily tracked with a version control (and with it, advanced file versioning). Image upload is also rather easy, and in fact, you don't have to to: just put the image in asset folder and link it from the Markdown content.

4. Extremely easy GitHub Pages integration. In another words, you can have free, custom-domain hosting for life just by putting your content on a GitHub repo. GitHub will even automatically generate the site for you with every commit you push. This is a technical advantage that simply no other solutions could ever provide.

While some might not like its Ruby-based environment or admittedly high learning curve for those not who are not technically-inclined, those are not the case for me. Until I decided to write something more meaningful and publish it on Medium, I'll keep this personal blog alive with Jekyll for days to come.

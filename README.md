howtopuppet
===========

howtopuppet.com - FAQ site for Puppet and related technologies

What
----
This is intended to be a curated, up-to-date, _linkable_ repository for common
questions and explanations, errors, and patterns.

Why
---

There's so much information out there about Puppet. And given how quickly the language has evolved over the
past few years, a lot of it is outdated, sub-optimal, or flat-out wrong with modern (let's say 3.x+) Puppet.
I'm not the most active member of #puppet or the mailing lists, but I try to keep up on what's going on. And
more and more, I see people asking the same questions, running into the same issues, and reproducing the same
anti-patterns. So, I figured that a nice, condensed place to store some pointers would be nice.

There are plenty of wonderful references out there about Puppet. Even though I've been using Puppet for a while,
when I type "d" into my browser URL bar, [docs.puppetlabs.com](http://docs.puppetlabs.com/) is usually the first
option. There's also a [Get Help](http://puppetlabs.com/community/get-help) page with links to great resources
such as the [puppet-users google group](http://groups.google.com/group/puppet-users), [FAQs](http://docs.puppetlabs.com/guides/faq.html),
[#puppet](http://webchat.freenode.net/?channels=puppet) on Freenode, and the [ask.puppetlabs.com](http://ask.puppetlabs.com/)
Q&A site. This isn't intended to replace any of them. This is intended to be a curated, up-to-date, _linkable_
repository for common questions and explanations, errors, and patterns.

Contributing
------------

1. [Fork the repository](https://github.com/jantman/howtopuppet/fork)
2. check out the ``gh-pages`` branch
3. make your changes (see below)
4. Optionally (but recommended) test locally (see below)
5. Submit a pull request

Adding a Post
-------------

Because of some limitations in how Jekyll works, dates have to be in the post filename.

1. Figure out which category you're adding your post in.
2. Copy ``post-template.md`` to a new file under ``_posts/categoryname`` named YYYY-MM-DD-slug.md, where
   "categoryname" is the name of the category you chose, "YYYY-MM-DD" is the date on which
   you're adding the post, and "slug" is a URL-safe, hyphen-separated version of the title of the post.
3. Fill in the metadata fields at the top of the file, and the body of the post. I've put comments within
   ">>>>" and "<<<<" that provide quick guidance on what each field should be. Be sure to add some
   useful/pertinent tags.
4. Since Jekyll __only__ does simple templating, there's no way to build short links to each post. So, grab
   the integer out of ``/next_redirect`` in the repository, put it in the redirect\_from metadata field
   on your post, and then increment the next\_redirect file.

Testing Locally
---------------

For the details, see the GitHub [Using Jekyll with Pages](https://help.github.com/articles/using-jekyll-with-pages) page.

In short:

1. Clone the repo locally
2. Checkout master
3. ``bundle install``
4. checkout the gh-pages branch (or the branch you're interested in)
5. ``bundle exec jekyll serve`` and check the content at [http://localhost:4000](http://localhost:4000)

Who
---

I'm jantman pretty much everywhere including [GitHub](https://github.com/jantman) and often in #puppet on Freenode,
or [@j_antman on Twitter](https://twitter.com/j_antman). I also have a [blog](http://blog.jasonantman.com/) with a bunch
of tech info/tips/tutorials and an occasional rant or two.

But I'm just the guy who thought of registering a cool domain name and starting this site, mainly after I found myself
(during my occasional stints of trying to be active on #puppet or the puppet-users list) helping new Puppeteers along
with the same bits of information over and over.

I'm attempting to fill the site with some useful content to start with, but this is very much intended to be
a community project.

License
-------

This site is licensed under [Creative Commons Attribution-Share Alike 3.0 United States License](http://creativecommons.org/licenses/by-sa/3.0/us/).


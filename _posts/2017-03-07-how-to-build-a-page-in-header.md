---
layout: post
title: How to build a page in header
date: 2017-03-07 21:03:30 -0600
tags: jekyll
---
`_layout` folders contains different kinds of pages in this web sites.
`_includes` folders contains `headers`, `footers`, and `icon` things. Therefore, if we want to add some pages here, we should first analyse the `head.html`, and `header.html` files here.
{% highlight ruby %}
% for my_page in site.pages %
% if my_page.title %
my_page.title | escape
% endif %
% endfor %
{% endhighlight %}
Here the `site.pages` means the markdown files in root folder. So that I recognize that if I build up a new text file, and rename as "what you-want to display on your site.md", I can add another pages in the header.
Then I open the file, and write down:

{% highlight ruby %}
---
layout: page
title: About
permalink: /about/
---
somthing you want to write down in this page.

{% endhighlight %}
The most important thing is that the `layout` style must be `page`. The title will be presented at the header of pages.

The organization of jekyll
default.html is a fundation.
home.html is based on default layout
page.html is based on default layout
post.html is based on default layout

---
layout: post
title: Copying HTML content into MadCap Flare
---

Collaboration is one of the challenges tech writers face. I avoid using MS Word as Word docs tend to pick up formatting issues as they skip from one individual to another. Confluence has become a powerful tool for colaboration, and with wiki pages,  you get a nice, simple WYSIWYG editor. I find myself collaborating a lot through wiki pages and I wanted to be able to copy text from a wiki directly into Flare. 

Skip straight to the [HTML to Flare XHTML converter](https://christalkstech.github.io/flarify).

## How it works

    
If you *CTRL+SHIFT+i*, you can copy the HTML content using developer tools.

![_config.yml]({{ site.baseurl }}/images/copyingElements.gif)

With HTML content we can get a lot of CSS that is *no bueno* for Flare. The [HTML to Flare XHTML converter](https://christalkstech.github.io/flarify) removes CSS styling and non-Flare friendly entities. You can then paste the *cleaned* content into the `<body>` of your Flare file.

![_config.yml]({{ site.baseurl }}/images/pastingElements.gif)



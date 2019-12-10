---
layout: post
title: Copying HTML content into MadCap Flare
---

Collaboration is one of the challenges we face with using an Authoring tool like Flare. 
I avoid MS Word like the plague as Word docs tend to pick up more and more formatting as they skip from one individual to another. Confluence has become a powerful tool for colaboration, and with wiki pages,  you get a nice, simple WYSIWYG editor. I find myself collaborating a lot through wiki pages and I wanted to be able to copy text from a wiki directly into Flare. 

Skip straight to the [HTML to Flare XHTML converter](https://christalkstech.github.io/).

## How it works

With wiki content we get a lot of confluence CSS that is *no bueno* for Flare.

    <tbody aria-live="polite" aria-relevant="all"><tr role="row"><td class="confluenceTd">Table Heading</td><td class="confluenceTd">14</td></tr><tr role="row"><td class="confluenceTd"> Title of something</td><td class="confluenceTd">35</td></tr><tr role="row"><td colspan="1" class="confluenceTd">Version number 12</td><td colspan="1" class="confluenceTd">28</td></tr><tr role="row"><td colspan="1" class="confluenceTd">488</td></tr></tbody>

Furthermore Flare works in XHTML (with its own madcap caveats), you can find problems with things like `&nbsp;`, for example.

The converter removes **all** CSS attributes and converts HTML entitites to be Flare friendly. You end up with just pure HTML that you can paste into the <body> of your topic.

![_config.yml]({{ site.baseurl }}/images/wiki.png)


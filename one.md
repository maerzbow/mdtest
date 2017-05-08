
---
title: About writing and formatting on GitHub
intro: {{ site.data.guides.dotcom-writing-on-github.shortdesc.about-writing-and-formatting-on-github }}
---

[Markdown](http://daringfireball.net/projects/markdown/) is an easy-to-read, easy-to-write syntax for formatting plain text.

We've added some custom functionality to create {{ site.data.variables.product.product_name }} Flavored Markdown, used to format prose and code across our site.

You can also interact with other users in pull requests, issues, and wikis with features like [@mentions](/articles/basic-writing-and-formatting-syntax/#mentioning-users-and-teams), [issue and PR references](/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests), and [emoji](/articles/basic-writing-and-formatting-syntax/#using-emoji).

{% if page.version == 'dotcom' or page.version == 'cloud' or page.version > 2.5 %}

### Text formatting toolbar
Every comment field on {{ site.data.variables.product.product_name }} contains a text formatting toolbar, allowing you to format your text without learning Markdown syntax. In addition to Markdown formatting like bold and italic styles and creating headers, links, and lists, the toolbar includes {{ site.data.variables.product.product_name }}-specific features such as @mentions, task lists, and links to issues and pull requests.

![Markdown toolbar](/assets/images/help/writing/markdown-toolbar.gif)

{% endif %}

### Further reading

- "[Basic writing and formatting syntax](/articles/basic-writing-and-formatting-syntax)"
- "[Working with advanced formatting](/articles/working-with-advanced-formatting)"
- "[Mastering Markdown](https://guides.github.com/features/mastering-markdown/)"
- "[Markdown Tutorial](http://markdowntutorial.com/)"


    var s = "JavaScript syntax highlighting";
    alert(s);
    
    return s;

A Table
=======

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

```java
            
            Optional<BlockMarker> newBlock = findStartingBlockMarker(line);

            if (newBlock.isPresent()) {
              if (!lastLineWasEmpty) {
                segments.add(seg);
                seg = new Segment();
              }

              seg.addLine(line, lineEmpty);
              actualBlock = newBlock.get();
```

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.
>
> An Empty line in a block was present

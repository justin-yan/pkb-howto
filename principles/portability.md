# Portability

Your PKB should be a lifelong companion, evolving to fit your needs and helping you solve problems. You need to be able to trust that something you’ve put into your knowledgebase can be accessed 10 years from now. In order to accomplish this, you should own your data, and have it in a format that _you understand_.

What does portability mean?

* **File Format**: I have a strong preference for plaintext over things like Word or Google Docs. In theory, you could export those docs if the software ever became unsupported, but you have very little control over the export result and its suitability for your needs.
* **File Content**: I have a strong preference for native formats that directly represent my knowledge as data. For example, in `markdown`, there is no “table of contents” directive, so there are two ways this can be accomplished:

{% tabs %}
{% tab title="Plugins + Standard Syntax" %}
A plugin in your editor could parse the headers and auto-generate a table of contents with lists and links:

{% code title="example.md" %}
```text
- [First Section](#first-section)
  - [Nested Section](#nested-section)

# First Section
## Nested Section
```
{% endcode %}

This is my generally preferred option, since any other markdown parser will understand this, and doesn't couple you to some special "table-of-contents" program, but rather expresses what you want with your table of contents as "data", directly in markdown.
{% endtab %}

{% tab title="Custom Directive" %}
You could make a dialect of markdown by adding a custom directive that your editor uses.

{% code title="example.md" %}
```text
![toc]
# First Section
## Nested Section
```
{% endcode %}

I dislike this option because other tools won't understand this special dialect, which makes this essentially "code".
{% endtab %}
{% endtabs %}

* **Rendering**: I enjoy interleaving some visuals and code in my knowledge, but I prefer native features like markdown’s typed codeblocks for including the code, and then having plugins for my renderer to handle specific codeblocks in certain ways \(for example, understanding `mermaid` and rendering charts, or `latex` and rendering math\).  This way, you retain _progressive enhancement_: every markdown parser will display it as a codeblock at minimum.

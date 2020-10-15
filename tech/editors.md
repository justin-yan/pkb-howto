# Editors

There is a huge range of editors out there.  Many of these tools are not exactly equivalent because they combine different features in one tool: some of these handle the synchronization of your data, others manage the file formats for you, so on and so forth.

Very loosely speaking, the more you care about control of your data and the underlying formats, the more additional work you'll have to do yourself \(figuring out how to handle filesync, migrations, etc.\).  Beyond that, there are a variety of other considerations: privacy, built-in linking, WYSIWYG editing, render modes, web clipping, and so on.  The best way for you to get a feel for what matters to you is to just try out a few different tools and see what you like.

I've included a sample list of tools that I've _heard of other people_ using for PKBs: \(**do your own due diligence** for whether you trust this software - this list is not a recommendation or me advocating for the safety of any this software.  As far as I know, they could be selling your notes to the highest bidder.\)

* [SublimeText](https://www.sublimetext.com/)
* [Obsidian](https://obsidian.md/)
* [Typora](https://typora.io/)
* [StandardNotes](https://standardnotes.org/)
* [Emacs Org-Mode](https://orgmode.org/)
* [Zettlr](https://www.zettlr.com/)
* [Notion](https://www.notion.so/)
* [RoamResearch](https://roamresearch.com/)
* [MediaWiki](https://www.mediawiki.org/wiki/MediaWiki)
* [TiddlyWiki](https://tiddlywiki.com/)
* [EverNote](https://evernote.com/)
* [OneNote](https://www.microsoft.com/en-us/microsoft-365/onenote)
* [Google Docs](https://docs.google.com/)

### SublimeText

SublimeText will give you a lot of control over your data and extremely smooth text editing capabilities.  You have the freedom to work with any file in any format, which means you'll have to make some choices about your file format, how you'll sync your data, and so on.  For now, unless you have a different preference, it's probably easiest to just start writing new files in [Markdown](https://www.markdownguide.org/) and go from there.

The tips below should help you make the most of using Sublime.

{% hint style="info" %}
Create a **sublime-project** file in your root folder
{% endhint %}

{% code title="~/pkb/pkb.sublime-project" %}
```javascript

	"folders":
	[
		{
			"binary_file_patterns":
			[
				"*.pdf",
				"*.PDF",
				"*.doc",
				"*.docx",
				"*.xlsx",
				"*.pptx"
			],
			"path": "."
		}
	]
}

```
{% endcode %}

This makes it possible for you to quickly open up your PKB through the project switcher \(`ctrl + alt + p` and select `pkb`\).

{% hint style="info" %}
Use **plugins**
{% endhint %}

* [MarkdownEditing](https://packagecontrol.io/packages/MarkdownEditing) adds useful features like Wikilink support.
* [MarkdownPreview](https://packagecontrol.io/packages/MarkdownPreview) adds the ability to view your rendered markdown.
* [MarkdownTOC](https://packagecontrol.io/packages/MarkdownTOC) easily generates table of contents.
* [TableEditor](https://packagecontrol.io/packages/Table%20Editor) makes working with tables a breeze.


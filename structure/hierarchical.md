# Hierarchical

Hierarchical structure is what we are generally most familiar with on a day-to-day basis: the folder systems on our computers are hierarchical \(each folder can be in at most one other folder\).  Advocates of associative structure warn about using folders and the risks of too much hierarchy, and while their advice is pretty good, I still think there are some good reasons for using folders.

The first argument in favor of using an associative structure is that an Index note _should_ be able to mimic any folder structure. After all, isn’t a folder called `Work` containing a few files basically the same thing as a file called `Work.md` that holds _links_ to those same files?  And if you use a folder, all of those files can't be in any other folder - but what if one of them is also relevant for, say, `School`?  In this sense, isn't a folder strictly worse than linking?

The important thing to understand about the use of folders in a hierarchical structure is that the main benefit is in its ability to _encapsulate_ knowledge beyond simply providing structure:

1. Folders have a standard and well-supported visualization \(the folder tree/project explorer\) which lets you navigate structure very quickly. As far as graph views have come, they are still not nearly as concise and intuitive, and I don't know anyone who maintains the strawman of 2000 files in a folder.
2. Folders have a variety of _folder-level operations_ such as _moving_ or _deleting_, that provides a lot of ease of use for _encapsulating_ and _operating on_ a domain of knowledge as an entire block. It’s not impossible, but it is much harder to naturally do the same with a linking structure, because many files could link to the same note.

Now, the exclusionary nature of folders is certainly a substantial downside.  When you stick something in a folder, it can only be in that one folder, which is a tricky limitation because most of the things we call “subjects” are somewhat arbitrary boundaries we’ve drawn around collections of facts. For example, should `Behavioral Finance` go in an `Economics` folder or a `Psychology` folder? Should `Game Theory` go in `Math` or `Economics`?

In my experience, the important thing to become comfortable with is that _knowledge domains will overlap_.  Creating a folder for an abstraction like "Math" is _useful_ because you can use it to encapsulate things like the millions of files that LaTeX might generate, or perhaps to move that entire collection of files to the trash.  But putting "Game Theory" inside of "Math" doesn't mean that Game Theory _**is**_ Math - it just means that you happened to feel that was a natural encapsulation for it.  You could very reasonably link to Game Theory from inside of Economics, and understand that this knowledge is relevant in multiple domains.

It would be _just as correct_ to put Game Theory inside of Economics and refer to it from Math.  Or even put Game Theory into its own folder at the same level as Economics and Math, and then link to it from both of them.  You are just organizing a series of knowledge domains in whatever way represents _useful structure_ _for your cognitive problems_.  If you find yourself wasting time digging through thousands of files, some folders might help.  If on the other hand you're digging through 10 layers of folders and can't find anything, perhaps you should flatten things out.  Over the years, I've come to develop the following heuristics:

1. Use some folders.
2. Don’t use too many folders.
3. You’ll know what the right balance is based on how productive you are vs. much time you waste dealing with folders.
4. Don’t implement workflow with folders. I’ve found that I like using different workflows in different parts of my PKB, and every time I’ve created workflows involving folders \(e.g. “Current Actions” and “Next Actions” folders\), I’ve found myself regularly rebuilding the whole thing \(and wasting time\).
5. Don’t worry too much about the exclusion problem: using the `behavioral finance` example, I will generally just quickly put it in whatever feels right \(`economics`\), or mix in the use of associative links \(put it next to `economics` and `psychology` and reference it from within those other folders\), or just **duplicate** it into both of them.  You can even do all three of these at the same time.


# Hierarchical

A lot of people warn about excess hierarchy with folders, and argue in favor of associative knowledge instead \(tags, links\). I think this is pretty good advice, but there are some good reasons for using folders as well, so I’ll try to break down the arguments.

The first point is that an associative structure _should_ be able to mimic any folder structure. After all, isn’t a folder `Work` containing a few files basically the same thing as a file `Work.md` that holds links to those same files? In this sense, a folder seems to be “strictly worse” than links. However, there are a few ways in which this “limitation” results in some concrete benefits:

1. Folders help you _encapsulate_ knowledge by treating everything inside as a block. It’s harder to do the same with the links, because many files could link to the same note, so under which file should your explorer hide that note?
2. Folders have a standard and well-supported visualization \(the folder tree/project explorer\) which lets you explore and locate knowledge very quickly. As far as graph views have come, they are still not nearly as concise, and the strawman of 2000 files in a folder seems pretty nontenable.

So why not use lots of folders? Programmers will be pretty familiar with the problem that folders present, however, which is that they are essentially _inheritance_. When you stick something in a folder, it can only be in that one folder, and suggests the relationship “this file _is an instance of_ this folder”. This is a pretty tricky limitation because most of the things we call “subjects” are moderately arbitrary boundaries we’ve drawn around collections of facts. For example, should `Behavioral Finance` go in an `Economics` folder or a `Psychology` folder? Should `Game Theory` go in `Math` or `Economics`?

The truth is that it actually _doesn’t matter_. The important thing to remember is that a particular hierarchy is just _one way_ of segmenting your knowledge into categories. There is no “correct structure”, and indeed, different ways of grouping subjects can present new insights and connections. A piece of knowledge is a standalone fact, and the “subjects” we construct \(Biology, Economics, Psychology, Math, etc.\) are conventions for grouping these facts together in a way that makes them more understandable. These subject groupings are often extremely useful, but at the same time, trying to pin down which of two subjects something goes into is generally not a super valuable use of time.

As a result I’ve largely settled on the following rules when it comes to folders:

1. Use folders.
2. Don’t use too many folders.
3. You’ll know what the right balance is based on how productive you are vs. much time you waste dealing with folders.
4. Don’t implement workflow with folders. I’ve found that I like using different workflows in different parts of my PKB, and every time I’ve created workflows involving folders \(e.g. “Current Actions” and “Next Actions” folders\), I’ve found myself regularly rebuilding the whole thing \(and wasting time\). Using folders to describe domains \(e.g. Math\) and working within files \(and using links\) for workflows has felt more stable and productive to me.
5. Don’t worry too much about ambiguity: using the `behavioral finance` example, I will generally just quickly put it in whatever feels right \(`economics`\), or make it an associative sibling \(put it next to `economics` and `psychology` and reference it from within those other folders\), or just duplicate it into both of them. Mistakes are easy to fix and this generally takes less time than agonizing about the decision to begin with.


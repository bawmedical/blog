## Why you don’t need a separate ‘document store’ for your Discourse online community

Pretty much every time I create a new ‘social collaboration’ Discourse setup for a new professional community I’m asked if there can be some kind of ‘document store’ built into it.

When I talk to the customer about this user need, they usually tend to mean that they want something like Dropbox, SharePoint, or some other ‘directory based’ file store.

Yes, you might argue that we should really be moving away from uploading documents and towards linking to web-native formats, but the reality of most businesses is that people use a lot of .docx, .xlsx, and similar offline doc formats, and this isn’t going to change immediately.

What the users *think* they want is a cloud based ‘directory structure’ into which the community can upload their useful shareable documents. In my communities this is often professional shareable resources like job descriptions for roles, clinical safety cases for health tech, internal policy documents, and standards definitions.

Having had a great deal of experience with this kind of file storage user request while running *Discourse-as-a-Service* for numerous professional communities in healthcare technology and related fields — **I’m going to tell you now why I don’t think you need it.**

Industry standard naming conventions for confusing and chaotic shared document stores (official, final, final v7.7)

### The Tragedy of The Commons

The Tragedy of the Commons is a phenomenon with which people who run communities are probably familiar. It’s the sad state of affairs that when something belongs to ‘everybody’, **nobody** takes care of it.

And this is exactly what happens with shared file-store platforms. Whilst there is often an initial fervour and lots of initial engagement in uploading new files and sharing, and lots of excitement about the information that’s available to everybody, this wanes after a time and, after a period of three to six months (YMMV), you’ll find that what’s left in your file store is total chaos.

Nobody knows who the files belong to, how old they are, or if they’re still current. Because of this, even if you do want to ‘tidy up’ the file store — few people quite have the courage to delete anything, because it could be something that somebody still needs. Even with active curation of the store, it’s nigh-on impossible for the curators to keep a tidy and usable repository.

You’ll find that the files are usually not versioned and there’s not always any indication of the owner of the file. Consequently, what you end up with is a jumble of files with random naming schemes (if there is a discernible naming pattern at all), making it impossible after a while to find anything — even if your site has good search.

### Experience with Discourse and Alfresco

When I was setting up the [Digital Health Networks](http://discourse.digitalhealth.net) on [Discourse](http://discourse.org) for the [CCIO Network](https://twitter.com/dhccio), on behalf of Digital Health Intelligence we also tried to set up [Alfresco](https://www.alfresco.com/) as a parallel file storage platform because of exactly this perceived user need for a file store.

And although we encountered other issues with Alfresco (such as the Community Edition lacking some features which we needed), the actual file storing platform failed us in exactly this way.

The files ended up as a mess that nobody could unpick. The initial excited uploading of files drifted into the trough of disillusionment when nobody could find the useful files they needed among the morass of other stuff. In the end, I exported everything from Alfresco and shut it down.

I transferred all the files into Discourse as uploads in topics, with a descriptive title and some text in the Topic that explained the purpose of the document. Where multiple files were related, I uploaded them as part of the same topic. And as I did so I realised why you **just don’t need a separate file store.**

### You don’t need ‘file storage’ when you’ve got Discourse

Using a forum for your file storage is a completely different and much better proposition to a ‘directory’ style of document dump. Because the nature of these uploads is that they’re *part of a conversation,* it’s much more likely that you can make sense of them when reading back later.

Every file that’s uploaded by anyone in a Discourse forum is always associated with the post or topic. Which means that **for no additional effort**, you get a Title, the ownership of the file (the user posting it), and the date it was uploaded.

But most important is the **conversation and the discussion** around this file or series of files. This is what helps someone coming along later to work out if these files are likely to be of use to them. Even with an actively and intelligently human-curated file-store, it’s hard to get this level of contextual information around the documents, and yet in a forum this context happens without additional effort.

And so it’s much easier to keep track of what is current. What is old. What is likely to have been superseded or have become obsolete. Updates to documents flow down the page in the discussion thread. And in Discourse you can ‘wikify’ the original post and maintain updates in the OP as well, so that people finding the thread can get the latest version right away.

A**nd so, actually, this is the solution to the problem. You don’t need a separate file storage system. You just need to educate your community to use their Discourse discussion platform for this.**

In Discourse, the content starts to form its own kind of self-curating ‘library of useful stuff’. Something that was uploaded by somebody in a thread that six years old, is probably likely to have been superseded or outdated by now. So it kind of keeps itself tidy. Text searching on the title of the document will still work, just as it would have done in the file-store paradigm, but additionally you have so much else that the search can hit — the context and discussion around the document aids discoverability of the documents.

And so in short, if your community is asking for a file store, the actual answer is they don’t need one. But as a good community manager, you **do** need to explain to them **why** they don’t need one, what will inevitably happen if they DO use one, and make the strong case for using Discourse as your document store. As ever, bringing your community along with you is the key to doing it well.
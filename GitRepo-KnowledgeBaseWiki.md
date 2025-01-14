# A Personal Git Repo as a Knowledge Base Wiki - DEV Community
![image](https://github.com/user-attachments/assets/9b4ff48d-38ac-4dae-8159-97eb07234f68)

###### [Article](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51)

[#productivity](/t/productivity) [#writing](/t/writing) [#markdown](/t/markdown) [#documentation](/t/documentation)

While it's not something that everyone likes to do, I've always found it essential to write notes. There are the project-specific notes that only have relevance within a particular workplace and are of course confidential, but then the stacks of notes that cover everything from the content of the training course you last went on to "what's the command-line way to add a new project again?" - and that second category is the one we're going to discuss here.

Besides good old pen and paper I've tried all sorts, with tools like Evernote, Keep, the original Catch Notes (RIP), and Apple Notes each having very different levels of support for formatting, embedding, and crucially, portability of stored data. The latter becomes especially significant if the service closes down, or if (in the case of Apple Notes) you hand back the computer at the end of a job. As I looked at the pages of pencilled notes I'd written while following an online tutorial recently, I realised that a more unified and durable approach would be extremely useful. A solution flashed into my head while updating the wiki for a personal project on Bitbucket - why not have a private repo consisting entirely of Markdown notes, rather than code?

[](#benefits)Benefits
---------------------

*   Markdown is familiar to a large proportion of developers, is easy to write, and widely-supported - but also fairly readable even as plain text without a parser.
*   Markdown has great support for inserting the kinds of things we so often need - code snippets, links, tables, and multi-level bullet lists - with minimal effort, allowing you to concentrate on the content.
*   Using a Git repo makes it easy to quickly sync the notes across machines.
*   This approach removes the reliance on proprietary sites. As each copy of the repo is just the same as any other, even the loss of your online Git account is not catastrophic.

[](#basic-structure)Basic Structure
-----------------------------------

The root of the repo has an `index.md` file, with each overall topic being contained in a folder - and each of these also contains an `index.md`. If it's a big enough topic, there might be an extra level, but the aim is _just organised enough_ without having a crazy directory tree structure.  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fymebjvcjr5juagswzq8m.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fymebjvcjr5juagswzq8m.png)

The root `index.md` contains links to the index files in each folder.  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fmj7vjwqbvmxw0d0y6s7x.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fmj7vjwqbvmxw0d0y6s7x.png)  
Those index files, in turn, link to other `.md` files within their own directories for each article.

[](#article-content)Article Content
-----------------------------------

The beauty of this being your _private_ repo is that you're not beholden to any particular standard - you can be free to write in as formal or as loose a way as you'd like. At some times you might have nothing but a raw text braindump, at others you may have topics that you can write on in a more structured way. The point that is central is that you write in the way that works _for you_, in the terms that make it the most useful for the way you read, think, and recall.

Code snippets (with the original spacing preserved) and shell commands can be inserted easily, as can links to external resources that might be useful for each topic.  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F2rz28t5f47h450mg2c8s.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F2rz28t5f47h450mg2c8s.png)  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fj5yftac1b6to2vzscqb9.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fj5yftac1b6to2vzscqb9.png)

In addition, now that everyone has a camera in their pocket, diagrams can be sketched, photographed, and included as inline images, rather than being laboriously reproduced with a computerised drawing tool.  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fudyl2jj5svcaut7pvf2q.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fudyl2jj5svcaut7pvf2q.png)

As an aside, if you need to copy/paste formatted text from other document formats, [PuppyPaste](https://puppypaste.com/) is a very handy tool which will convert the formatting to the Markdown equivalent, which you can then copy/paste/edit as necessary.

[](#reading)Reading
-------------------

The main online Git sites will support the viewing of Markdown files, but if you want to view them outside of this framework then a small amount of extra work is needed. As web browsers don't generally have native support for Markdown files, you can't get the benefit of using one as a viewer directly, but some very kind people have provided solutions to this. Someone recommended [MDwiki](https://dynalon.github.io/mdwiki/#!index.md) and having used it, I will too.

Simply download the HTML file into the root of your repo, and rename it to `index.html`. Pointing a web server at this folder (I wrote an absolutely minimal one with Node.js and Express) makes it an HTML web-browsable wiki.  
[![](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F5keln5vc4037wzlmdtlr.png)
](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F5keln5vc4037wzlmdtlr.png)

[](#uses-and-conclusion)Uses and Conclusion
-------------------------------------------

I now have copies of my own repo on a Windows desktop, Mac laptop, and a USB flash drive, as well as on Bitbucket. A quick `git pull` on each grabs the latest changes as needed, and after that the notes are available even if there is no network available. I'll be continually adding to it and think that this is a solid way of preserving the jewels picked up along my development journey. I hope some of you find this approach useful too!

[![](https://media2.dev.to/dynamic/image/width=64,height=64,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Forganization%2Fprofile_image%2F7065%2F76b8a4ec-ad62-4abe-b67d-a6572f9d4b0c.png)

Devs on Wix

](/wixfordevs)Promoted

Dropdown menu

*   [What's a billboard?](/billboards)
*   [Manage preferences](/settings/customization#sponsors)

* * *

*   [Report billboard](/report-abuse?billboard=203216)

[![](https://media2.dev.to/dynamic/image/width=775%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fi.imgur.com%2FacRjfK8.jpeg)
](https://www.wix.com/studio/developers/build-wix-apps/learn-how/?utm=devto_ad&bb=203216)

[](#2025-your-year-to-build-apps-that-sell)[2025: Your year to build apps that sell](https://www.wix.com/studio/developers/build-wix-apps/learn-how/?utm=devto_ad&bb=203216)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Dive into hands-on resources and actionable strategies designed to help you build and sell apps on the Wix App Market.

[Get started](https://www.wix.com/studio/developers/build-wix-apps/learn-how/?utm=devto_ad&bb=203216)

Top comments (23)
-----------------

Subscribe

    ![](https://media2.dev.to/dynamic/image/width=256,height=,fit=scale-down,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F8j7kvp660rqzt99zui8e.png) 

Personal Trusted User

[Create template](/settings/response-templates)

Templates let you quickly answer FAQs or store snippets for re-use.

Submit Preview [Dismiss](/404.html)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F218294%2Fa7eed80f-0283-4ac6-96fc-68fa73319f1a.jpeg)](https://dev.to/mrrcollins) 

[Ryan Collins](https://dev.to/mrrcollins)

Ryan Collins

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F218294%2Fa7eed80f-0283-4ac6-96fc-68fa73319f1a.jpeg)  Ryan Collins](/mrrcollins) 

Follow

Just a geek developing through life.

*   Joined
    
    Aug 25, 2019
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk7b)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk7b)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/mrrcollins/comment/1bk7b)

I learned of [Obsidian](https://obsidian.md/) last week from [harshibar](https://www.youtube.com/watch?v=ms4cWMsOITs). It looks promising, unfortunately, it doesn't recognize .markdown as a Markdown file. :-(

From my limited testing, it looks like it could be useful, especially being able to create links.

Like comment: Like comment: 4 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk7b)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F101333%2Fd7429dbe-8e4b-4ceb-92d2-1b14437c313c.jpeg)](https://dev.to/thomashighbaugh) 

[Thomas Leon Highbaugh](https://dev.to/thomashighbaugh)

Thomas Leon Highbaugh

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F101333%2Fd7429dbe-8e4b-4ceb-92d2-1b14437c313c.jpeg)  Thomas Leon Highbaugh](/thomashighbaugh) 

Follow

Web developer, dog owner & Linux nut. https://thomasleonhighbaugh.me I also use machine learning to make some bomb art too.

*   Location
    
    Bay Area
    
*   Education
    
    College, Certificate, More College, Lot of Udemy
    
*   Work
    
    Self-Employed Web Developer // Starving Artist // World's Best Dog Owner
    
*   Joined
    
    Sep 14, 2018
    

• [Jun 5 '24](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-2filj)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-2filj)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/thomashighbaugh/comment/2filj)

That's an easy enough solution with a batch renaming tool to switch `.markdown` to `.md`, depending on your platform/package-manager the tools differ of course so figure out which one works for you but personally obsidian is just another vendor to lock you into their product and its opinionated assumptions.

Like comment: Like comment: 1 like Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/2filj)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk7c)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk7c)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bk7c)

Thanks for the tip!

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk7c)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F743903%2Fdcbad19b-c206-436a-83bb-ad5aa02c7576.png)](https://dev.to/scottgilhooly) 

[ScottGilhooly](https://dev.to/scottgilhooly)

ScottGilhooly

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F743903%2Fdcbad19b-c206-436a-83bb-ad5aa02c7576.png)  ScottGilhooly](/scottgilhooly) 

Follow

Music and Films and Software ... Oh My!

*   Education
    
    University of Glasgow
    
*   Work
    
    Developer at University of Manchester
    
*   Joined
    
    Nov 3, 2021
    

• [Nov 3 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1jdd4)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1jdd4)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/scottgilhooly/comment/1jdd4)

+1 for Obsidian. Nice and simple and portable (I have it on Mac and Windows). Oddly, never occurred to me to put all the notes i have scattered EVERYWHERE into a git repo!

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1jdd4)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)](https://dev.to/cadams) 

[Chad Adams](https://dev.to/cadams)

Chad Adams

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)  Chad Adams](/cadams) 

Follow

Senior Software Engineer

*   Location
    
    Okatie, SC
    
*   Work
    
    Senior Software Engineer, Experian
    
*   Joined
    
    Aug 21, 2018
    

• [Feb 20 '21 • Edited on Feb 20 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk12)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk12)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/cadams/comment/1bk12)

I did this too but thought instead of making it private why not make it public. Seems like every developer I know does this in some way.

I started a project a couple weeks ago to fix this problem. It’s in the concept phase so a lot of design can change. I’m looking for some feedback so if you want to check it out that would be great. :)

[syntaxrecall.dev](https://syntaxrecall.dev)  
[github.com/syntaxrecall/syntaxrecall](https://github.com/syntaxrecall/syntaxrecall)

Like comment: Like comment: 3 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk12)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 20 '21 • Edited on Feb 20 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1f)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1f)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bk1f)

I've actually never known another developer do this (or if they have, they've been quiet about it), but I guess writing about it attracts other people who think the same way!

Making content public or private is down to personal choice of course, but I think there's something to be said about removing the pressure of the public gaze and tailoring the content to exactly what _you_ need. There's also a benefit if you want to use code snippets/examples/diagrams (or entire topics) that you explicitly don't want to share for whatever reason. However, using an open source format like MD means that it's very easy to port content out from one repo to another if there's something to share more widely.

Thanks for the link! I tried to launch the site itself but couldn't get it to respond to any searches - are there any pre-requisites for the browser running it?

Like comment: Like comment: 3 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk1f)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)](https://dev.to/cadams) 

[Chad Adams](https://dev.to/cadams)

Chad Adams

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)  Chad Adams](/cadams) 

Follow

Senior Software Engineer

*   Location
    
    Okatie, SC
    
*   Work
    
    Senior Software Engineer, Experian
    
*   Joined
    
    Aug 21, 2018
    

• [Feb 20 '21 • Edited on Feb 20 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1h)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1h)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/cadams/comment/1bk1h)

Some of the devs I've worked with use [cacher.io/](https://www.cacher.io/). I tried it, but I didn't want to pay for it. I like the personal wiki approach but I prefer the devhints.io approach more. Everyone can contribute and knowledge share. Saves everyone time, making everyone more productive.

For my site yeah there's not much content currently cause I just started it. Try searching for one of these though.

**Cheatsheets**

*   Git
*   VSCode
*   Lua
*   Markdown
*   Sass
*   Screen
*   Vim
*   Yarn

**Tools**

*   JSON Editor
*   Phobia
*   Tailwind playground

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk1h)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F18587%2Fca1b8a36-25ff-4939-9a0f-0a43d8c586e4.JPG)](https://dev.to/subbramanil) 

[Subbu Lakshmanan](https://dev.to/subbramanil)

Subbu Lakshmanan

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F18587%2Fca1b8a36-25ff-4939-9a0f-0a43d8c586e4.JPG)  Subbu Lakshmanan](/subbramanil) 

Follow

Enthusiastic programmer, working as Android developer building custom Android Images (AOSP) and apps.

*   Email
    
    [subbramanil@gmail.com](mailto:subbramanil@gmail.com)
    
*   Location
    
    Dallas, Tx
    
*   Education
    
    Masters of Computer Science
    
*   Joined
    
    May 9, 2017
    

• [Mar 16 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1cep3)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1cep3)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/subbramanil/comment/1cep3)

Love the idea of browsing & viewing the notes on a browser!! I have been using markdown + VSCode + git for my notes for over 4 years now. Absolutely love it!!

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--w8t1DEUl--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/67pklswh2t52fagmpdjg.png)
](https://res.cloudinary.com/practicaldev/image/fetch/s--w8t1DEUl--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/67pklswh2t52fagmpdjg.png)

I will give it a try on MDWiki!! Thanks for the great post!!

Like comment: Like comment: 4 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1cep3)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Mar 16 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1cf06)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1cf06)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1cf06)

Thank you! I love that you've got your actual daily project notes there too - great for recalling design decisions from the distant past :)

Like comment: Like comment: 1 like Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1cf06)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F557962%2F9e235317-6c46-4fc4-a1ce-5ac49c6ce52e.png)](https://dev.to/timothydjones) 

[Tim Jones](https://dev.to/timothydjones)

Tim Jones

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F557962%2F9e235317-6c46-4fc4-a1ce-5ac49c6ce52e.png)  Tim Jones](/timothydjones) 

Follow

Python devops automation developer with 25+ years of experience in application development, including Java, SQL, GIS, and a variety of other technologies. Always looking to learn new things.

*   Location
    
    Tulsa, OK, USA
    
*   Work
    
    Automation Engineer
    
*   Joined
    
    Jan 11, 2021
    

• [Feb 19 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bjck)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bjck)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/timothydjones/comment/1bjck)

Hi, Adam. Thanks for the tip about MDwiki. I'm going to look into that.

I have recently started [my own TIL repository](https://github.com/TimothyDJones/til) on GitHub following several of the concepts that you described. I don't have much there yet, but it seems to be a good fit for me so far. Check it out and let me know what you think.

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bjck)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)](https://dev.to/cadams) 

[Chad Adams](https://dev.to/cadams)

Chad Adams

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F94831%2F86fa0534-8e6b-4a52-bc0b-d821fbf3ad88.jpg)  Chad Adams](/cadams) 

Follow

Senior Software Engineer

*   Location
    
    Okatie, SC
    
*   Work
    
    Senior Software Engineer, Experian
    
*   Joined
    
    Aug 21, 2018
    

• [Feb 20 '21 • Edited on Feb 20 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1o)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk1o)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/cadams/comment/1bk1o)

If you don't mind check these out and give me some feedback. :)  
[syntaxrecall.dev/vscode-keyboard-s...](https://syntaxrecall.dev/vscode-keyboard-shortcuts)  
[syntaxrecall.dev/vim](https://syntaxrecall.dev/vim)

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk1o)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk2g)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bk2g)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bk2g)

Looking good! I'll definitely be making use of some of those VS code shortcuts.  
(as an aside, it is a classic of dev life that you need a cheat sheet to exit `vi` 🙂)

Like comment: Like comment: 1 like Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bk2g)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bjng)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bjng)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bjng)

I like where you're going with that! I might borrow the idea of having a section specifically for tools - little cheat sheet pages that would be really useful on a second monitor 👍🏿

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bjng)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F263541%2F3f18c71c-0891-447a-ab3b-2230935bf7af.png)](https://dev.to/kevlatus) 

[Kevin Latusinski](https://dev.to/kevlatus)

Kevin Latusinski

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F263541%2F3f18c71c-0891-447a-ab3b-2230935bf7af.png)  Kevin Latusinski](/kevlatus) 

Follow

I build digital experiences that bring joy into everyday life.

*   Location
    
    Germany
    
*   Joined
    
    Nov 2, 2019
    

• [Feb 22 '21 • Edited on Feb 22 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bm2m)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bm2m)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/kevlatus/comment/1bm2m)

it sounds like [foam](https://foambubble.github.io/foam/) might be for you: it uses exactly your type of markdown and file based layout, while simplifying the process of linking content. All while being a VSCode plugin.  
I recently started using it and must admit that I'm hooked 🤷‍♂️

Like comment: Like comment: 3 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bm2m)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F517878%2Ff216ec89-2513-4d84-a18e-7a3988f7c629.png)](https://dev.to/maxivanov) 

[Max Ivanov](https://dev.to/maxivanov)

Max Ivanov

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F517878%2Ff216ec89-2513-4d84-a18e-7a3988f7c629.png)  Max Ivanov](/maxivanov) 

Follow

Software Engineer / Cloud Architect. I help developers use cloud platforms efficiently. I write about Azure, AWS, Serverless, full-stack TypeScript.

*   Location
    
    Portugal
    
*   Work
    
    Software Engineer
    
*   Joined
    
    Nov 20, 2020
    

• [Feb 21 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkld)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkld)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/maxivanov/comment/1bkld)

Like it. What's your process of adding images to the pages? Is it: take a picture with a smartphone → icloud/dropbox sync to computer → move the file to the repo → add an image in markdown?  
I'm yet to find a perfect solution for a personal knowledge base. I like to add diagrams next to the text (often a doodle is worth a hundred words) and I want the process to be as easy as possible. I found Notability app to serve best my needs. Using it on my iPad and computer. Also tried OneNote, GoodNotes and (Apple) Notes but they didn't click with me.

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bkld)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 21 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkn4)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkn4)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bkn4)

Thank you! Yes, that's basically the process for adding images - I've only had to do that with one or two hand-drawn ones so far, for screenshots it's of course even simpler than that.  
When I was first introduced to Apple Notes, I got into using it but getting the information out was ridiculous - I ended up connecting it to my Google account and so the notes now live in a Gmail folder as though they're emails. I've started the process of copying/reformatting the info to live in this repo, where it'll be a bit more useful!

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bkn4)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F498293%2F36c2d582-65f1-4975-9235-6e72e911e97b.jpeg)](https://dev.to/timster) 

[Tim Shaffer](https://dev.to/timster)

Tim Shaffer

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F498293%2F36c2d582-65f1-4975-9235-6e72e911e97b.jpeg)  Tim Shaffer](/timster) 

Follow

*   Joined
    
    Oct 24, 2020
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkcd)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkcd)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/timster/comment/1bkcd)

If you want a super easy http server, python has one built in. Just go to the directory and run this:

`python3 -m http.server`

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bkcd)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)](https://dev.to/adam_b) 

[Adam Braimah](https://dev.to/adam_b)

Adam Braimah

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

• [Feb 21 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bki8)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bki8)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/adam_b/comment/1bki8)

That's a great tip! 👍🏿

Like comment: Like comment: 1 like Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bki8)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F448938%2Fa96bdbed-af66-4f21-81c6-eb16fc2293a7.png)](https://dev.to/eelstork) 

[Tea](https://dev.to/eelstork)

Tea

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F448938%2Fa96bdbed-af66-4f21-81c6-eb16fc2293a7.png)  Tea](/eelstork) 

Follow

Language and API Design, Game AI, Behavior trees, Procedural Design, Entrepreneurship. Concise code.

*   Location
    
    Formosa
    
*   Education
    
    Computational Creativity (PhD)
    
*   Work
    
    Senior Game AI Engineer at Ultimerse
    
*   Joined
    
    Aug 7, 2020
    

• [Feb 21 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bknb)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bknb)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/eelstork/comment/1bknb)

Also - try Notational Velocity if you're on macOS

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bknb)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F167787%2F8e1aadbe-8af0-4524-b69b-6083d60668f9.jpeg)](https://dev.to/epszaw) 

[Konstantin Epishev](https://dev.to/epszaw)

Konstantin Epishev

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F167787%2F8e1aadbe-8af0-4524-b69b-6083d60668f9.jpeg)  Konstantin Epishev](/epszaw) 

Follow

Interested in the things around.

*   Email
    
    [lamartire@gmail.com](mailto:lamartire@gmail.com)
    
*   Location
    
    Poland
    
*   Work
    
    Software Engineer at Uscreen Inc.
    
*   Joined
    
    May 15, 2019
    

• [Feb 20 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkap)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1bkap)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/epszaw/comment/1bkap)

Like your idea. Honestly, there is really no need to do website to collect something. Never thought about "just repository" as about a knowledge base!

Like comment: Like comment: 2 likes Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1bkap)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)](https://dev.to/longtth) 

[Long Nguyễn Xuân](https://dev.to/longtth)

Long Nguyễn Xuân

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)  Long Nguyễn Xuân](/longtth) 

Follow

Just an average man in the world, I love software and Software Engineering. full time Project Manager and Business Analyst. part time lecturer, life time learner.

*   Email
    
    [longtth@gmail.com](mailto:longtth@gmail.com)
    
*   Location
    
    Da nang, vietnam
    
*   Joined
    
    Mar 25, 2021
    

• [Aug 16 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h998)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h998)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/longtth/comment/1h998)

MDwiki is stopped maintain.  
And when I tried with ver 0.6.2, it doesn't show up anything, error

Like comment: Like comment: Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1h998)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)](https://dev.to/longtth) 

[Long Nguyễn Xuân](https://dev.to/longtth)

Long Nguyễn Xuân

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)  Long Nguyễn Xuân](/longtth) 

Follow

Just an average man in the world, I love software and Software Engineering. full time Project Manager and Business Analyst. part time lecturer, life time learner.

*   Email
    
    [longtth@gmail.com](mailto:longtth@gmail.com)
    
*   Location
    
    Da nang, vietnam
    
*   Joined
    
    Mar 25, 2021
    

• [Aug 16 '21](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h999)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h999)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/longtth/comment/1h999)

[imgur.com/isDChd9](https://imgur.com/isDChd9)

Like comment: Like comment: Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1h999)

Collapse Expand

 

 [![](https://media2.dev.to/dynamic/image/width=50,height=50,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)](https://dev.to/longtth) 

[Long Nguyễn Xuân](https://dev.to/longtth)

Long Nguyễn Xuân

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F603874%2F8d78146e-811e-46a3-94e6-f4a5b6718d6b.jpg)  Long Nguyễn Xuân](/longtth) 

Follow

Just an average man in the world, I love software and Software Engineering. full time Project Manager and Business Analyst. part time lecturer, life time learner.

*   Email
    
    [longtth@gmail.com](mailto:longtth@gmail.com)
    
*   Location
    
    Da nang, vietnam
    
*   Joined
    
    Mar 25, 2021
    

• [Aug 16 '21 • Edited on Aug 16 • Edited](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h99a)

Dropdown menu

*   [Copy link](https://dev.to/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51#comment-1h99a)

*   Hide

*   [Report abuse](/report-abuse?url=https://dev.to/longtth/comment/1h99a)

can you have a look!?

Like comment: Like comment: Like [Comment button Reply](#/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments/new/1h99a)

[View full discussion (23 comments)](/adam_b/a-personal-git-repo-as-a-knowledge-base-wiki-j51/comments)

[Code of Conduct](/code-of-conduct) • [Report abuse](/report-abuse)

Are you sure you want to hide this comment? It will become hidden in your post, but will still be visible via the comment's [permalink](#).

Hide child comments as well

Confirm

For further actions, you may consider blocking this person and/or [reporting abuse](/report-abuse)

[![](https://media2.dev.to/dynamic/image/width=64,height=64,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Forganization%2Fprofile_image%2F5051%2Fec213fb0-f4a0-49ca-aedf-d18ed4445858.png)

Pieces.app

](/getpieces)Promoted

Dropdown menu

*   [What's a billboard?](/billboards)
*   [Manage preferences](/settings/customization#sponsors)

* * *

*   [Report billboard](/report-abuse?billboard=59778)

[](#eliminate-context-switching-and-maximize-productivity)[Eliminate Context Switching and Maximize Productivity](https://docs.pieces.app/extensions-plugins/obsidian?utm_source=dev-to&utm_medium=banner&utm_campaign=dev-to-site&bb=59778)
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[![](https://media2.dev.to/dynamic/image/width=775%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F2ba1tyyafghcrnb8m9oe.png)
](https://docs.pieces.app/extensions-plugins/obsidian?utm_source=dev-to&utm_medium=banner&utm_campaign=dev-to-site&bb=59778)

Pieces Copilot is your personalized workflow assistant, working alongside your favorite apps. Ask questions about entire repositories, generate contextualized code, save and reuse useful snippets, and streamline your development process.

[Learn more](https://docs.pieces.app/extensions-plugins/obsidian?utm_source=dev-to&utm_medium=banner&utm_campaign=dev-to-site&bb=59778)

Read next
---------

 [![](https://media2.dev.to/dynamic/image/width=100,height=100,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F920309%2Fadb29bf4-2cd0-4c21-b6ba-24cbd1a344d8.png) 

### 12 Essential AI Tools for Web Development to Boost Your Projects

Kafeel Ahmad (kaf shekh) - Jan 4](/kafeel_ahmad/12-essential-ai-tools-for-web-development-to-boost-your-projects-hjg) [![](https://media2.dev.to/dynamic/image/width=100,height=100,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F2461160%2Fefda9ea8-49f8-4d07-b358-445b8e7d5a20.png) 

### Generating Permalinks in VS Code Using hogashi.vscode-copy-github-permalink

John Ajera - Dec 1 '24](/jajera/generating-permalinks-in-vs-code-using-hogashivscode-copy-github-permalink-4p5c) [![](https://media2.dev.to/dynamic/image/width=100,height=100,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F2332623%2Fdac61bf7-de2d-4c03-b9dc-8f41c8a3f097.png) 

### 🛠️ 25 Must-Have Golang Tools and Libraries You’ll Actually Use for Everyday Coding

0x3d Site - Jan 3](/0x3d_site/25-must-have-golang-tools-and-libraries-youll-actually-use-for-everyday-coding-4gi1) [![](https://media2.dev.to/dynamic/image/width=100,height=100,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F170161%2F065bcc7a-446e-4433-ad63-2fa5fa85bba2.jpg) 

### De pleno para senior: o que está faltando?

Jessilyneh - Jan 3](/jessilyneh/de-pleno-para-senior-o-que-esta-faltando-568l)

 [![](https://media2.dev.to/dynamic/image/width=90,height=90,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Fuser%2Fprofile_image%2F562514%2F7190202a-5745-402c-8e42-00c23604a6fc.jpg)  Adam Braimah](/adam_b) 

Follow

Senior software engineer. Book, vinyl, sneaker, and headphone accumulator.

*   Location
    
    UK
    
*   Education
    
    BSc (Hons) Computer Science, University of Manchester
    
*   Joined
    
    Jan 18, 2021
    

### More from [Adam Braimah](/adam_b)

[Code Review Anti-Patterns

#productivity #career #developers

](/adam_b/code-review-anti-patterns-2e6a)

[![](https://media2.dev.to/dynamic/image/width=64,height=64,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Forganization%2Fprofile_image%2F18%2F84b10f94-6f62-4b6b-9bdd-0df3eb1eea65.png)

Twilio

](/twiliotemphideme)Promoted

Dropdown menu

*   [What's a billboard?](/billboards)
*   [Manage preferences](/settings/customization#sponsors)

* * *

*   [Report billboard](/report-abuse?billboard=204128)

[![](https://media2.dev.to/dynamic/image/width=350%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fi.imgur.com%2FTcMGJiS.png)
](https://www.twilio.com/code-exchange?utm_source=buysellads&utm_medium=cpc&utm_campaign=bsa_brand-developer_acq_emea_en_devto_ungatedcontent_static&utm_content=brand-developer_codeexchange_ungatedcontent_static_v1_h1_c1&bb=204128)

[](#turn-code-into-relationships)[Turn Code Into Relationships](https://www.twilio.com/code-exchange?utm_source=buysellads&utm_medium=cpc&utm_campaign=bsa_brand-developer_acq_emea_en_devto_ungatedcontent_static&utm_content=brand-developer_codeexchange_ungatedcontent_static_v1_h1_c1&bb=204128)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

You bring the vision, we have the code.

[Learn more](https://www.twilio.com/code-exchange?utm_source=buysellads&utm_medium=cpc&utm_campaign=bsa_brand-developer_acq_emea_en_devto_ungatedcontent_static&utm_content=brand-developer_codeexchange_ungatedcontent_static_v1_h1_c1&bb=204128)

👋 Kindness is contagious

Dropdown menu

*   [What's a billboard?](/billboards)
*   [Manage preferences](/settings/customization#sponsors)

* * *

*   [Report billboard](/report-abuse?billboard=126494)

Close

Explore a sea of insights with this enlightening post, highly esteemed within the nurturing DEV Community. **Coders of all stripes** are invited to participate and contribute to our shared knowledge.

Expressing gratitude with a simple "thank you" can make a big impact. Leave your thanks in the comments!

On DEV, **exchanging ideas smooths our way** and strengthens our community bonds. Found this useful? A quick note of thanks to the author can mean a lot.

### [](#-cta-httpsdevtoenterstatenewuser-)[Okay](https://dev.to/enter?state=new-user&bb=126494)

Thank you to our Diamond Sponsor [Neon](https://neon.tech/) for supporting our community.

[DEV Community](/) — A constructive and inclusive social network for software developers. With you every step of your journey.

*   [Home](/)
*   [DEV++](/++)
*   [Podcasts](/pod)
*   [Videos](/videos)
*   [Tags](/tags)
*   [DEV Help](/help)
*   [Forem Shop](https://shop.forem.com/)
*   [Advertise on DEV](/advertise)
*   [DEV Challenges](/challenges)
*   [DEV Showcase](/showcase)
*   [About](/about)
*   [Contact](/contact)
*   [Free Postgres Database](/free-postgres-database-tier)
*   [Guides](/guides)
*   [Software comparisons](/software-comparisons)

*   [Code of Conduct](/code-of-conduct)
*   [Privacy Policy](/privacy)
*   [Terms of use](/terms)

Built on [Forem](https://www.forem.com) — the [open source](https://dev.to/t/opensource) software that powers [DEV](https://dev.to) and other inclusive communities.

Made with love and [Ruby on Rails](https://dev.to/t/rails). DEV Community © 2016 - 2025.

![](https://media2.dev.to/dynamic/image/width=190,height=,fit=scale-down,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F8j7kvp660rqzt99zui8e.png)

We're a place where coders share, stay up-to-date and grow their careers.

[Log in](/enter) [Create account](/enter?state=new-user)

![](https://assets.dev.to/assets/sparkle-heart-5f9bee3767e18deb1bb725290cb151c25234768a0e9a2bd39370c382d02920cf.svg)
 ![](https://assets.dev.to/assets/multi-unicorn-b44d6f8c23cdd00964192bedc38af3e82463978aa611b4365bd33a0f1f4f3e97.svg)
 ![](https://assets.dev.to/assets/exploding-head-daceb38d627e6ae9b730f36a1e390fca556a4289d5a41abb2c35068ad3e2c4b5.svg)
 ![](https://assets.dev.to/assets/raised-hands-74b2099fd66a39f2d7eed9305ee0f4553df0eb7b4f11b01b6b1b499973048fe5.svg)
 ![](https://assets.dev.to/assets/fire-f60e7a582391810302117f987b22a8ef04a2fe0df7e3258a5f49332df1cec71e.svg)

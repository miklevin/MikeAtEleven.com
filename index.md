--------------------------------------------------------------------------------
## Fri Aug 20, 2021

Hello World! It's Mike At Eleven! I just launched that website yesterday with
the intent of doing some live streaming (or at least content releases) on my
channels (usually YouTube but others soon) at 11:00 AM and PM. And here I am 11
AM the next day... woot! We'll see if it sticks.

I'll often do silent journal streaming like this, for I'm sure an audience of
almost no one. But I always have things on my mind and am fine with thinking
out loud to myself, and in this case some potential audience because YouTube
lets me, so hey, why not? It could be the thing that sticks.

Whether or not it sticks, it certainly can be the catalyst for other things.
The first rule of making stuff happen is to capture your ideas and begin the
process of actualizing. An idea is more real merely by virtue of writing it
down. In the information age such as we're in, it actually is real in the sense
that it's published and shared content that's consumed by other people, plaid
back in their heads, and that makes it real in at least the sense that stories
are real. It's no longer locked away.

Okay enough of that. Let's get down to some actual actualization. 1, 2, 3... 1?
Well, it's really the work day and I'm just taking a short break for this. And
so I think through what goes next naturally on this site. I work dramatically
differently from most people, and that makes a lot of difference in how useful
I am professionally and even how I think in my personal life.

For example, vim. Can you imagine just thinking out loud to yourself like this
in VSCode? Where would you begin? Where I begin is in a github repo. It's
actually a git repo that happens to be stored in a private repository on
Github. Many folks treat git and Github like the same thing. They're not.
Github is a community site built up around the git program written by Linus
Torvalds to help with Linux kernel development. Github is a site that sprung up
around the git program because even though git is already a DISTRIBUTED
revision control system, one of the places that's nice to distribute your code
is to a "centralized" location that you can always push to and pull from for
backup, undo and switching machine locations. Forget about developer
collaboration for a moment.

Let me demonstrate...

There! Now all my latest journal changes are in Github. Now I don't actually
publish my daily journal even though I back it up to Github. It's in a private
repo and I only publish excerpts. One place I publish them is to:

    MikeAtEleven.com

HERE! Or soon to be here. How do I do this? I add another vim buffer. Observe:

It's in my 2nd vim buffer now which I can cycle to with:

    :n

Observe...

That was my entry from yesterday. But I want today's entry over there too. And
so today's "At Eleven" video will be about making a 2nd entry. Soon I will type
these things over in that journal (in defiance of my own 1-textfile-for-life
principle) for the sake of the site. 

And I will show you how my vim blogging macro works. But first...

--------------------------------------------------------------------------------
## Thu Aug 19, 2021

Hello World! This is a silent live stream. I'm planning on getting a new
website registered and hosted with github.io publishing in the next few
minutes. It's all the "new way" for me. Recently I retired my WordPress site at
MikeLev.in and exported all the content as markdown which github.io pushes out.
It's not pretty yet, but it's also no longer on WordPress and besides my Github
membership, I have no hosting costs anymore. 

This is a live performance. Excuse any mistakes. But here we go looking up a
site we would like to register. My aspiration is to do some sort of video every
night or morning AT ELEVEN. So it will be Mike At Eleven. And because I'm
old-school, I'll use .com. I still think it's the best TLD baring any
overriding reasons to do otherwise (like MikeLev.in). 

I may end up starting from this point...

I re-started this live-stream. Getting a hang of how this works. Just installed
OBS and my stream key from YouTube for the first time on this new laptop.
Registered a new domain: Mike At Eleven... mikeateleven.com. Now it's time to
activate it on github.io. 1, 2, 3... 1? Set up the DNS...

Github includes "free" web hosting. You can resolve a domain to a repository
branch. Most people host it at reponame.github.io but or use a
www.registered.com. I actually plan to resolve to the "apex" domain, aka the
registered domain without a www or other subdomain. We do that with a series of
A Records with the "@" symbol as host... Okay we've got our 4 DNS entries. But
it's resolving to Github now with it having no idea where to send the traffic.
So let's do a before/after...

I should have done a before/after BEFORE that. You can now see that it's
resolving to Github. Otherwise it would have been an even more generic error
about no DNS or no site found. Let's make a repo...

I use my Windows Home / github folder so much I default my terminal program to
cd into it. Now I make a new folder there with the same name as the site...

So I simply made a mikeateleven folder, created an index.html file in there and
added it to the repo and committed it. Oh yeah, I also initialized the folder
AS a git repo with git init. So far no actual Github... just git the local
program. Let's push the repo to Github...

We name our branch as main...
We set the address of our remote repo location...
And finally we do our first push that needs a little more info than usual...

After that, you can just use "git push".

Anyway now we tell it's a github.io page. Github recently promoted the feature
onto their submenu...

This is the first time I used a plain index.html. It shouldn't be a problem. If
it is, I'll switch to an index.md (markdown) which will make the jekyll system
kick in.

Okay, a few things. I added the domain through this area which by the way is:

Repo / Settings / Pages

That www warning is not important because we're not using www. We're resolving
the site to the apex domain (no www).

And there we go! We went from just registered domain (moments before this
video) to a Hello World index.html in a few minutes. Recap...

1. We add the 4 github.io DNS entries at our registrar that provides DNS
   services. NameCheap in this case (recently switched everything off of GoDaddy)
2. We create a local repo and then push it up to Github.
3. We go into that Repo's Settings at Github and select Pages and set a few
   things including the registered domain we're using.
4. After a few minutes you can activate "Enforce HTTPS" which makes the site
   more secure and better for SEO (eliminates "2nd version" of the site).

Okay, it's still a very plain text file which you can see from view-source...

That's nothing different than I typed into my text editor vim. But we want to
make it real HTML and also pretty. So we can select a theme.

That won't work on a .html file. It has to be markdown. So we'll git rename
index.html to index.md...

That was weird. Anyway what happened was this...

I accidentally made my git repo at Windows Home / github instead of /reponame.
And so I copied the files I knew belonged in there back in, including the .git
(invisible) directory that gets created when you git init. I also did a git
pull because once you choose a theme and set a domain Github automatically puts
a few files in your repo... so I had to do a git pull before I could commit and
push my local changes. 

I should have pushed while I was explaining all that because it takes a few
minutes for the Github.io Jekyll system to recognize your new .md files and
stylize them. It could be done by now...

See how it all has a look now? Even though the file looks like plain markdown
locally, when you push it there's a system that converts it to richer html.
Okay, let's do our first real entry there. Let's make it this whole entry. I
might change it later, but my plan is to do something like this (live YouTube
broadcast for example) every day at eleven either AM or PM.

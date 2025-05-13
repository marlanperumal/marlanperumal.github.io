---
layout: post
title:  🥚A parting easter egg to kick things off
date: "2025-05-13"
tags: ai coding games
---

In the last week at my previous job at Eighty20 Consulting, my partner set up a cute little game where she'd send me some thoughts and ideas about the end of my time there. I could choose, whether they would be funny, mindful, kind, naught or academic. One of the "naughty" ideas was

> Hide random notes around the office in places where they'll only be found weeks or even months later. Write things like 'I know what you just did' or 'It wasn't like this when \[your name\] was here

![post-it](/assets/images/Pasted image 20250513162820.png)

I thought this was great and spent my last evening "working late", writing up silly little things on post-it notes and finding cunning places to hide them. Nearing the end, my creative juices all but spent, I wrote down a url [https://eighty20.stuntedchicken.co.za](https://eighty20.stuntedchicken.co.za) and a date (exactly 1 month later).

I owned the domain `stuntedchicken.co.za` but there was nothing at the `eighty20` subdomain at the time. It was a nifty little placeholder but I didn't really know what I was going to put there. I'd given myself a 1 month buffer till that date, when I figured people would understand to mean when to go look there.

Over the next couple of weeks, I threw around a few ideas of what to put there, ranging from an essay, to a video or song but I quite liked the idea of building a little game that my former team members could play. Random little puzzles and challenges were one of the great parts of our company culture and I'd previously built a couple of web app games for us before (a football world cup predictor, a mastermind type game and a couple of others that I've now forgotten).

I fully intended though to spend my first month of "retirement" doing as little as possible, and as much as I was looking forward to using my upcoming available time to write code and build things, that would need to wait until I got all the bumming around out of my system in that first month. So I took the lazy person route and asked ChatGPT.

One of the things I knew I needed to learn how to do better was use AI tools to take care of simple tasks and fast track my way around things I didn't know very well yet. I'd gotten as far as envisioning a game where, taking a pointer from the name, a user would be presented with a screen full of randomly positioned dots and they would need to draw a line that splits them into 2 regions containing and 80% and 20% of the dots respectively. This seemed a simple enough premise, with enough "almost, let me try again" pull to it. I duly asked ChatGPT to built it and was very pleasantly surprised with what it produced on the first shot. A single follow up prompt and it was almost exactly what I wanted. (Here's the [conversation](https://chatgpt.com/share/682359ff-1c64-8000-8399-ed172fb6ee45) for reference)

![initial-screenshot](/assets/images/Pasted image 20250513163644.png)

Mission almost complete with time to spare until my self-imposed deadline. Looking at the code I'd been handed though revealed the flaw I'd been expecting in this approach. Although most of it was pretty straightforward, I didn't really understand the key bit that actually drew all the dots and the line using the HTML canvas API, having never used it before.

I also had loads of ideas around adding a login with a leaderboard, with different game types extending the basic dots and line them, but (and I know many will be ridiculing me for this), I didn't really know how I would implement any of that in a simple vanilla HTML and JS site like this. I hacked myself into frontend web dev via React and completely skipped over the basics of using `document.getElementById()` etc. and I'd need to wrap my head around what should have been a preceding mental model.

Not to be deterred from my slacker AI first approach though, I'd just heard about v0 and cursor, fired those up and vibe coded my way to a 2nd iteration that looked marginally better and should allow me to build in all those cool new features I had in mind. It was all built on top of Nextjs, which was complete overkill but since this was also something that I wanted to learn (I'd only previously used React for fronted SPAs), that was fine by me.

And here's the result - you can check out the actual game at [https://eighty20.stuntedchicken.co.za/](https://eighty20.stuntedchicken.co.za/) and the code is on [Github](https://github.com/marlanperumal/eighty20-split). I must say that I was incredibly surprised by this initial experience, of how simple it was not only to build the app but deploy it (for free!) on Vercel (other hosting providers are available). As it turned out I never actually returned to this project to add any of those new features and I doubt if any of my former colleagues actually ended up finding and playing even this initial version, but it was a good excuse and a nice little intro to the projects I'd build after that.

![final-screenshot](/assets/images/Pasted image 20250513170036.png)
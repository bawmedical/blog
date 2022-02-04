## There’s no such thing as a free Launch (or maybe there is)… Launchers on Linux in 2017

The winner — Albert Launcher — on Linux Mint 18.2

> **Confession: I once owned a MacBook Pro.**

There was once a time when I just *had* to try a Mac and see what all the fuss was about. In the end I came back to Linux (yes, really. Long story). But MacOSX left one permanent mark on me — I learned the productivity-enhancing value of **application launchers** like [Spotlight](https://en.wikipedia.org/wiki/Spotlight_%28software%29) and [Alfred](https://www.alfredapp.com/).

When I came back to Linux I looked around for a nice-looking, customisable launcher, and although there is a lot out there, Linux launchers aren’t *quite* up to the standard of Alfred yet. Nevertheless, it’s all free software (whereas Alfred cost me money) and so I spent some time auditioning launchers both for my personal use and for inclusion in the NHSbuntu distro. *(Why do I want a launcher for NHSbuntu? That’s another blog post, coming soon!)*

I thought I’d share the results of my hunt for a free launch here. I had some loose criteria for what’s a ‘good’ launcher for NHSbuntu, which I’ve listed at the bottom of the article.

> For those not familiar with launchers — a launcher is a text box which pops up when you use a particular key combination (often Ctrl + Space, Alt + Space, anything that is very quick and easy to execute). You can then type into the text box to launch applications, find files, play music, execute shell commands, search the web, and many other activities. **It keeps your hands on the keyboard** and makes it fast and easy to switch tasks, open new browser searches, and accomplish tasks.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725785439/2K7v8Th0F.png)

A launcher (in this case [uLauncher](http://ulauncher.io/))

Here’s my run-through of the available options for cross-platform launchers on Ubuntu Linux. Your mileage may vary, and your comments are welcome.

### [Synapse](https://launchpad.net/synapse-project)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725787214/h2Le4PQPi.png)

Synapse launcher

*   For a long time this is what I used for my own system, I have since then ‘auditioned’ every launcher on this list that I could get to work. Synapse remains a solid and great launcher.
*   **Pro**: very fast, no noticeable keystroke lag, searches through your ‘last used documents’ to rapidly suggest applications, documents, and web searches.
*   **Con**: written in **Vala** ([Wat?](https://www.destroyallsoftware.com/talks/wat)); documentation isn’t inviting to the new potential contributor; not particularly responsive to feature requests from what I can see; code is managed on Bazaar & Launchpad (as opposed to GitHub) which makes it harder to get involved (for me at least); Limited appearance/skinning options.
*   **Suitability for NHoS:** Moderate-High

### [Zazu](http://zazuapp.org/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725789029/GWt84jIwc.png)

Zazu — a self-confessed Alfred clone, but beautifully done, cross-platform, and incredibly extensible.

*   **Zazu** is a relatively new entrant, being based on based on the [Electron](https://electron.atom.io/) cross-platform native application framework and is written in Javascript/HTML/CSS. Named after the Rowan Atkinson character from the Lion King, apparently.
*   **Language:** Javascript
*   **Pro**: Looks beautiful, incredibly extensible, great documentation, responsive support from TinyTacoTeam, new themes easy to make, plugins also easy to make.
*   **Con**: Noticeable keystroke lag and delay in popping up
*   **License:** MIT
*   **Suitability for NHoS:** High

### [Albert](https://albertlauncher.github.io/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725790794/1ede4_Xng.png)

*   **Language:** C++, Qt5
*   **Pro**: Fast performance, extensions can be written in Python, project is updated regularly and is managed on GitHub, comes with a LOT of really nice UI themes OOTB, very responsive development team
*   **Con**: It’s still ‘officially’ in Alpha (0.14.8 at the time of writing) but it’s very very stable even so.
*   **License:** GPL
*   **Suitability for NHoS:** **It’s what we’re going with!**

### [Ulauncher](http://ulauncher.io/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725792485/FDsWYJBDt.png)

Ulauncher on Linux

*   **Language:** Python
*   **Pro**: Fast. written in Python and it’s easy to extend/add modules using Python. Adding custom browser searches was very easy, using the GUI editor. An active project on GitHub, with Gitter support.
*   **Con**:
*   **Suitability for NHoS:** Moderate

### [Unity Dash](https://help.ubuntu.com/stable/ubuntu-help/unity-dash-intro.html)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725794230/QiZOqkGYT.png)

Unity Dash on Ubuntu

*   **Pro**: Looks nice, works very well with Unity I’m told
*   **Con**: Essentially tied to the Unity desktop environment, not standalone. It’s a pretty big Con I’m afraid. Especially with [Unity being retired from Ubuntu](https://arstechnica.com/information-technology/2017/04/ubuntu-unity-is-dead-desktop-will-switch-back-to-gnome-next-year/). Also all the transparency effects and animation are quite heavy on system resources.
*   **Suitability for NHoS:** None
*   **License:** GNU GPL v3 (I’m presuming - same as Ubuntu)

### [Kupfer](https://kupferlauncher.github.io/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725796137/muAG4ev3N.png)

Kupfer launcher

*   **Language:** Python
*   **Pro**: Code managed on GitHub, Python based makes it potentially more accessible for contributors from our community,
*   **Con**: Mainly aimed at Linux ie not necessarily cross-platform (would probably work on Win/Mac since it is Python, but might need hacking), Documentation sparse,
*   **Suitability for NHoS:** None
*   **License:** GNU GPL v3

### [Gnome Do](http://do.cooperteam.net/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725797742/z7x78fm_G.png)

Gnome Do on Ubuntu

*   **Pro**: Well, the screenshots look nice…
*   **Con**: It’s a dead project, [no recent updates on Launchpad](https://launchpad.net/~do-core/+archive/ubuntu/ppa) since ~2009
*   **Suitability for NHoS:** None
*   **License:** GNU GPL v3

### [Launchy](https://www.launchy.net/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725799472/sU4vQFVxij.png)

Launchy on Linux Mint 18 using default theme.

*   **Pro**: Nice launcher, cross platform, fast enough.
*   **Con**: It’s a dead project, [no recent updates on Launchpad](https://launchpad.net/~do-core/+archive/ubuntu/ppa)
*   **Suitability for NHoS:** None
*   **License:** GNU GPLv2

### [Dext](https://github.com/vutran/dext)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725804054/fYO-7I0qL.gif)

*   **Dext** is another cross-platform launcher app that is powered by the [Electron](https://electron.atom.io/) platform (Chromium browser + node.js). There are quite a few of these now and I don’t really have time to review them all here.
*   **Language:** Javascript
*   **Pro**: Visually great, lots of plugins and has its own CLI package manager for adding plugins. Lovely GIF animation of it in use is really illustrative to people who haven’t used a launcher.
*   **Con**: Slow performance (related to the limitations of Electron mainly); Also, it seems to be doing a very similar thing to Zazu and I wondered if they might be able to merge the projects in order to consolidate their user base and develop faster (in the long run), heavy on resources due to Electron, large download size — again due to Electron.
*   **Suitability for NHoS:** Moderate
*   **License:** MIT

### What makes a good launcher?

I’ve made some judgements about the launchers I’ve tried, based on some criteria that I think are important, but I accept that other people’s priorities are going to be different. I invite debate in the comments below.

*   **Cross-platform:** NHoS is a Linux-based operating system (available in Ubuntu flavour, RHEL flavour available soon!) — BUT I wanted to ensure that whatever launcher we chose for NHoS had cross-platform availability so that users who are using more than one OS in their work and home lives can use the launcher for everything they do. Cross-platform usually also means a larger user-base, better plugins, and more features.
*   **Extensible:** We are creating an OS for NHS clinical professionals — they might eventually find uses for their launchers that we haven’t even imagined yet — we’d expect a good launcher to allow extensions to be written in some fairly accessible programming language (eg Python, Javascript, Ruby)
*   **Fast:** I can’t recommend an option that is laggy on my *own* machine (a fast laptop) when much of the NHS uses very old and slow machines which we want to speed up by using a lightweight linux.
*   **License:** The license selected by the project needs to be fairly compatible with our base distro (ideally it should be GNU GPL v3 like Ubuntu)

I hope this article has explained our thinking behind selecting the Albert Launcher for NHoS.

If you’ve enjoyed this article then please do share it.

Comments, as always, are welcome.
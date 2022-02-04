## Why we chose Python for the RCPCH Digital Growth Charts project.

So here is a little bit of a ‘stream of consciousness’ blog post I felt compelled to write, about why we chose Python for the RCPCH digital growth charts API. Not everyone will be interested in this, it’s here more a geeknote than anything.

[https://github.com/rcpch/digital-growth-charts-server](https://github.com/rcpch/digital-growth-charts-server)

We knew that we were going to build an API server. And we knew at some early point we were going to have to pick a technology with which to build a server. And there are many, many programming languages we could use. And, of course, there are many, many ‘holy wars’ about which programming language is best, most performant, easily understood, etc.

And of course, there’s our own skill sets as programmers, the kind of languages we’re familiar with. My personal favourite language is Ruby, but this is often regarded as a poorly-performant, niche language for people who were last cool in 2005. (Rubyists know that brains are expensive and CPU cycles are cheap, so expressivity and developer productivity beat pure performance every time but hey…)

Simon, a paediatrician and coder, who with me has shared the task of writing the server and demo clients, has experience in Android development and JavaScript. And we knew we would need to build a JS app as a demo at some stage. So we did consider Node/JS for the API server as well. But it didn’t seem right to be building a maths-heavy API in node.js/JavaScript, given that JS has always been notorious for problems with its floating point handling. I’m sure that’s all probably all fixed now, but still. FUD, eh. It sticks.

#### Accessibility and learning curve

One of the early considerations was that we wanted to open source this, and we wanted to make sure that that open source code was easily ‘accessible’ to other clinicians who might want to read the code. Firstly, they can point out our bugs. And, secondly they provide independent peer review of the code.

I’m a firm believer that clinicians can learn to code, which doesn’t have to mean that they’re going to be writing entire electronic healthcare record applications, but what they can do with that skill is use it to solve small problems like a clinical calculator or some other similar thing.

So I didn’t want to use is a language that has a very high initial learning curve, or requires a very complex development environment, compilation steps, or other things that will dissuade the initial user or reviewer.

Python is one of those great languages where you can open the command line type ‘python’, and you’re using Python.

They teach Python in my children’s high school, which I think is that is a good sign in terms of accessibility — if school children can learn this as their first language, then that’s a great thing.

A few years back I’d used a lot of Python with Open Health Care UK and their platforms built with the (Django-based) Opal framework, so I knew enough Python to quite like it. Not as much as Ruby though… 😉

#### Adoption and stability

Python is the de-facto language of the scientific, research and bioinformatics community, where it’s very well adopted, it’s been around for 30 plus years. And it’s currently on Python 3, so it’s gone through a lot of its initial growing pains and is now quite a nice stable language.

It’s used by big players such as Google, and other organisations including the NHS spine, which runs on Python API’s. There’s a lot of Python at Microsoft. So this is a hugely popular language. It’s not going to disappear on us, or disappear off into an AngularJS style major-version arms race.

#### Standard libraries and webbish stuff

And so the other reason we chose Python is that it’s got a fairly well developed set of standard libraries, so that where we were using libraries, we will be using ones that are maintained by the Python Software Foundation, and not third party libraries that are not necessarily going to have long term support or bring us problems long term.

Although a lot of the calculations are statistical, we needed a language which had the full range of Web tools for building a performant and secure API, so we couldn’t have used more traditional stats languages such as R. Although our testing fixtures are developed in R.

Prof. Tim Cole, who designed modern UK growth charts back in the 1990s is chief tester, and he used R to generate fictional children and measurements with known centiles and SDS scores, and we would then throw these at the API and compare the results till be got perfect accuracy.

Of course, the design of our API means that our future work doesn’t necessarily have to be in the same language. And users of the API don’t need to care at all what it is written in — they use their preferred language to access accurate growth chart data via the REST API.

We’d love to have feedback on this idea and hear your views on this choice. I’d love to know what other technologies we could have used, maybe when we’re on 2.0 we’ll give them a try!
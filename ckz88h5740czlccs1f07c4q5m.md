## Why the TRUD must die

The TRUD (Terminology Reference and Update Distribution) — artist’s impression

I’m sorry to be the bearer of bad news, but the way that NHS Digital communicates standards and interacts with its developer community doesn’t belong in the 21st Century. It has to change.

#### What is wrong

It’s 2018 and the breathless health-tech fangrrls and fanbois are quite rightly wondering where we are up to with delivering a whizzy hooked-up app ecosystem supporting self-care, video-consultation, online booking for everything and all kinds of other nice things, all integrated with NHS systems — *because we don’t want silos do we?* — and all compliant with standards.

We’re wondering why funky startups don’t enter the market with new systems, and why developing new functionality for existing systems takes unbelievably long periods of time and is stupendously expensive.

Hmmm.

And then you look at the state of the documentation for those standards and NHS services, and you realise why.

They are *hidden* — and when you find them, they’re impenetrable — and it’s apparent that there is no intention to be helpful within those documents.

Say you’re a greying yet dashing clinician/developer intent on building a **new, transformative, disruptive open source GP clinical system** (no, I’m not building one. Or am I? No definitely not.). The specifications for implementing something you’ll definitely need to support, a transfer mechanism called [GP2GP](https://digital.nhs.uk/services/gp2gp), are buried in something called [TRUD](https://isd.digital.nhs.uk/trud3/) (Terminology Reference Update Distribution).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725773582/iBA67kTlO.png)

All sorts of modernity on display in the latest MIM version

It’s not a Terminology, but it’s in there anyway, at the bottom of the well. It’s in a thing called the [Messaging Implementation Manual](https://isd.digital.nhs.uk/trud3/user/guest/group/41/pack/1/subpack/28/releases). So you download the latest version (if you can call anything with an NPfIT logo on it ‘latest’). But what you need is not the latest version — no, that would be logical, but no — it’s in MIM Release 3.1.10 (Released 30 March **2005**). More recent MIM documents don’t have GP2GP in there. Whuh?

The most recent release of the MIM (Release 7.2.02, April **2008**) proudly carries the logo of the *National Programme for Information Technology (NPfIT)*, a programme that was [**officially abandoned** nearly 10 years ago](https://en.wikipedia.org/wiki/NHS_Connecting_for_Health), and famously was o[ne of the most expensive and disastrous IT projects in human history](https://www.theguardian.com/society/2013/sep/18/nhs-records-system-10bn). Some versions even have the *Connecting for Health* logo — another defunct brand. It’s hard to have confidence in documentation so derelict.

These are all *current* specifications that are needed for new products to be accepted as GPSoC products, and provide business-as-usual functionality in GP systems and across the wider NHS. They will be requirements for any new entrant under the new [£450m GP IT Futures](https://ted.europa.eu/TED/notice/udl?uri=TED:NOTICE:348994-2018:TEXT:EN:HTML) framework, so we will want to make compliance as easy as possible, right?

This is how NHS Digital looks from the outside to developers. Not a modern, self-aware, and positive organisation but as an awkward, irritable, adversarial organisation — “no we are not going to be helpful, we’re going to make finding the specification you want as bloody difficult as possible”

#### Why can’t this specification just be on the open internet?

Even in 2008, at the time of release of the final MIM, the Internet was no infant. Twitter and GitHub both existed and e-commerce and e-banking was thriving. What is it about the nature of our organisation that means we need to hide specifications away in an obscure part of an obscure site?

### So, how do we fix it?

How to start fixing this mess boils down to two words:

1.  **Developer.**
2.  **Experience.**

Developer Experience. We need to start believing that the users of that documentation **matter**. We have to think about the overall ‘developer experience’ they have using that documentation.

> None of the NHS’ tech is so unbelievably complicated that it can’t be made easier to understand and to implement.

One of the reasons that our NHS tech infrastructure costs so much and is so dominated by a few massive incumbent suppliers is **our own fault** for making it so hard to develop against these specifications and standards. Newcomers just don’t stand a chance.

### We need to [‘**do the hard work to make it simple’**](https://www.gov.uk/guidance/government-design-principles#do-the-hard-work-to-make-it-simple)

What does that mean? It means we need resources to develop and provide things that help others integrate with NHS Digital services.

*   Freely available, open source reference implementations of all standards.
*   Open source client library code for multiple programming languages — targeting not just those we know are used by existing incumbents — often ‘Enterprisey’ languages like .NET and Java — but targeting the languages used by the modern Web and by the kinds of organisations we want to *encourage to get involved in NHS tech:* not an exhaustive or unarguable list, but here goes: Swift for iOS, Javascript, Kotlin and Java for Android, Ruby, Python, Go, and yes, I’m sorry, PHP)
*   Online documentation that we can be proud to show to developers and our mothers.
*   Open, public forums in which NHS Digital staff are encouraged to spend time and reply to queries, building a community of interest
*   People working on these technologies — be they technical architects, software engineers, clinicians, or delivery team — need to be free to **blog** about their work, share successes and failures, teach and learn at conferences, and be part of their community.
*   Regular hackathons like the excellent Inaugural INTEROPen hack day in November 2018, which brought together NHS Digital services with dozens of startups and vendors

This is tantamount to a **complete digital transformation** of the NHS’ developer culture and web presence.

### Some examples of how to do it well

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725775151/lZttpccbXq.png)

[developer.nhs.uk](http://developer.nhs.uk)

[developer.nhs.uk](http://developer.nhs.uk) is an excellent example of the way forward. Taking this as a beacon, more technical resources need to be applied to translate, revise, and update old documentation like the MIM into clear, intuitive, developer-friendly pages like the above.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1643725777375/7bgiaERVM.png)

[NHS.UK Service Manual](https://beta.nhs.uk/service-manual/)

The new [NHS.UK design principles](https://beta.nhs.uk/service-manual/design-principles/) and [Service Manual](https://beta.nhs.uk/service-manual/), and the [NHS.UK Frontend](https://github.com/nhsuk/nhsuk-frontend) are also welcome and impressive pioneers of great documentation and a developer experience that parallels other government design agencies and follows tech-industry expectations.

### In a way right now the NHS is lucky. It doesn’t actually need to ‘invent’ anything in order to innovate.

All we need to do is **look at what the rest of the ‘normal’ tech world is doing** and implement those standards and cultures and norms.

Out in the ‘normal’ world of tech, if you have an API and you want people to use it, then:

*   **Do:** Document your API on the open web, in an engaging and interesting way that shows people what they can DO with it, and leads them through the learning journey, from ‘Getting Started’ through to ‘Contributing’.
*   **Do not:** Start with a UML diagram, document control grid, arcane versioning, or the Connecting For Health logo
*   **Do:** Provide client libraries to make integration faster (and of course by providing the implementations you can make sure they work the way your API would want them to work).
*   **Do not:** expect each and every organisation integrating with your API to start entirely from scratch, building a ground-up, hand-knitted implementation, each with its own special bugs. (And paying them each to do so)
*   **Do:** Provide instant signup to the developer portal, immediately-available API keys, and free ‘dev/test’ usage of the API; if not a free usage tier as well.
*   **Do not:** make them email servicedesk@whatever.nhs.uk to get access to an undocumented test environment, in 2 weeks’ time
*   **Do:** Engage directly, openly and honestly with the developer community to help you — they will: build libraries for less-common languages that you don’t have resources to write for… Comment on and update your documentation… Be your social media fan base… Fix bugs in your API codebase… Talk about your API at conferences for you…

So that’s why the TRUD must die.

If you enjoyed this diatribe, you may enjoy other diatribes I have written on Medium.

Thanks for reading.

Marcus
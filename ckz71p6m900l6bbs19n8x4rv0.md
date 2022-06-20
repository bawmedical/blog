## Being Outspoken Works!

Hi. My name is Marcus Baw and I'm a GP and software developer mainly working in the UK health technology and NHS clinical informatics area. I'm known for a few things, one of them is being a bit outspoken in meetings and blogs. As I stepped down from the Chair of RCGP's Health Informatics Group last week, the team I've been working with described me as "Always Willing To Offer An Opinion" (which I'm getting made into a T-shirt, by the way!), and which I'm taking as a compliment!

I am (sometimes) outspoken, *not* to upset people, but to get **change** to happen. Whilst we're here, I'll just clarify that I'm also not some brutish infantile troll who has a Twitter bio that reads something like "I say what I like, taking offence is your choice". I hate that childish attitude. I'm all about a reasoned argument of **why** the status quo won't do, a change-enabling story, and if I can give you my thought on *how* to fix it - I will.

Recently I've been shown a great example of that 'getting change to happen' really working, and I wanted to put some thoughts out there about being outspoken and why I think it works. It's mainly a story about the NHS - because that's what I know, but much of what's here would apply in almost any organisation.

## 'The TRUD Must Die'

About 4 years ago I wrote a blog post called ["Why the TRUD Must Die"](https://marcus-baw.medium.com/why-the-trud-must-die-ac27377ee189) - it was a bit of a rant about the terrible state of the documentation for NHS Spine services, which were languishing hidden in a website called the TRUD ([Terminology Reference Update Distribution](https://isd.digital.nhs.uk/trud/users/guest/filters/0/home) - something that was *originally* designed in the [NPfIT](https://wolandscat.net/2018/10/28/why-npfit-failed/) days to distribute medical terminologies like Read Codes, and advise the system suppliers implementing them that there was an update).

I'd been simply stunned of the appalling state of the 'Messaging Implementation Manual' which was meant to be the documentation for developers integrating with NHS Spine and related national services. It was dated looking, still branded ***NPfIT*** and with a 'Connecting for Health' logo, and the numerical versioning had nothing to do with the highest version being the correct version containing all currently available services. Barmy.

## Boom! Like that.

That blog post attracted a little bit of criticism at the time, and some of the responses were gently patronising, suggesting that (as ever) this was user incompetence, I didn't know what I was doing, this is the way they've always done it, and if I would just settle down and get a job at NHS Digital then in a mere 20 years this jumble sale of documents would all make sense to me, I'd be on the inside, and we could all go back to sleep and leave things as they were.

I didn't hold out much hope of significant change, but hey, I'd at least got it off my chest, and frankly that is half the fun of being outspoken. I've got an actual email folder labelled 'Best Rants Ever'. It's a rush, pressing send on something that (in my own assessment of course) highlights the problem and solution with a laser focus.

## "Nasty blog does good"

I know from conversations I've had with NHSD staffers that this 2018 blog post was read and shared inside NHS Digital, and, while maybe not everyone agreed with it, and some hated it, for others it was used not just as a call to action, but in some ways a bit of a recipe book for what needed changing, and **What Good Would Look Like**.

In the intervening years, I'd made friends with some of the NHS Spine API team, and they actually came to the 2020 Rewired Health Developer Conference which I ran in March 2020, just before COVID locked us all up for the best part of 2 years. I got to see that they were developing a much better API developer portal and adopting the 'Developer Experience' and documentation standards that have been common in the rest of the tech world for a decade now.

## Follow-up call: January 2022

Last week I was invited to a follow-up call with the NHS API documentation team, where they showed me the current API Developer Portal, and line-by-line they compared things I said in the [TRUD Must Die](https://marcus-baw.medium.com/why-the-trud-must-die-ac27377ee189) blog with the TRUD at the time and then with the new API Developer Portal.

I was invited to explore the documentation and the signup process and give feedback, and I walked through the process of sending an API call using the industry-standard and beautiful Swagger documentation, and getting a response from an NHS Number lookup (A PDS Trace, using the FHIR PDS API). All in just a few minutes.

This represented not just a massive sea-change in organisational culture, but an epic feat of implementation, documentation, and harmonisation so that all these APIs are visible, discoverable, and easy to understand.

You can see the new API Catalogue pages here
https://digital.nhs.uk/developer/api-catalogue

I want to be clear that I'm not taking the credit for this change, or for the years of hard work put in by the NHS API team, their leadership, or the final output. I'm kind of just pointing out that sometimes being outspoken can help to get the outcome that's needed. At the very least, it didn't make anything worse. Yet sometimes we are dissuaded from being as outspoken as we feel we should be, because of so many cultural and even 'professionalism' related constraints.

**I'm here to argue that NOT speaking out when change is necessary is the MOST unprofessional you can be.**

## The Importance Of Being Honest

With that in mind, I have some thoughts and advice for aspiring outspoken change agents:

* **BE outspoken"**. The only thing worse than an unpalatable truth being called out is an unpalatable truth that is never called out! Get the message out and use any tools you have to get the message through to the people who need to hear it.

* **Don't fear the ZOUD ** - *the Zone Of Uncomfortable Debate* - a term I learned from my good friend and inspiring health tech leader Joe McDonald - a person who himself was 'let go' from the National Project for IT for what he describes as Career Limiting Frankness.
<br/>I guess this does highlight one of the downsides of being outspoken, which is that it can cause the machine to react against you and it can have negative career consequences. Protect yourself in whatever way you can, but also remember that the more of us are outspoken, the greater safety in numbers we have. Acknowledge it openly, and welcome it, when the conversation has entered the ZOUD. This helps everyone realise that we're **all** feeling uncomfortable, it's not just them, they're not being singled out for admonishment. The first step to fixing a problem is to acknowledge that there **IS** a problem.

* **Change isn't an inside job.** The truism often peddled "It's easier to change things from the inside" is not really true. You need both, certainly in this example you need both the people on the inside who can make the changes, and the call to action catalysing change from the outside. Often the source of the criticism needs to be from an outside, 'deniable' source. An internal person couldn't **possibly** say what I said, even if they believed it. The organisation's immune system known exactly what to do with internal whistleblowers - persecute, execute, eject.  In this case, as a non-employee of NHS Digital, although I have no genuine 'authority' or influence in the organisation, the 'soft power' came from the argument alone.

* **Play the long game.** It takes years for serious systematic and culture change. [In the case of NHS WiFi it took about 7 years](https://www.youtube.com/watch?v=BcGu7kMHz-I) to get from an attitude of (genuinely, I was told this) "Why would a clinician need WiFi access at work?" to "NHS WiFi is essential for accessing clinical knowledgebase and must be ubiquitous". Similarly in this TRUD case, 4 years is a relatively short time to get this far. An organisation cannot ever admit a brand new programme isn't successful. You have to wait a few 'half-lives' until the senior figures have moved on, the inherent problems are more apparent, the effect of the 'sunk costs fallacy' is waning, and the idea of change and improvement can be contemplated.

* **Be the 'critical friend'.** If the organisation you've criticised reaches out to talk to you more about your feedback, then this is often a good way to make friends and become that 'critical friend' who can then be the best of both worlds - trusted internally as a source of a good steer, and yet independent enough not to be affected by the power structures inside the organisation. However, if they ask you to delete or take down the criticism, this is a strong signal to you that they are not ready to engage constructively. **Call out this tactic** as being what it is - simple suppression of dissent, you know - a tool of a dictator, a totalitarian move. An organisation that is so thin-skinned that it can't survive debate is dangerously fragile and shouldn't be in charge.

* **Don't be afraid to upset some people.** It will happen. I've always been pretty outspoken but I will often caveat this by making it clear that I'm not doing it to upset people, I'm doing it to make things better. In a way it's about respecting those people's time and effort. Never attack individuals though, only challenge incorrect ideas, cultures, and practices. 
<br/>There **are** good, diligent, smart people working in organisations across health tech, but against their better judgement they are stuck in a programme of work that is a dead end. It is *out of respect for their time* that we are prepared to be outspoken, so that they can be working on the right things in the right way. The people who will be most upset are those with the most responsibility and power, usually. They can take it (or should be able to). The people lower down the command chain will often *agree* with your unpalatable truth, and by changing the conversation for them you can actually save them decades of wasted work. 

* **Abilene, the required watching after reading this.** The only way to get off the bus to [Abilene](https://www.youtube.com/watch?v=uFQ-ukyvAMk) is for someone to disagree with the current course of action, and (ideally) present a better one. As [Jerry Harvey points out in the first 20 minutes of this excellent talk](https://www.youtube.com/watch?v=uFQ-ukyvAMk), often as humans we do the wrong thing not because we can't manage our disagreements but because we can't manage our **agreement**. Essentially a meeting can become a multi-way politeness competition, in which the complex multi-dimensional human hierarchies conspire to let us all go somewhere that nobody wanted to go, and nobody thinks is a good idea.

* **Be positive.** Don't *only* criticise, you need to *inspire* as well - you have to present a **better** vision of the future, or how things could work better. In that TRUD Must Die blog, which I re-read as part of the call last week, and I had actually forgotten how much detail I'd put in there about what **good** developer experience would look like. The NHSD team actually walked me through my blog post and pretty much checked off my wish-list in their current API Portal. You've no idea how good that feels!

I hope this article is of help to *someone*, I wrote it partly in celebration of the immense improvement I've seen in the NHS Spine APIs and to congratulate that team for the incredible achievement. And the other part of writing it was to encourage and embolden any of you out there, however frustrated you are right now.

Change *can* happen, and this is one way to achieve it. Sometimes being outspoken can achieve what would be impossible with any amount of orthodoxy, any number of webinars, Strategies, limitless empty engagement and consultation exercises, and all the hot air in the NHS.

Marcus


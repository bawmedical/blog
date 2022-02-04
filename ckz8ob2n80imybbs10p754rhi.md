## Royal Colleges 3.0: ‘Best Practice As Code’

I’ve spent the last few months working with the [Royal College of Paediatrics and Child Health (RCPCH)](http://rcpch.ac.uk) on a project to deliver a [Digital Growth Charts web-service](https://growth.rcpch.ac.uk/). It’s been a hugely interesting project to help digitise the complex clinical logic of growth chart use into code.

As part of doing that work I’ve done a lot of thinking and talking about the project — describing the fundamentals of the project to a wide range of stakeholders, and in doing so I started to get a glimpse of what the bigger picture might be.

What does it mean when a Royal College has started to create ‘Best Practice As Code’? What does the future of this look like? How can we spread this idea more widely?

This led me into thinking about what Royal Colleges actually do, how they did it historically, and how they might do it in a future in which it’s almost impossible to know ‘all the medicine, all the time’ — simply because of the volume of new knowledge and the speed with which it changes. #[knowledgehalflife](https://en.wikipedia.org/wiki/Half-life_of_knowledge)

### Royal Colleges 1.0

(I think they also used to call them just, er, ‘Royal Colleges’)

Royal Colleges are basically a professional club. An *exclusive* club for clinical practitioners with a specific clinical interest or role. Royal Colleges define what is best practice in the speciality of interest, and disseminate that best practice. It’s an important part of how we ensure that the people practising medical specialities are suitably qualified to do so. You can join the club if you pass their entry requirements. These vary widely, but they often include examinations and vocational (practical, on-the-job) training.

There are Royal Colleges for every kind of medical and surgical speciality — Physicians, Surgeons, Anaesthetists, Nurses, Emergency Medicine, Paediatrics, General Practitioners, Psychiatrists — and more. And each country tends to have its own suite of medical Colleges (not all Royal of course — in those cases where they have escaped the clutches of their monarchies….)

For a long time (in the case of some Colleges, hundreds of years) these roles were carried out in entirely analogue fashion. Paper documents. Journals posted to clinicians. Meetings and conferences and committees.

This worked pretty well, limited as it was by the speed of the postal service, the cost and size limitations of physical meetings, and the intensely hierarchical nature of committees, College Councils, Presidents and Chairs — which tends to prevent a diverse range of practitioners getting involved in standards and guideline development.

### Royal Colleges 2.0

In the late 1990s and especially in the 2000s–10s, Royal Colleges started, at varying speeds and with varying alacrity, to adopt the publishing models of the Internet age. We now, fairly reasonably, *expect* a Royal College’s latest guidance to be published in some digital format.

Generally it’s a downloadable PDF — OK, sure there are better ways to publish web content, but by and large that misses the point—which is that suddenly guidance could be developed and published more cheaply and rapidly.

Accessing guidance in a timely fashion also became orders of magnitude easier. **Royal Colleges 2.0** allowed clinicians to get **near real-time knowledge**. But this still requires the clinician to download a document and read it, transferring the knowledge into their brain either in advance, or maybe just ‘at the point of care’.

There’s still potentially a discoverability problem with web-published guidance, because it doesn’t necessarily present itself to the clinician when they need it — the clinician needs to know about the existence of the guidance, then go and find it, and absorb it. PDFs and websites don’t integrate with an electronic clinical record. So we need better ways to get the right knowledge in front of the right clinician and patient, at the right time, so that together they can make good plans.

But most of all, there’s now a problem of **information overload** — how can the clinician *possibly* learn and know **all** the knowledge that their areas of medicine have to offer, and how can they then keep it all up to date? How can they access this knowledge when it’s needed, and ensure they get it **right the first time**?

It’s increasingly apparent that while Royal Colleges 2.0 has brought great benefits, we’re now approaching the limits of those benefits purely due to the volume of knowledge that is now available and the ability of clinicians to keep up with it all, process it, and enact the guidance safely.

Enter **Royal Colleges 3.0 — Best Practice As Code!**

### Royal Colleges 3.0

Following on from the scene-setting above, what we need is a way to **bring best practice right into the electronic patient record, dynamically, and on-demand**. And there have already been attempts to do this, in the form of simple clinical calculators and decision support templates. For the purposes of this blog I’ll group all of them under the term *digital* *clinical tools.*

Craftspeople end up making their own tools — woodworkers design and make new woodworking tools, and surgeons design surgical instruments. The best of these eventually become ubiquitously used.

Counter-intuitively (for those with typical commercial views), successful adoption of a tool such that it becomes ubiquitous **relies on sharing the idea and design as widely as possible**. Excessively tight intellectual property restrictions around the innovation might allow for short-term profit, but in software this actually just prevents its natural spread and limits its long term impact.

A huge array of clinical digital tools already exists. Sites like [MDCalc](http://mdcalc.com) contain hundreds of such tools. But crucially there is very little integration of these tools into clinical records. Where it’s been done, it’s very sporadic and variable as to which tools are integrated into which EPRs. We certainly couldn’t train clinicians to *expect* such tools to be in their arsenal when they become qualified. **And that is the test.** **Is the tool ubiquitous enough that you can say it will be everywhere?** A trainee surgeon can be trained that there will be the full array of specialist surgical tools in the tray for the job they’re doing. We *can’t* say the same for a paediatric endocrinologist’s special tools, because these are software which is either *not yet written* or not yet widely enough implemented to be something we can expect to be present.

#### **Ubiquity**

Digital clinical helpers and tools have existed for many years, but these have been **very** sporadically deployed in specific patient records systems. Where one system implements a clinical tool, other systems may not do so. Without ubiquity they will not become established in clinical practice.

How do we achieve ubiquity? By separating these clinical tools from their end-user-facing applications. **They need to be designed and distributed as APIs.** Using an API (usually these days this would be a [REST API](https://restfulapi.net/), but other types are available and it *doesn’t really matter* as long as they exist) means a single trusted source can perform calculations, offer decision support, and other clinical tools. In my mind, for this article, that ‘trusted source’ is the Royal Colleges and other professional bodies — but it could be **any organisation** as long as it has the stature to be trusted by clinicians.

The user’s EPR sends the required information, the API performs the calculation, and the result is returned to the EPR. In terms of the EPR developer, this is much easier to implement and way faster. There is no risk of locally implementing the clinical tool wrongly. You’re always going to have the latest version of the clinical tool.

And there are clinical tools which *should* exist but are not implemented in code because they’re expensive and tricky to implement. This is the area where **only** respected and trusted organisations such as Royal Colleges could really excel — having the reputation and gravitas to be able to produce ‘Gold Standard’ tools, even where these are difficult to produce and clinically assure.

#### **Clinical accuracy and safety**

We need these digital clinical tools to be safe and accurate for clinical use. Which organisations have the capability, will, and trusted stature to build and distribute these tools? Who better than the Royal Colleges, who have *always* been in the business of providing clinical guidance and knowledge, to own these clinical artefacts? Sure they’ll need to upskill in order to do so — but 25 years ago *none* of the Royal Colleges had a website, they had to upskill to move to RC2.0 — they’ll do the same for RC3.0.

#### How to do this RIGHT

[**Do the hard work to make the API simple**](https://gds.blog.gov.uk/2014/07/28/doing-the-hard-work-to-make-things-simple/#:~:text=Our%20fourth%20design%20principle%20is,the%20wider%20Civil%20Claims%20system.): Publish robust REST APIs with a good developer experience, rich documentation, responsive support, user and developer forums, SLAs for uptime and build a community of those who use them, build them, and test them.

**Testing**: API code can be built and published with a bulletproof test battery at every level within the software, which can run every time the code is changed to assure that the clinical tool is correct and safe. Current MHRA regulation around software tools is far too lightweight and relies on suppliers ‘marking their own homework’ too much. We can do so much better — publishing test outputs showing how the tool has been verified as safe.

**Terminologies**: The APIs can recommend the correct clinical terminologies and reference sets of terminologies that must be used to ensure that the ‘input data’ is correct. It’s worth bearing in mind that most of the recent issues with mis-implemented clinical calculators in UK GP IT were [actually errors relating to the selection of SNOMED-CT terms or Read Codes](https://www.gov.uk/government/news/mhra-information-on-tpp-and-qrisk2). Proper terms for the recording of data can also be supplied.

**Open Source**: Publishing the code in its entirety in open source is I think also fundamental to achieving trust. These APIs are not a ‘black box’ which takes inputs and returns outputs, but a fully auditable, open, reviewable, clinico-technical artefact. I’ve written much more [here about why Open Source Is The Only Way For Medicine](https://medium.com/@marcus_baw/open-source-is-the-only-way-for-medicine-9e698de0447e). Open source is the key to achieving robust, widely reviewed code. Open source also guarantees equity of access for all.

**Clinician-led**: Not every clinician wants to code. *But all clinicians have the capacity to learn to code if they want to.* Python is taught in my kids’ high school. That’s actually a big part of why I chose Python for the RCPCH Digital Growth Charts project — it’s simple, well-tested, readable, and ubiquitous. I’m absolutely convinced that there are enough clinician coders out there to supply the world with safe, shareable, clinical tools. All they need is the framework within which to do it, and the support of the rest of the clinician community. They’ll need technical help too, I’m not here trying to freeze out non-clinician developers. But recalling the experience of [developing the RCPCH centile chart code](https://github.com/rcpch/digital-growth-charts-server), **there’s absolutely no way we could have done it** without having two clinician-coders in the team.

**The slow ramp to EPR integration**: We all know that the world of EPRs moves fairly slowly, but by doing some of this [**hard work to make it easy**](https://gds.blog.gov.uk/2014/07/28/doing-the-hard-work-to-make-things-simple/#:~:text=Our%20fourth%20design%20principle%20is,the%20wider%20Civil%20Claims%20system.), we can encourage EPR vendors to build in these clinical tools, because it will be easy to do and involve only the minimum of clinical risk for them.

**Expert guidance**: Royal Colleges should build APIs under the guidance of an expert panel, such as the one assembled for the RCPCH Digital Growth Charts. These panels should be inclusive, shouldn’t get involved in the implementation, but should make the decisions that guide the implementation. THey should always have a mind to best practice and ‘[the principle of least surprise](https://en.wikipedia.org/wiki/Principle_of_least_astonishment)’ for the average clinician.

In the short term, we might also have to provide simple web-based ‘[demo clients](https://github.com/rcpch/digital-growth-charts-react-client)’ that facilitate ‘cut-and-paste interop’ — certainly not the best way to provide the tool, but better than nothing. And it’s what clinicians are already having to do! But we can make it at least easy to cut and paste a clinically safe, well formatted, informative entry. We can suggest clinical codes to use. We’re here to make clinicians’ lives easier and in doing so drive up the quality of care.

### Get involved & spread the word

Clinical informaticians, clinicians and health techies like us can be part of the solution, recognising that the clinicians’ digital tool-set needs to be upgraded, encouraging respected organisations like Royal Colleges to consider this a legitimate part of their remit, building those tools, and helping the profession move forward into a world where these tools are widely available.

It’s worth mentioning also that these clinical tools are only one of a huge number of [**Missing Healthcare Technology Things**](https://github.com/pacharanero/awesome-missing-nhs-things) which are slowing down progress. The health IT world’s obsession with achieving Interoperability is not going to fix these missing things alone.

All of this is really just an idea at this stage, but we’re bringing the first stage of it to reality with the [RCPCH Digital Growth Charts project](https://growth-blog.rcpch.ac.uk/) and really only time will tell if Royal Colleges 3.0 will come to pass.

If this idea resonates with you and you want to talk about it more, either comment below or [contact me on Twitter](https://twitter.com/marcus_baw).
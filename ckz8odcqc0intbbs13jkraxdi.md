## No, you do not need a Domain Specific Language (DSL) for Clinical Decision Support or Clinical…

Image credit — unknown (image [link](https://www.bladeforums.com/threads/useless-knives.1615076/page-5)) — found through searching ‘useless tools’

Otherwise known as Computable Biomedical Knowledge artefacts, or perhaps less pompously as Digital Clinical Tools, clinical decision support and clinical calculators *could* be built quite simply using mainstream programming languages. This is what I would regard as positive effort towards solving a problem. Libraries of testable, open source, reusable code, each solving one problem in the huge problem space of medicine.

But most of the work that currently exists in this area is actually in developing abstract standards — spending time and effort to **not** solve the problem. Not solving the problem simply kicks the can down the road, expecting other future clinicians to take the time and learn your special bespoke DSL, and write the digital clinical tools.

Implementation also becomes a problem, because now ‘someone’ has to write and maintain a runtime which can interpret the DSL information, and execute it in an error-free way.

I thought I’d treat the world to a nice balanced ;-) appraisal of the pros and cons of DSLs for clinical uses like this.

### Reasons TO use a custom DSL

*For non-techs: ‘$LANGUAGE’ below is used in the way placeholder variables are used in code — you can replace it with the name of any language, eg ‘Java’, or ‘Python’*

*   If you choose *$LANGUAGE* you will never stop having to explain to irate people why you chose that ugly/slow/insert-insult-here language *$LANGUAGE*.
*   “Building a clinical decision support DSL avoids tying the entire project to a single mainstream language” — by simply creating a whole new problem of *tying the entire project to your bespoke language, which nobody else on the planet uses*. Neat. Well done you.
*   “It avoids having to teach clinicians to code”. Hello, it’s 2021 and children in primary school are being taught mainstream programming languages without any problems. And clinicians, who can read, understand, and actually make some useful clinical decisions on the basis of 35 pages of NICE guidance, are *probably* intelligent enough to learn some code.
*   Using a DSL for clinical decision support **prevents the mainstream language chosen being PHP**. (This is the *only* valid reason in this list)
*   (In the DSL sales brochure) “multiple implementations of *$SOME\_ACADEMIC\_DECISION\_SUPPORT\_DSL* runtime can exist, built in various languages, so users in all languages are equally well catered for”. (Reality) Welcome to your new multilingual maintenance and clinical safety nightmare, population: 1.
*   On the other hand, nobody ever got 17 academic papers, a decade of conference talks, and a professorship for writing some calculators in Python. And nobody got a nice sideline in their private consultancy from implementing clinical calculators in Python. For that you need a really arcane and difficult DSL — ideally one only *you* understand.

### Reasons TO just write it in a language

*   If you choose a DSL you will *never* stop having to explain to irate, professorial/academic types why you didn’t use *$SOME\_ACADEMIC\_DECISION\_SUPPORT\_DSL* :-)
*   A lot of what you’re having to do in the DSL *looks* like a programming language to me. Just get over yourself and use one that *already exists*. The job of writing clinical calculators and decision support is hard enough without making it significantly harder by inventing your own language.
*   When you use an existing language, you benefit from inbuilt language ecosystem and text editor features to solve problems like:

> modularisation of code, error handling, testing, hard things like crypto and statistical libraries, code linters, syntax highlighting in text editors, snippets, sensible diffs in Git, tools like Github, serverless runtimes…

*   Coding has been taught in schools for at least 5 years. Next-generation clinicians will have at least a basic understanding of coding, which those clinicians who want to develop digital clinical tools will extend.
*   Languages are **real** and executable and many of them have been around for decades already. The latest *$SOME\_ACADEMIC\_DECISION\_SUPPORT\_DSL* may not be around in 5 years time.
*   *Writing* a DSL is the easy bit. Maintenance of a runtime which interprets the DSL and turns it into something usable is the hard bit, and a problem not to be underestimated. If you just use a mainstream language, you don’t need to build and maintain this.
*   If there is even **one** critical error in the runtime of your DSL interpreter, you can harm thousands of patients. And with a DSL you are going to have to implement a lot of **basic** functionality. Simple conditionals, branching logic… all there for you to implement from scratch and ripe for you to make an error in doing so.
*   The kind of clinicians that would get involved in this type of slightly technical work would learn *whatever language is necessary*. If a clinician can learn to understand *$SOME\_ACADEMIC\_DECISION\_SUPPORT\_DSL* then why is it presumed that they cannot learn to understand *$LANGUAGE.*
*   You can leverage *existing* ‘make it easier’ frameworks around existing languages (eg [EduBlocks](https://edublocks.org/) for Python) — just in case your clinicians do end up needing that GUI or visual toolkit for designing digital clinical tools. Again no need to write the whole thing from scratch.
*   Existing languages may have useful medical tools already built for things like handling of clinical terminologies (libraries like PyMedTermino), and the shared language can form a nucleus around which a clinical coding community can form. This will never happen with a single-purpose DSL, simply because it is not comprehensive enough.
*   If you need the clinical calculator to be technology stack independent there are many strategies to achieve this while still allowing you to use a mainstream programming language. For example, you could use REST as the ‘agnostic’ layer, or transact JSON via stdin/stdout (both of which I’ve used myself)

I do understand the draw of wanting to make digital clinical tools which are agnostic to the stack being used by those who might want to implement them. But honestly, there are better ways to do it than using a DSL.

And there’s one final question I would ask, if I haven’t yet convinced you:

> If you wrote a book but wanted to ensure it had a *truly* international audience, would you write it in a brand new and bespoke language that was equally impenetrable to all language speakers?

I’d love to hear your comments below. I have a fairly thick skin, so go for your life. I am a freelance GP, software developer, and clinical informatician. I am always for hire. [I only do open source](https://medium.com/@marcus_baw/open-source-is-the-only-way-for-medicine-9e698de0447e). And sometimes I write deliberately inflammatory blog posts. :-)

### Declarations of Interest

*   I have written a lot of clinical calculators in Python. When you’ve done a few **real** calculators you realise all the things that would be really hard to implement in your own DSL interpreter. *(Unfortunately these particular calculators were not open sourced, I have since parted ways with the company for whom I wrote them, partly for this reason)*
*   Simon Chapman and I wrote the RCPCH Digital Growth Charts internal logic in Python. There is no way we could have built the complex statistical logic required in our own DSL.
*   I have never written a Clinical Decision Support or Clinical Calculators DSL. And I never will. Who’s got the time?

#### General tech articles which sort-of agree with me

*   [https://dev.to/arturmartsinkovskyi/dsls-for-non-programmers-are-a-hoax-3m47](https://dev.to/arturmartsinkovskyi/dsls-for-non-programmers-are-a-hoax-3m47)
*   [http://deliberate-software.com/poor-dsls/](http://deliberate-software.com/poor-dsls/)
*   [https://stackoverflow.com/questions/1003241/when-should-i-use-a-domain-specific-language](https://stackoverflow.com/questions/1003241/when-should-i-use-a-domain-specific-language)
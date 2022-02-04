## The Clinical Software Usability Scale

It’s been 5 years since the Clinical Software Usability Scale (cSUS) was created. Following a discussion with a friend and colleague Dr Dave Pao today, I realised there wasn’t really much out there describing cSUS.

### Methodology

Following the pattern established by the scoring of the [established, pan-industry, Systems Usability Scale (SUS) 8](http://www.usability.gov/how-to-and-tools/methods/system-usability-scale.html), the questions are scored against a 5-point scale **Agree Strongly — Agree — Don’t Know — Disagree — Disagree Strongly**

The ‘axis’ of the questions is alternated in order to try to vary the ‘positive’ or ‘negative’ attitude that the question could be seen to have.

The questions were created by the members of the CCIO and CIO Networks, during a plenary session at DHI CCIO Summer School 2015, and in ensuing discussions on [this thread](https://discourse.digitalhealth.net/t/clinical-software-system-usability-scale/1147).

### The Clinical Software Usability Survey questions are:

1.  In my opinion, the software reduces the risk of clinical error. *(positive)*
2.  Effective support for this software is hard to access in a clinically-appropriate timescale. *(negative)*
3.  In my opinion, the software improves the quality of clinical care I can provide. *(positive)*
4.  The quality of the interaction/consultation with the patient is adversely affected by the use of this software. *(negative)*
5.  Using the software gives me the key information I need on patient’s history, diagnosed conditions and current care and treatment plan. *(positive)*

### Notes

*   Each question scores from 0 to 4 points, where 0 signifies a trait of the least usable system and 4 signifies a trait of the most usable system. Clearly, because the ‘axis’ of the questions is alternated, the mathematics of the scoring must be alternated too. It makes the scoring a little bit complicated, again this is how it’s done is the SUS so we followed suit.
*   The points are summed to give a total for the cSUS score in which the minimum score is 0 and the maximum score is 20. They are then multiplied by a factor of 2.5 to give a score ranging from 0 to 50. The authors of SUS felt it necessary to include this multiplication step, which I believe is an unnecessary complication (and in fact, for those authors, resulted in [completely avoidable confusion as to whether the SUS is a percentage 8](http://www.usability.gov/how-to-and-tools/methods/system-usability-scale.html)), but we followed them in doing so in order to maintain compatibility/parity of weighting between SUS and cSUS.
*   In total therefore we end up with a SUS score out of 100 and a cSUS score out of 50. The total score for the combined survey is 150.

If you have any feedback or ways to improve the questions or methodology, then this would be a good place to discuss it. **If making a suggestion to improve on of the questions, please supply a suggested alternative form of words, rather than just making a comment about the existing form of words.**

I’ve also created a [repo on GitHub](https://github.com/pacharanero/csus) for the cSUS questions for ease of forkability, feedback, and pull requests.

Back in 2016, myself and Jon Hoeksma from Digital Health Intelligence presented a [webinar with the first cSUS survey results](https://vimeo.com/166190203%2018).

[cSUS is licensed CC-BY-SA 4.0 International](https://github.com/pacharanero/csus)
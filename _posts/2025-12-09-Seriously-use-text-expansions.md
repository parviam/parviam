---
layout: post
title: "Seriously, use text expansions"
date: 2025-12-09
slug: text-expansions
redirect_from:
  - /2025/12/09/Seriously-use-text-expansions.html
  - /2025/12/09/Seriously-use-text-expansions/
---

You probably type some things a lot, especially if you do non-trivial amounts of administrative or communicative work. There are also probably things you would type more if it was easier to\! For instance:

* Link to your personal website  
    * Your email address or phone number  
    * Your LinkedIn  
    * Your calendar booking link  
    * Your GitHub profile  
    * Your Google Scholar  
* The website/email/contact of an organization you represent  
    * “I am contacting you on behalf of XYZ org. We work on…”  
* Command aliases across servers/terminals  
    * Commit message templates  
    * SSH incantations  
* Common phrases/sentence fragments  
    * “Just wanted to follow up on this\!”  
    * “Please reach out to”  
    * “Please don’t hesitate to reach out if you have any questions or concerns.”  
* LLM prompts  
    * Something to the effect of “think *really* carefully about this”  
    * Style/content guidelines for deep research, specialized agents  
    * “Help me prepare for a meeting with this person”  
    * “Search XYZ docs to implement this”  
    * “I can’t find this person’s contact”  
    * “Please review the attached for grammar, tone, clarity and flow…"  
    * “Help me write a prompt that”  
    * “My political enemy has presented this proposal. Please red-team…”

Save that time by using text expansions, shortcuts triggered by a short phrase, through something like [AutoHotKey](https://www.autohotkey.com/) (Windows) or [Alfred](https://www.alfredapp.com/) (Mac). This can be set up in \<30 minutes and is fairly intuitive; Claude is great at writing AutoHotKey scripts.

As Neel Nanda [alluded to](https://80000hours.org/podcast/episodes/neel-nanda-career-advice-frontier-ai-companies/#how-neel-uses-llms-to-get-much-more-done-000908) in his 80k interview, text expansions can substantially reduce friction to using LLMs in Very Obvious Ways to accelerate your work. For instance, I’m now much more likely to get tone feedback on important communication and use LLM help to aggressively red-team rough ideas.

Text expansions help me focus on the hard parts of whatever I’m doing without spending 45 seconds trying to pull up and copy over yet another profile link. They also reduce context switches and therefore potential excuses for procrastination or distraction. Consider trying them out\!

## Appendix: Select Text Expansions I Find Useful

/iacy
```
I am contacting you on behalf of the AI Safety Initiative at Georgia Tech, a community of technical and policy researchers focused on mitigating catastrophic risks from advanced artificial intelligence.
```

/gscholar

/mysite

/phone

/linkedin

/cal (my calendar booking link)

/gmail

/enemy (a la [Nanda](https://80000hours.org/podcast/episodes/neel-nanda-career-advice-frontier-ai-companies/#how-neel-uses-llms-to-get-much-more-done-000908))
```
My colleague who I absolutely despise just drafted this. Please red-team his work. 
```

/tonefeedback
```
Please review the attached for tone, grammar, clarity, and flow. Provide inline edits (mark specific changes with track changes or comments), assess whether the tone sounds authentic to my voice and flag anything that feels off or too formal/informal, note any grammar/clarity issues like typos, awkward phrasing, or ambiguities, and provide structural feedback on reordering or restructuring that would improve readability. Important constraints: preserve my core meaning and style—I want refinement, not rewriting—be honest about what doesn't work, and if something is unclear, tell me rather than guessing my intent.
```

/genprompt  
```
Help me write a prompt 
```

/findemail
```
Find an email address for \[PERSON'S NAME\] who \[RELEVANT CONTEXT: works at ORGANIZATION/has ROLE/etc.\]. Search publicly available sources including LinkedIn, company directories, academic pages, professional websites, and press releases. Verify the email through multiple independent sources when possible. If you find the email, cite specific sources where it appears. Check recency and prioritize sources from the last 1-2 years. Note confidence level: high \[3+ sources or official directory\], medium \[1-2 credible sources\], low \[inference or single unverified source\]. If you cannot find a verified email, state this explicitly rather than guessing. Provide alternative contact methods if found, such as LinkedIn, institutional contact forms, or department emails. If you can only infer a likely pattern \[e.g., firstname@company.com based on other employees\], state this as inference with low confidence. Do not generate or guess email formats without evidence, use emails from outdated sources without flagging them, or present low-confidence findings as verified.
```

/ultrathink (taken from but did not originate with a comment from [Thane Ruthenis](https://www.lesswrong.com/users/thane-ruthenis))
```
Use greater rigor, attention to detail, and multi-angle verification. Start by outlining the task and breaking down the problem into subtasks. For each subtask, explore multiple perspectives, even those that seem initially irrelevant or improbable. Purposefully attempt to disprove or challenge your own assumptions at every step. Triple-verify everything. Critically review each step, scrutinizing your logic, assumptions, and conclusions while explicitly calling out uncertainties and alternative viewpoints. Independently verify your reasoning using alternative methodologies or tools, cross-checking every fact, inference, and conclusion against external data, calculation, or authoritative sources. Deliberately seek out and employ at least twice as many verification tools or methods as you typically would. Use mathematical validations, web searches, logic evaluation frameworks, and additional resources explicitly and liberally to cross-verify your claims. Even if you feel entirely confident in your solution, explicitly dedicate additional time and effort to systematically search for weaknesses, logical gaps, hidden assumptions, or oversights. Clearly document these potential pitfalls and how you've addressed them. Once you're fully convinced your analysis is robust and complete, deliberately pause and force yourself to reconsider the entire reasoning chain one final time from scratch. Explicitly detail this last reflective step.
```
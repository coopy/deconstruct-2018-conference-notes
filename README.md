# deconstruct-2018-conference-notes
Notes from the Deconstruct 2018 conference in Seattle

## Julia Evans | @bork | Stripe | "Impossible Program"

### Busting some myths
1. ~You have to be an expert~
  - Find a starting point to learn from
  - Prototype something
2. ~If it were possible, someone would have built it already~
  - It may just not have occurred to anyone yet
  - The idea may have occurred, but nobody's put it in practice yet
  - There may not be that many people operating in the space
3. ~You have to work on weekends~
  - Julia doesn't program on weekends (she draws comics and writes blog posts)
  - She took one week of vacation to build the prototype
  - She applied for a 3 month paid Segment fellowship and got it (see negotiate leave with boss)

How to do something ambitious: Give your future self the time - put it on your calendar. Negotiate a sabbatical with your employer.

### Making it actually good:
1. Review prior art
2. Invest in testing
3. Invest in usability
4. Write documentation

### Takeaways
- Employers should provide easy sabbaticals with continued benefits.

## Sandy Metz | "Polly wants a message"

Teaches OO classes. Started seeing a pattern of where things go wrong.

Churn and Complexity are usually inversely related: A file changed often gets simpler. The code smell is when a file with high churn has high complexity. The symptom is a large, complex file, with many conditionals, and it happens in files that are **important to the business domain**. 

> "The stuff you care about most gets worse, faster".

> "What brought you success will doom you to failure".

### The path to pain
Fowler's design stamina hypothesis results in this recommendation: Don't spend too much time on design up front, just throw code at the wall and see what sticks. But at some point (hard to recognize when), you have to take a step back, think about design, and refactor.

### Takeaways
- Procedural doesn't scale; depends on complex conditionals.
- Dependency injection is great, but _inject something smart,_ not just a flag!
- OO is mainly polymorophism; don't create complex class hierarchies.
- Factories are where the conditional goes in OO. Set it and forget it.

## Tea Ho | @teabait | donorschoose.org | Accessibility

### Takeaways
- Alt text can convey the "feel" of the images - don't be limited to a dry description!
- Look out for `:focus {outline:none}` in CSS reset libraries. BAD.
- Use `aria-live` to denote an updating section, along with `aria-busy`, `aria-atomic`.
- Use plain language (especially in stressful situations like errors). Helps neuroatypical folks who may take things more literally.
- Use radio buttons for mutex choices. `role=radio` is a pain to implement correctly.
- Get started easily!
  1. Do a tab-key test of your website.
  2. Use a contrast checker (google it).
  3. Get a screen reader (like Chrome Vox, or use your operating system's).

## Ryan Herr | @rrherr | "Banjo Grammar"

### Takeaways
- CFG = context free grammar is a set of simple rules!

## Vicky Nguyen | wickyvinn | Fastly | "Show me your echolocation"

Hard-code routing tables and do branched pings to probe network speed

### Questions
- How do you load balance the optimal routes so you don't DDOS them
- How are routing tables updated when "hops" are added and removed?

## Nabil Hassein | Formerly Khan Academy | "How are all of your relationships?"

### Look into
- Bret Victor: "What can a technologist do about climate change?"
  - Critique: We must create options for **people**; policy makes got us into this mess and won't help us.
- Grist Magazine: "Ice Apocalypse"
- Assata Shakur: "Assata" autobiography
- Nabil Hassein: "Against black inclusion in facial recognition"

## Jumana Bahrainwala | @jumzb | "Scaling relational db migrations"

### Questions
- When you split your transactions up, how to you ensure a failed colunm add doesn't crash a later column write?
- How do you load test your migrations?

## Katrina Owen | @kytrinyx | Github | exercism.io | "Making Decisions"

- Dr. Stephen Wiseman: Lucky people are more preceptive.
- Dr. Share Frederick: Make opportunity costs explicit. Instead of "Don't buy"; "Spend $100 on something else".

### Takeaways
- Tactics for opening up from a narrow perspective
  - Image that an option _isn't available_ to you
  - Instead of brainstorming the solution, _Questionstorm_ the problem space
  - Disagreements uncover information you didn't have. Assume rationality and as Questions until you understand their perspective.
- Strategy is a plan for overcoming obstacles (You must identify what the obstacles are)
  1. Identify Challenge and Opportunity
  2. Come up with guiding policy - how to deal with challenges
  3. Coherent action - define aligned steps
- "Good strategy can be defined on the back of a napkin"

### Questions
- What are some questionstorming techniques?


  

---
layout: blog
title: Observations from the Jagged Frontier paper
date: 19 September, 2023
---

If you know me, you know that the last two years of my life have been all about consulting and technology. So, when the “Navigating the Jagged Technological Frontier” paper came out yesterday, I was really excited! 
Some of the findings like enhanced productivity and confabulations feel obvious. Especially for an MBA student that turns in strategic recommendations for class projects every other week. But of course, a study co-branded by professional organizations like BCG, HBS, and MIT helps validate those (yet to be peer-reviewed), and more importantly quantify them.

However, there were many insights that were interesting to me, and hopefully you. Before I share those, here’s a recap of the study:

> We examine the performance implications of AI on realistic, complex, and knowledge-intensive tasks. The pre-registered experiment involved 758 consultants comprising about 7% of the individual contributor-level consultants at the company. After establishing a performance baseline on a similar task, subjects were randomly assigned to one of three conditions: no AI access, GPT-4 AI access, or GPT-4 AI access with a prompt engineering overview. We suggest that the capabilities of AI create a “jagged technological frontier” where some tasks are easily done by AI, while others, though seemingly similar in difficulty level, are outside the current capability of AI. For each one of a set of 18 realistic consulting tasks within the frontier of AI capabilities, consultants using AI were significantly more productive (they completed 12.2% more tasks on average, and completed tasks 25.1% more quickly), and produced significantly higher quality results (more than 40% higher quality compared to a control group). Consultants across the skills distribution benefited significantly from having AI augmentation, with those below the average performance threshold increasing by 43% and those above increasing by 17% compared to their own scores. For a task selected to be outside the frontier, however, consultants using AI were 19 percentage points less likely to produce correct solutions compared to those without AI. Further, our analysis shows the emergence of two distinctive patterns of successful AI use by humans along a spectrum of human AI integration. One set of consultants acted as “Centaurs,” like the mythical half horse/half-human creature, dividing and delegating their solution-creation activities to the AI or to themselves. Another set of consultants acted more like “Cyborgs,” completely integrating their task flow with the AI and continually interacting with the technology.

# Identifying the frontier
While these categories are not exhaustive, I found it worth noting:
Frontier
Inside	Outside
o	Creativity
o	Analytical Thinking
o	Writing Proficiency
o	Persuasiveness	o	Working with cross-modal inputs (such as structured data and qualitative inputs)
o	Comparing contrasting pieces of information against each other

# Retainment
I’m glad that the study examined retainment. Simply put, it reflects how much consultants blindly trust the AI’s output. 
<IMAGE>

You might have thought that those who duplicated AI’s responses to a larger extent might get trapped with incorrect answers, but interestingly those who choose to retain AI outputs to a relatively high degree produced significantly better answers on average.

# Skill levelling

The biggest shocker. 
Not so humble brag – I’ve performed well at most places. Top 0.5-3 percentile in all education endeavors, good schools, top 5% at work that has had significant impact. Thus, while there is always competition, I used to feel secure that my intellectual capacity will let me positively differentiate myself. But that might not be as true now.

The study demonstrates how LLMs act as a leveler of skills. Apart with the infographic below from the paper, these were two insights that I took away from the numbers:
1.	The bottom-half consultants saw twice as much absolute improvement as compared to their peers in the top-half.
2.	The top-half consultants went from being 28% better than the bottom-half to being just 5% better than the bottom-half.

<IMAGE>
<TABLE?>
 
# AIs impact on talent development
People will stop delegating work inside the frontier to junior workers, creating long-term training deficits. Navigating the frontier requires expertise, which will need to be built through formal education, on-the-job training, and employee-driven upskilling.

I’m curious to see how employers balance using AI for short-term competitive advantage that eats into long-term sustainability of a talent pipeline.

# Convergence of thought
What LLMs solve for that’s distinct from AI so far is creativity. To me creativity meant a variety of thought. But the study demonstrates that AI’s ‘creativity’ does not fit that definition.

While subjects using AI produce ideas of higher quality, as discussed in the previous sections, there is a marked reduction in the variability of these ideas compared to those not using AI. This suggests that while GPT-4 aids in generating superior content, it might lead to more homogenized outputs. There is a whole appendix section dedicated to this topic of ‘Collective Variation’.

The quality distributions are the most popular, but I the similarity distributions were what surprised me. And something that I’ll keep in mind now when thinking about when/how much to use generative AI.
<IMAGE>
<IMAGE>
  
The paper suggests that companies that want to maximize exploration and innovation as opposed ot consistently high average outputs should maintain a diverse AI ecosystem, possibly multiple LLMs, or increased human-only involvement to counteract homogenization.

In a competitive landscape where many are leveraging AI, outputs generated without AI assistance might stand out and achieve notable success due to their distinctiveness.

# GenAI Literacy
“GPT +Overview” is a recurring term in the paper. You even see it in the above graphs. The ‘overview’ here refers to supplementary prompt engineering training that the group of consultants received. For every test where the humans-with-GPT outperformed the control group, the AI-trained humans-with-GPT outperformed both the groups.
Nothing too surprising here, but a reminder for me to continue incorporating prompt engineering in my own use too. Since last week, I began using custom instruction I’ll report back on my experience once I have spent more time with it. I am curious to know what training was given to the BCG consultants for this study. 

## Note
The paper refers to some natural language processing techniques like Google’s Universal Sentence Encoder (USE) and Restricted Damerau-Levenshtein distance (RDL). If you’d like to understand what those terms mean, I’d be happy to explain them in simple terms since I used to use them in the products we built at Credit Suisse. 
If you really grasp the tables that list the results of the regression models, let me know. I’d like some clarity on interpreting those :)
---
layout: blog
date: 22 May 2024
title: AWS Summit - LA 2024
---
![](/blogs/aws_summit_la24_images/keynote.jpg){: width="65%"}
![](/blogs/aws_summit_la24_images/lobby.jpg){: width="25%"}

AWS Summit is a series of events around the world for engineering organizations to learn the capabilities of AWS and engege with leaders within it. This blog is about the events I attended during the Los Angeles summit in 2024. I believe some event highlights should appear on [their website](https://aws.amazon.com/events/summits/los-angeles/) later too.

# 1. Keynote - AI at AWS
_Dr. Matt Wood, VP of AI at AWS_

This was supposed to be the "keynote" of the day with the VP of AI, but on the whole I found this session uninspiring in content. We spent 60min+ on 5 generic 'laws' of value creation with GenAI that can be summarized by saying - _You need AWS_. For what its worth, I've added my notes below.
![](/blogs/aws_summit_la24_images/meme1.jpg)

What I did enjoy was experiencing a keynote. The quality of the stage and slides was amazing and I appreciate the production effort that went into it. Also, if the recording is made available, please watch Ken Lovell's 10min part about golf in this. That was a masterclass in presenting on stage.

In the course of getting to our GenAI-in-everything future, here are 5 things that we can be assured of:
1. AI Foundations are in the cloud
- GPUs, cluster scaleout, Tranium, Inferentia
2. Start with pervasive and efficient experimentation
- [AWS Bedrock](https://aws.amazon.com/bedrock/)
- Use cases
    - Summarization
    - Analysis
    - Reasoning
    - Code interpretation
- Factors
    - Speed
    - Cost
    - Quality / intelligence
- It measures metrics such as Accuracy, Robustness, and Toxicity. Add also has the features to get the same feedback from relevant experts in the organization.
3. Mix and match models to your use case
4. Consistency, Coherency and Control are delivered through data
- Keep models focused, set constraints, and fine-tune your model.
5. GenAI can turbocharge your organization
- Amazon Q
- Hypothesis: 30% of work done is differentiated and 70% is not, just a necessity
- Apart from suggesting code snippets, the code editor also tells you where to palce the snippet. Customer quotes claim that >50% of code suggestions are accepted.
- Integrates with document solutions like Confluence. Create custom Q-apps like sumamrizing meeting notes when you get back from vacation.

![](/blogs/aws_summit_la24_images/shade_on_competitors.jpg){: width="45%"}

# 2. GenAI in Retail & CPG
[Michael Conor](https://www.linkedin.com/in/michael-connor-605256/) has a job that I aspire too. He is the "Global Generative AI Product Lead for WWSO" which seems to mean that he talks to the biggest brands from all industries and builds GenAI PoCs with them.    

![](/blogs/aws_summit_la24_images/industry_applications.png){: width="100%"}
![](/blogs/aws_summit_la24_images/retail_cpg_apps.jpg){: width="100%"}

- Organizations can (1) take an approach to embed GenAI expertise in groups or (2) create GenAI centers of excellence. Speaker recommends the former and thats how Amazon does it too.
- [Amazon Rufus](https://www.aboutamazon.com/news/retail/amazon-rufus) - Amazon.com's shopping assistant that provides chat-based shopping suggestions by considering (1) Product descriptions, (2) Reviews, and (3) Customer preferences (for instance brand preference, willingness to pay)
- We did a demo of a simple content marketing tool that was built using Bedrock Studio. It asked for product facets, response size, tone, and compliance concerns to create marketing content.
- Demo of how CPG's (Coke) could provide self-help solutions (soda dispensers) to customers (Burger King) that infer chat questions and suggest solutions from the manual. It can also infer images of dashboards and internal configurations to come up with an answer. It will save $250 which is the minimum per technician visit.

### Retail layouts
- Demo of AI's store layout suggestions based on a foot traffic heatmap (generated with AI and CCTV footage).
![](/blogs/aws_summit_la24_images/heatmap.jpg){: width="100%"}
- Each retailer has a 10+ page guidebook of the rules of visual representations of a store's products or services on display (called planogram). These go on to specify color combinations, product placement by height, safety constraints.
- Each CPG has a 'category leader' who owns relationships with distribution channels (like Target, Walmart). This leader needs to know the planogram preferences of the retailers.
- We did a demo of AI inferring proposed planograms against these rules (unstructured data such as PPTs) and suggesting changes required.
- Showed a concept of how an AI workflow could use a picture of an aisle to identify missing SKUs and list them for restocking.

_Source: [McKinsey report](https://www.mckinsey.com/~/media/mckinsey/business%20functions/mckinsey%20digital/our%20insights/the%20economic%20potential%20of%20generative%20ai%20the%20next%20productivity%20frontier/the-economic-potential-of-generative-ai-the-next-productivity-frontier.pdf)_

### Contact Centers
- Interesting fact: Order status check calls to contact centers can cost $14/call for quality brands.\
- Typically < 10% of calls get reviewed for quality purposes. AI can summarize (saving 5min/representative) and provide feedback about the call immediately and as trends.

### Generative Imagery
- Experimental demo of Amazon [Diffuse to Choose](https://www.maginative.com/article/virtually-trying-products-in-any-setting-with-amazons-new-ai-tool/) that allows shoppers to blend their likeliness and product photos. This allows for visualization on different body types and skin tones. It is done using a diffusion mode though, so it can have differences in details like prints and patterns on outfits.
- The most bullish use case is for keeping the same product in different contexts. This saves the time and cost of a studio. An extreme example of this is a beer brand that used customer's travel interests to present them ads of the brand's beer on those beaches. 
- Used [ComfyUI](https://github.com/comfyanonymous/ComfyUI/tree/master) to create high quality mockups.

# 3. Personal Agents - Ninjatech Demo
[Babak Pahlavan, CEO NinjaTech AI](https://www.linkedin.com/in/babakp/)<br>
[_Try it out_](https://myninja.ai/), use code AWSLAsummit20 and AWSLAsummit10 for a trials of the paid tiers.

- Ninjatech was a big favorite of Amazon at this event. They want to put an executive assistant in everyone's hands.
- Ninja does everything in parallel. You do not have to wait for one query to finish to start a second one.
- They trained their model in $30K and it has outperformed all but GPT-4 turbo on NQ and HotPotQA benchmarks.
- It also has a very sophisticated avatar that talks to you.
- Ninja has 5 modules:
1. Intent Analyzer - First recepient of the user's query. Decides which of the other modules this needs to be assigned to. Might rewrite the query when passing to the other model.
2. Researcher - The demo seemed very similar to [Perplexity](perplexity.ai) that I use when I need referenced answers. It does start with structuring the research and then goes onto fill the structure with multiple individual queries. So I wonder if it is simply prompt engineering under the hood.
3. Scheduler - Links with Google calendar. It can also engage in multi-turn conversations with guests to schedule an event.
4. Coder - Think of any LLM you are familiar with today.
5. Advisor - Think of any LLM you are familiar with today.

### My opinion
- It's ChatGPT + Perplexity + Calendar Plugin under one ChatUI. There is some value in unfying these, but I'm skeptical. Pricing will definitely matter.
- Speaking of pricing, this seems like a low margin product. One of its differentiators in the research module is the volume of content it reads. How can it use 3+ GenAI APIs (that each go for $20 per month) and sell that at $10-30 per month as NinjaAI.
- There are limits on the number of queries per module on the paid plan. These are probably sufficient ($20 plan buys 1,320 research tasks).
- They claim that AI is very bad with recognizing details relevant to scheduling, but my experience with NLP makes me think that's not really true.
- Loose the avatars. Nobody wants to see their assistant, especially one that's an API. Hearing is sufficient.
- They will later expose this agent though Slack, email, text and call. That should be very helpful.


![](/blogs/aws_summit_la24_images/arcade1.jpg){: width="45%"}
![](/blogs/aws_summit_la24_images/arcade2.jpg){: width="45%"}

In the arcade game on the left, every few alien corresponds to a kubernetes cluster that supports the game (telemtry visible in the bottom half of the screen). Kill them and they respawn, much like AWS's fault tolerance capabilities. Very creative demo, don't you think?
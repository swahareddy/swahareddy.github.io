---
layout: blog
title: South by Southwest 2024
date: 15 March, 2024
---
Last week I was at South by Southwest, a festival that I've been wanting to attend since forever. A 10-day carnival of 1000+  conference style events on tracks such as AI, mixed reality, culture, design etc along with another 1000+ music, film, and comedy events. My days looked like 10am-5pm of conference events and then 6pm-1am of socializing and attending music showcases! Sometimes a breakfast event at 8am too!

I've added some of my notes from the technology panels and keynotes here. **Click into the Mixed Reality and Generative AI titles below** to see notes of sessions from these tracks. You can find more audio and video recordings on the SXSW schedule website and YouTube channels respectively. I also want give a shoutout to the [South Asian House](https://www.instagram.com/southasianhouse/) for a great desi music lineup. 

![](images/neelyfellows.jpeg){: width="39%" }
![](images/banner3.jpg){: width="60%" }

# [Mixed Reality 🔗](/blogs/sxsw2024/sxsw2024_xr)
# [Generative AI 🔗](/blogs/sxsw2024/sxsw2024_genai)
# Miscellanous
1. [Link to Scaling Safely: Waymo's Roadmap for a Multi-City AV Service](#scaling-safely-waymos-roadmap-for-a-multi-city-av-service)
2. [Content Moderation](#content-moderation)

## Scaling Safely: Waymo's Roadmap for a Multi-City AV Service

> Fully autonomous ride-hailing is here. In San Francisco, Metro Phoenix, and increasingly Los Angeles, it’s totally normal to hail a Waymo ride with no human driver. Waymo has already provided more than 700,000 rides to members of the public, without humans behind the wheel. This is a fireside conversation with about how Waymo has successfully built a multi-city service, how it navigated a breakout year for autonomous vehicles in 2023, and why the autonomous future of transportation is closer than ever before.
> 
> Tekedra Mawakana, Waymo co-CEO<br>
> Laurie Segall, Mostly Human

- I recently read the book on 80:20. It was far too repetitive, so I would not recommend it, but it did drill the concept into me. And describes to me, the essence of Waymo’s journey
    - It is not possible to pre-preprogram and even train for every situation.
    - Examples of edge cases that need to be accommodated:
        - Fog in San Francisco
        - Heat in Death Valley
        - Thunderstorms in Miami
        - Sandstorms in Pheonix
        - Wipers for bird poop on sensors
        - Older people that are walking in the opposite direction on the road
        - Black ice
- On safety:
    - We had L3 in 2013 (what Tesla has now) but decided not to offer that to the public since it would not have been safe
    - Did a pilot with Waymo employees (waymonauts :P). And despite knowing the product and receiveing instructions, they would take their attention of the road often
    - People trust the technology more than they should.
- Community engagement:
    - It also influences indirectly influences politics and thus regulation. In SF, the residents advocated for us
    - Autonomous vehicles are an opportunity to expand access to mobility. Eg - We work with blind schools. Through them we learnt to add a ‘honk’ feature so they can find their Waymo in a crowd of cars.
- From a UX PoV, riding in a Waymo is better than an Uber/Lyft since the experience is consistent (same cars, all cleaned on schedule), comfortable (Jaguar), and can be personalized (music).
- In-vehicle driving animations
    - The Waymo identifies objects at every instant and predicts their individual movements. We used to show this on the in-car screen, but it was more discomforting than comforting.
    - What we show now has been reduced to be just what (simply) reassures riders - other cars, people, infrastructure, traffic cones
- On job transformation - For car mechanics, Waymo certification is the highest kind because they are trained to inspect and repair HiTech safety-critical sensors.
- Do people expect to pay more or less than current rideshares? Did not have a clear answer.
- On whether (auto) insurance companies are a major driver for AVs - No clear answer. But seemed to indicate that it is not a big deal currently.
- Future of Waymo is multiple business lines:
    - Ride sharing
    - Delivery services
    - Classic trucking
    - Licensing technology to automobile manufacturers
- When is the car’s design going to change
    - i.e. take out the steering wheel etc
    - Cannot currently change it since it is mandated by regulation. So its not a current consideration
    - It could look like a dining table layout where you can spend time with your family/team. There is no need to orient one way of there is no driver.
    - Reminded me of the Zoox vehicle:
        ![Untitled](images/zoox.png){: width="65%" }      

## Content Moderation

> There is a problematic gap between the pace of technological change and regulatory development. Once policies are agreed and implemented – technology has moved on. That’s why it’s important to design measures that are both robust and flexible. But as online interactions move from bulletin boards to multiverses, how can users stay protected?
> 
> Brittan Heller, Stanford University<br>
> Ronaldo Lemos, Meta Oversight Board<br>
> Maxime Prades, Meta<br>
> Charlotte Willner, Trust & Safety Professional Association
> 
> [Event Link](https://schedule.sxsw.com/2024/events/PP135408)

To check whether an institution is independent, look at:

1. Governance structure
2. Funding
    - Who is paying for it? What is the duration of the funding, and which year of it are we in?
3. Transparency
4. Insulation
    - Internal policies that protect content and people in the body such as (fixed) ‘tenure’ terms

Sam Altman has been calling for an international oversight body for AI like UN’s nuclear watchdog (IAEA) ([link](https://www.euronews.com/next/2023/06/07/openais-sam-altman-calls-for-an-international-agency-like-the-uns-nuclear-watchdog-to-over)). Brittan suggested that we can look to these aspects of International Court of Justice as inspiration:

1. Consensual Jurisdiction - States (countries) volunteer to be a part of this body and abide by its decisions
2. Advisory Opinions - The ICJ issues advice to states that seek it out when they need fair external input.
3. Triage - In urgent cases, the ICJ can issue provisional measures

Brazil’s internet laws are a model for the world - [An Online Bill of Rights in Brazil - Open Society Foundations](https://www.opensocietyfoundations.org/voices/online-bill-rights-brazil)

Meta has been using AI in content moderation for:

1. Classifiers for problematic and safe content
2. Prioritization of content that needs review

Meta has found GenAI valuable for training. For instance there is not much content on first person shooting data. Our attempts to filter this often catches innocent content like gaming live streams. GenAI lets us generate realistic content that we use to train our models.

OpenAI technical whitepaper on how GenAI can be an effective tool for moderation - [Using GPT-4 for content moderation (openai.com)](https://openai.com/blog/using-gpt-4-for-content-moderation)

Recent (Meta) Oversight Board made these recommendations to Meta:

1. Label AI generated content
2. Cheapfakes can be as harmful as Deepfakes and should be treated as such ([link](https://www.wired.com/story/meta-youtube-ai-political-ads/))

Detecting AI generated content:

- Is too expensive - Most AI-generated content is not harmful, so finding the few bad ones is cost-prohibitive
- Watermarks - Industry-level conversations going on for visible and invisible watermarks

2024 - 4-5% of social media feed is AI-generated. In 2030 that will be 90%+ ~ Ronaldo Lemos

Future of regulations:

- [AI Act](https://artificialintelligenceact.eu/the-act/) (EU) is likely to come out in 2 years
- Also look at existing learnings like the Hollywood screenwriter’s strike

![](images/taiwanbeats.jpg){: width="60%" }
![](images/dinosaurband.jpg){: width="60%" }

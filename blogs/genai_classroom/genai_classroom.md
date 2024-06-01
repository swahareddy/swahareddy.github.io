---
layout: blog
date: 12 April 2024
title: GenAI in my Classrooms
---

Since ChatGPT came out, I have been a student in 20 courses and a teaching assistant for 7. This post is about my observations of GenAI (henceforth referred to as AI) in the classroom based on these experiences.

# 1. Innovative Use Cases

There is no course where I have seen AI be more ingrained than the mandatory marketing course for the MBA.PM program. This section is about mostly my contributions to this course. Prof Dutta reached out five months in advance to talk about his goals for the course, a key point was the forward thinking use of AI in the classroom. To that end, these are the changes we made:
1. Created exercises that give students exposure to new tools and means of learning.
2. Added course content that introduces opportunities and risks of AI.
3. Channel back peer feedback by having teams present their learnings from using GenAI in their final assignment.

## 1.1 AI Exercises
### Generative Imagery: Positioning

A common marketing framework is STP = Segmentation --> Targeting --> Positioning.
Positioning is about communicating about your product to the cusomer segments you've prioritized. The case for the day was on Clorox (classic hardcore cleaning brand) launching Green Works (plant-based). Students were tasked with creating an Instagram launch post for two segments - environmentally conscious customers and mothers.

I wanted them to use generative imagery for the graphics in the instagram post. They could also use LLMs for the caption. For many in the class this was the first time witnessing text-to-image models do their magic and the exercise was met with _wows_ across the room. To run this, I created a [Canva template](https://www.canva.com/design/DAGAS94nsb0/zB0N6Gc-ebe9oFOMIvrIvA/view?utm_content=DAGAS94nsb0&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink&mode=preview) and demonstrated its Magic Media functionality. 

![](canva_magicmedia.jpg){: width="100%"}
![](greenworks_positioning.png){: width="100%"}

### AI Bots: User Interview Simulation

A great marketer is able to ask customers good questions and derive non obvious insights about their behavior that be used to further the use of the brand. The case for this class was the Accor hotel chain and its concerns with how customers were booking rooms. 

Thus I designed an assignment for students to identify the customer buying journey and be able to creatively probe the customer. I created three customer bots on [character.ai](character.ai) and gave them personalities and context from common user personas. The students then worked in small groups to spend some time texting witht their 'customer', learn who they are and their buying journey.

![](3bots.png){: width="90%" }

*The class was split into 3 groups, each assigned a different customer*

![](bot_instructions.jpg){: width="100%"}
![](jenny1.png){: width="45%" }
![](jenny2.png){: width="45%" }

*Description provided to create Jenny's persona*

![](bots_room.png){: width="100%"}

*You can have customers discuss among themeselves in rooms like these*

### Github Copilot

Every MBA student takes a mandatory statistics course in their coursework. Mine was in September 2022, two months before ChatGPT was launched. So my class learnt t-stats, regression, and classification using Radiant, a interactive UI within R Studio, never touching the code. The next year's MBA class (September 2023) however learnt he same concepts using R code directly. In their first class, they were taught how to use an IDE and integrate Github Copilot. Note: 84% of this class is from a non-engineering background!

I TA'd the Quantitative finance class. The professor usually goes out of his way to warn students that python is a prerequisite, but this year he was able to relax the requirement since he felt comfortable teaching students the logic of the algortihms rather than the code itself, and trusting that they would be able to figure out the programming themeselves.

## 1.2 New Course Content

Top of a marketing funnel is discovery. Back in the good old days, discovery or intent would begin with a google search. Recently social media and feeds have begun to inspire purchases, and most recently questions are being most directly resolved though AI.

I wrote an article on how seach engine optimization and marketing would be affected by an AI-answer driven world and what could be done to still remain top of mind there. I've refined the piece by implementing feedback from career SEO veterans, SEM executives, and academia.

> See the article - [SEO/M and GenAI](/swahareddy.github.io/blogs/seo_genai.md)
>
> ![](/blogs/seo_genai_images/Picture9.png){: width="100%"}

GenAI's biggest impact within marketing is probably in customer service (chatbots) and advertising (creating assets). I introduced Google Product Studio to the class to demonstarte how agency access can be democratized in the future and micro targeting can be achieved. This product if taken further, could also use Gemini to uniquely customize messaging for the viewer and text-to-video for video ad generation given a product.

<iframe width="80%" height="100%" src="https://www.youtube.com/embed/kyTu3mgGfUA" title="Digital marketing, generated by AI | Google Ads" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## 1.3 Student Feedback

In the programming courses that used there were a fair share of students that found the AI-assisted programming challenging, and could have benefited from a Drivers Ed course in programming rather than being given the wheel of a Cybertruck i.e. Copilot. The availability of AI doesn't mean that there isn't a need for a foundational education. The 'time to market' however, has significantly improved.

In the marekting course, all teams had to present to their peers on how they have been using AI in their group projects. We heard some interesting observations comparing tools. For instance Claude was preferred for market sizing and other analytical tasks. Gemini was preferred for its ability to integrate with the Google suite that teams were using, and Bing Chat (in Edge) was preferred for its ability to limit context to specific web pages and the browser integration. One team never presented the whole class, but rather used digital characters (deepbrain.ai) to do so, including deepfakes. I was introduced to sider.ai that provides a lot of the same features as above, but uniquely, has a a YouTube summarizer. It uses the video's transcript/captions, somthing that you could paste into a chatbot yourself, but Sider makes it seamless.

AI has been able to provide equity to non-native English speakers in my class. They are now faster and more confident inn the owkr they put out, and AI has a made a meaningful reallocation of their learning : proofing time allocation. 

# 2. Academic Use Policy

On the whole I have been impressed by the encouraging attitude taken by my professors towards AI. If they haven't encouraged or expected them, they have been (rightfully) ignorant about its role in their course. I have not seen any professor take a stand against AI in the classroom. Of course, university level guidance and the lack of trustworthy auditing tools must have played a factor in their approach.

I was part of a panel on technology ethics for the business school's board where the ethics of AI plagiarism was discussed. From the discussion I gathered that USC Marshall's policies have been technolgoy forward compared to other academic institutions. In the appendix I have sumamrized the variety of points from syllabi of 15+ of my courses from multiple departments. Most professors have taken the approach of "If you can't beat em, join em", and ask for attribution. 

# 3. The Challenges

### Citations
Professors want students to cite the AI model they use. If that means, the APA style...
> OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. https://chat.openai.com/chat
... thenI don't think that adds any value as a reference. This kind of citation could refer to the use of AI for anything from grammatical corrections to hallucinating facts. Thus, some professors as for prompts. When they asked for prompts in the spring of 2023, I was genuinely confused about what they wanted, as if all conversations are not a series of prompts getting closer to the ideal answer. ChatGPT's 'Shared Links' feature came out in June'23 and helped solve this challenge, but this is not available in all major chatbots.

### Integrity
Turning a digital exam into a pen and paper one because students might use AI seems like progress in the opposite direction. When I heard of that in one of the courses, my inital reaction was one of frustration too. However, grading the finals of the marketing management course changed my mind. This final has a lot of fundamental marketing questions about a popular brand and a HBS case. The kind of questions that ChatGPT is good at. Reviewing the answers made me realize that I knew ChatGPT's writing style, and could identify it in every fourth submission. You know what I'm talking about - Unnecessary introductions and conclusions, an attempt to balance all sides even when there should be a clear preference, regurgitating standard points that miss the creative outliers that human would have had... Professors are hesitant to use browser lockdown tools (similar to ones used for at-home proctored tests that don't let you switch tabs/windows) since they hurt the tone of the class and the teacher's realtion to students. 

### Plagiarism Software
These are not reliable and have a 2-5% false positive rate. You cannot take disciplinary action against a student when you're 5% unsure that they did anything wrong. However, I have seen students being called in for review based on reports from such software.

There are also preliminary studies of AI-detection tools flagging the human-authored work of non-native speakers for plagiarism far more than those of native speakers. 

# _Looking Ahead_
Kunal Shah
Prompt engineering
Students take the easy way out, it can be very detrimental too
people barely read cases anymore

### Redesigning Curriculum
I'll take the case of a startegy course of mine that had articles, case discussions, and guest lecturers. If you've ever taken a startegy course, you know that AI is a gold mine to do those assignments. This course used to let students pick _any_ company/product of their choice and allow them to write an open ended paper on it. This year however, the professor simply added that students must incorporate course readings and class learnings from speakers and fellow students into their paper. 

This simple change made the course more demanding by an order of magnitude, but I also paid more attention in this course than any other. We now one had to make continuous notes of relevant peer comments, transcribe guest lectures, and review all the readings! This reminds me of the BCG/HBS study that showed that AI reduced the performance gap of the top and bottom half from 28% to 16%. Strategies liek this course's can help bring back a meaningful difference between an A+ and B. However, there needs to be consideration for the additional time that such changes might demand from students.  

# Appendix:

A summary of academic AI policies from syllabii of 30 business school courses:
- You may use AI-powered programs to assist with all assessments **except for the midterms and final exam**.
- AI text generation tools may present incorrect information, biased responses, and incomplete analyses; they are not yet prepared to produce text that meets the standards of this [law] course.
- To adhere to university values, you must cite any AI-generated material (e.g., text, images, etc.) included or referenced in your work and provide the prompts used to generate the content.
- Using an AI tool to generate content without proper attribution will be treated as plagiarism and reported to the Office of Academic Integrity.
- Permitted to use AI for programming assignments; must not solely rely on AI; AI-generated content must be cited.
- **Expected to use AI** tools like ChatGPT for analyses; AI-generated material must be properly attributed.
- Use of AI-generated tools is **prohibited** for assignments; considered plagiarism.
- Use of AI Generators: You may wish to use AI in this class. Learning to use AI is an emerging skill, and I **welcome the opportunity** to meet with you to provide guidance with these tools.
- AI tools are permitted to help you **brainstorm topics or revise work** you have already written. If you provide minimum-effort prompts, you will get low-quality results. You will need to refine your prompts to get good outcomes.
- Proceed with caution when using AI tools and do not assume the information provided is accurate or trustworthy If it gives you a **number or fact, assume it is incorrect** unless you either know the correct answer or can verify its accuracy with another source. **You will be responsible for any errors** or omissions provided by the tool. It works best for topics you understand.
- I encourage you to use artificial intelligence (AI)-powered programs to help you to learn how to negotiate more effectively. We will be conducting a couple of negotiations using AI-driven counterparts, as we expect that you will be negotiating with bots and other forms of AI in the world outside of this class.

---

Note: My experience has been limited to the graduate **business** school of **one university**. Cases, reflection papers, and ambiguous class discussions are a big part of business school courses (especially strategy and marketing courses). These have influenced my view of AI in the classroom and are likely to be very different from Ai in a journalism or engineering program.


  

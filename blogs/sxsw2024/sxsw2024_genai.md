---
layout: blog
title: South by Southwest 2024 - Generative AI
date: 15 March, 2024
---

## Table of Contents

- [GenAI Unlocking Creativity](#genai-unlocking-creativity)
- [How AI is changing the art of the job](#how-ai-is-changing-the-art-of-the-job)
- [Enabling AI Everywhere: Intel](#enabling-ai-everywhere-intel)
- [Amazon AGI](#amazon-agi)
- [AI Agents: Authenticity vs Augmentation](#ai-agents-authenticity-vs-augmentation)


## GenAI Unlocking Creativity

> Creativity is both fueled and limited by experience, which can overwhelm those who are expected to be creative but were never taught how. But generative AI offers a shortcut to unleash the creative in all of us. This session will demonstrate how generative AI helps power innovative ideas, design solutions, and artistic expressions with real world examples from Canva and HubSpot customers, from creators and small businesses to cross-functional teams at Fortune 500s.
> 
> Cameron Adams, co-founder and Chief Product Officer, Canva<br>
> Kipp Bodnar, Chief Marketing Officer, HubSpot

- CanvaGPT is among the highest rates apps on the GPT store
- Canva launched text to image capability in Nov’22, same month as ChatGPT’s launch. That product was shipped in 6 months, their fastest launch

> Humans suck at prompting ~ Cameron Adams

- Editing as a skill
    - Great PMs are great editors.
    - Editing is a skill applicable across multiple industries roles.
    - Especially critical in a GenAI world
    - Get better at asking questions. Think about what your job could look like if you freed up your mind. You’re probably going to have that freedom soon, start planning for it.
- Hubspot State of AI report:
    - AI now saves 2-2.5h per day
    - 95% say they spent less time on manual work
    - 83% use this time for creative work
- HubSpot campaign assist tool creates landing page, URLs etc and let people overcome creative blocks by freeing up administrative tasks.
- Example of GenAI in Canva:
    
    Canva’s use case development in GenAI is mind-blowing. Not only do they have 10 apps with a large variety of features, but they also have many more on [their app store](https://www.canva.com/your-apps/). 
    
    - Magic Media - Turn your imagination into reality by watching your words transform into images and videos (Magic Media’s text to image, DALL·E by OpenAI, and Imagen by Google Cloud)
    - Magic Switch - Swap formats, languages, and dimensions for multiple platforms, or auto-translate them without leaving the page.
    - Magic Expand - Extend an image in any direction. Fix awkward framing, save zoomed-in images, or turn a vertical shot into a horizontal one in seconds.
    - Magic Grab - Redesign images to select and separate the subject of your photo so that you can edit, reposition, or resize it.
    - Magic Edit - Reimagine your image and add to, replace, or edit it with a short written prompt.
    - Magic Eraser - Make your subject stand out. Brush away unwanted details and distractions from your photos.
    - Background Remover - Remove backgrounds from images and videos in a single click.
    - Magic Animate - Automatically apply the perfect animations and transitions to your entire design.
    - Magic Morph - Transform words and shapes with a simple written prompt. Magic Morph applies effects to text and shapes to quickly create patterns and textures.
    - Magic Write - Quickly reword sentences or paragraphs and summarize or expand your text.
- Described an example at Canva’s recent HR all-hands:
    - Magic Switch: Convert whiteboard to a document
    - Magic Write: Convert the document to a blog style
    - This process would have taken a team of 3 people a day
    - Magic Translate: Convert the MoMs to other languages for global teams
- Hubspot: AI-personalized emails have 80% increase in conversion rate. The email copy has references specific to the recipient’s industry/role. Using RAG with a vector DB of Hubspot’s blogs, courses etc
- Canva 2024 Focus: The design process is very feedback driven. Aiming to make Canva’s features support faster feedback loops.

## How AI is Changing the Art of the Job

> From resume-building to navigating that first job, to taking on new responsibilities, AI is disrupting how we seek job opportunities and employers identify and train talent. But, can AI level the playing field or will it perpetuate societal biases? How critical will knowledge of AI be for career success? Purposeful applications of AI can shape a more equitable and meaningful future of work for employees and managers alike. Join to explore how AI can unlock opportunity, identify untapped talent, and help all employees contribute and advance faster in their careers.
> 
> Nickle LaMoreaux, Chief Human Resources Officer, IBM<br>
> Jim Link, CHRO, SHRM Society for Human Resource Management<br>
> Garrett Lord, CEO And Co-Founder, Handshake<br>
> Jena McGregor, Forbes

- Probably just 2% of jobs are fully replaceable by AI. These might just be counter balanced by jobs created by AI.
- But for bulk of us in the 98%, there will be a need to change the way to do our jobs.
- Given this need to change and the fact that capability and tools are so dynamic right now, companies should look to add young talent that can bring the savviness to their teams.
- Won’t the increased needs decrease future hiring needs?
    - Depends on whether your company/economy is growing or stagnant/shrinking.
    - Might see wage growth for same roles.
- [AI + HI](https://conferences.shrm.org/ai-hi-project)
- Stats
    - 60% of people currently surveyed see their job style changing with AI
    - Only 25% of organizations are using AI.
    - 66% of them started in the last two years.
    - Average student takes 3 jobs in the first 5 years of their career and changes industries twice.
- IBM
    - IBM is a skills first organization. 50% of their roles do not need a bachelors degrees. Apart from the largely commented about biases of AI, they’d be concerned about AI inferring education qualifications as a marker for quality.
    - IBM does not use AI to prioritize resumes yet. The only application in hiring function is a chatbot.
    - AI Principles:
        - Always label AI processes
        - Explain the models. Input, output, reasoning.
        - AI is not a decision maker
- Using AI to transcribe interviews and identify which interviewers need more training and might be asking biased questions.
- Conversational AI unlocks the ability for employees to ask questions they might not have asked a human such as vulnerable coaching questions or personal benefits needs.
- AI regulations around the world are still uncertain. HR and employee rights are a regulated function too. So until there is sufficient global clarity, MNCs are hesitant to do meaningful experimentation in it.

## Enabling AI Everywhere: Intel

> Generative AI technologies such as ChatGPT have accelerated our journey to an “AI Everywhere” reality. Discussions abound on whether these AI models will replace or complement human ingenuity for a wide range of professionals, but the societal value of unlocking such critical technologies cannot be overstated. While the explosion in size and complexity of the models and their voracity for data and compute naturally lend itself to making Gen AI the domain of a few, early design decisions emphasizing the use of ubiquitous hardware and open software are critical to ensuring wider future access.
>
> Wei Li, VP AI and Analytics, Intel

Intel’s AI Stack:

| Models | Bloom, BioGPT, LLaMa, Stanford Alpaca |
| --- | --- |
| Open Software | PyTorch, HuggingFace, DeepSpeed, FastRAG |
| Hardware | Zeon, Gaudi, GPUs
Designed for deep learning and keeps price performance in mind |

- Pre-trained → Supervised fine tuning → RLFH (Reinforcement learning w/ human in loop)

AI development at Intel:

| Step | Done by |
| --- | --- |
| Pre-trained models | [Mistral](http://mistral.ai)  |
| Supervised fine tuning | Intel |
| RLFH (Reinforcement learning w/ human in loop) | Intel |

Intel’s GPU AI Software stack:

| Domain APIs | HuggingFace, DeepSpeed, Mosaic |
| --- | --- |
| Deep learning frameworks | Tensorflow, PyTorch, Intel extensions.. |
| Language and models | Triton, TF libraries, oneMKL |

## Amazon AGI

> Amazon believes AI is the most transformational technology of our time, capable of tackling some of humanity’s most challenging problems. That is why the company is investing in generative AI to responsibly develop and deploy large language models (LLMs) across all of its businesses. These advancements are part of Amazon’s long-term pursuit of Artificial General Intelligence (AGI).
> 
> Vishal Sharma, AGI VP, Amazon<br>
> Ryan Heath, Axios

|  | Level | Amazon’s approach |
| --- | --- | --- |
| L3 | Use cases (shopping, smart assistants etc) | Innovating |
| L2 | Models | Open approach, using multiple models |
| L1 | Hardware | Innovating |

- Any sophisticated AI use case is combination of multiple models of varying complexity. For instance Alexa is ~30 models. The one that listens for the ‘Hey Alexa” trigger is different from the Voice-to-text model that follows it.
- GenAI applications at Amazon:
    - Advertising - Image processing for product displays. Creatives are the most expensive part of advertising.
    - Selling - Generating product listings
    - Software - Code Whisperer has shown to generate 50% increase in efficiency. Eg - 5 developers were able to perform an upgrade in 1000 applications in a few days.
    - Alexa - Preview is live that lets you have fluid and natural conversations with Alexa.
    - Robots - 750,000 robots across all Amazon locations. Even incremental improvements in robotics changes a lot for us.
- People in the US are (5 times more) more skeptical about AI than in people in Asia
- Amazon leadership principle that comes up a lot for AGI - Success and scale bring broad responsibility
- Unsure of where future architectures are heading, but for now RAGs that connect to a knowledge graph or vector database are the best solution for reliable GenAI.
- Amazon [TitanText LLM principles](https://aws.amazon.com/machine-learning/responsible-machine-learning/titan-text/)
    1. **Controllability:** Explores the control levers over Titan model behaviors, including pre-training and fine-tuning data and filtering processes.
    2. **Performance Expectations:** Illustrates how Titan Text performance varies across different customer applications and workflows.
    3. **Test-driven Methodology:** Outlines the comprehensive testing approach, including automated benchmarking, human evaluation, and red-teaming.
        1. **HELM Benchmarks:** Introduces Stanford's Holistic Evaluation of Language Models and its use in comparing LLM performance.
        2. **Human Evaluation:** Discusses the importance of human judgment in assessing LLM effectiveness, especially for complex tasks.
        3. **Independent Red-teaming:** Describes continuous evaluation by a skilled team to identify and mitigate issues in Titan Text.
    4. **Safety:** Outlines safety measures, alignment with human rights principles, and customer responsibilities in testing for safety.
    5. **Fairness:** Addresses bias mitigation efforts and measures to ensure fair treatment across demographic groups.
    6. **Explainability:** Offers techniques for understanding Titan LLM's decision-making processes and attribution of information.
    7. **Veracity:** Highlights challenges in ensuring completions align with facts and trusted sources, and the role of RAG.
        1. **General Knowledge:** Evaluates Titan Text LLMs' performance in answering general knowledge questions across various datasets.
        2. **RAG:** Discusses the performance enhancement with Retrieval-Augmented Generation.
    8. **Robustness:** Measures Titan Text's stability and performance under perturbations across different datasets.
        1. **Orchestration:** Describes Titan Text Express's capability in coordinating tasks and interactions with other tools or services.
    9. **Privacy:** Assures customer data privacy and outlines privacy measures implemented in Amazon Bedrock.
    10. **Security:** Details security measures in place for Titan Text LLMs, including encryption, access control, and monitoring.
    11. **Intellectual Property:** Offers IP indemnity coverage for outputs of generally available Titan models.
    12. **Transparency:** Emphasizes providing information and feedback channels to customers, and the responsible use of Titan Text.
    13. **Governance:** Outlines methodologies and practices to ensure responsible development and deployment of Titan Text.
- Alexa hunches - [The science behind Hunches: Deep device embeddings - Amazon Science](https://www.amazon.science/blog/the-science-behind-hunches-deep-device-embeddings)

## AI Agents: Authenticity vs Augmentation

> Social VR allows multiple users to synchronously interact in a shared virtual space & presents an exciting future in the metaverse. While interactions mostly involve human users, advancements in generative AI have hastened the mass creation & integration of AI-controlled virtual agents in social VR. Organizations may be tempted to use this quickened pipeline to populate social VR worlds with dynamic agents, though there are factors to consider.
> 
> Grace Ahn, The University of Georgia<br>
> Blair MacIntyre, JPMorgan Chase & Co.<br>
> Bree Mcewan, The University of Toronto<br>
> Daniel Pimentel, University of Oregon
> 
> [Event Link](https://schedule.sxsw.com/2024/events/PP133972)

- We (the adults) are developing a  metaverse that we think is normal. Thats not necessarily the best possible version of it.
- For instance kids who are exposed to metaverse growing up find it ‘normal’ to have avatar friends that they might never meet in-person.
- A possible metaverse future is one where we have our own virtual lounges that your friends come to visit us in.
- AI agents can be like dogs when you go dog-walking in a park - a reason to begin a conversation that would not have happened otherwise. A means to identify shared interests.
- Educating for the metaverse is so diverse:
    - Young children are vulnerable since they have leftover effects of their time in virtual worlds
    - Teenagers are likely the easiest to train
    - Adults are the hardest to train! They can’t forget the UX they are familiar with.
- There will be a need for Perceptual Engineering - i.e. not just UI engineering for realism of virtual worlds, but making interactions in it similar to human interactions
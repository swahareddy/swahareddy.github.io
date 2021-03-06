---
layout: blog
title: A picture speaks a 1000 words 🖼 ℹ
---
I'm not go into the history or philosophy of this adage. And as for its meaning, it's self explanatory.
## How did I get here?
When I was playing with GPT2, [teaching it to talk like my friends](https://github.com/swahareddy/gpt2AI_whatsapp_simulation), I was feeding the untrained model random internet snippets. And some of the stuff it was dropping was mind blowing. I could see why OpenAI was worried about fake news like applications of this.

>I gave it the first sentence from [this](https://www.wikiwand.com/en/Abhinandan_Varthaman) wikipedia page. Going forward, I will be **denoting the input in bold** and the text that follows will be the output.

>**Wing Commander Abhinandan Varthaman VrC (born 21 June 1983) is an Indian Air Force fighter pilot who,[3][4] during the 2019 India–Pakistan standoff, was held captive in Pakistan for 60 hours after his aircraft was shot down in an aerial dogfight.** He did not know when, or why, he was captured, however, he had been deployed on an Indian airbase to a "terrorist safe haven," where to say "these are my terrorists."[10]
>His name was Abhinandan, during the battle.In 1940, at the age of twelve, he went to Syria to fight with the Chinese Empire.[14] He was in a situation in which the two American servicemen were in battle to protect them from friendly fire from China.[13]
>
>In 1946, Abhinandan was in the Indian Air Force as part of a Special Observership Program, which allowed him or the other pilots in Indian Air Force air-force combat planes to fly without being "satellites".[18] However, he had lost several other pilots, and he would not be able to perform the operation if he was flown to an Indian airbase.
>
>In 1946, during the Indian Army's losses from an Indian plane crash, Abhinandan was given the task of flying a Apache and other AN-100/US/IM-100 aircraft. He was given the task of flying a AN-100 aircraft that was to carry up to 8 more squadrons of 8 aircraft, which consisted of 15 of the aircraft each, with the number of aircraft flown by all American and Russian Air Force, which included two of the planes being used by Mr. V.V.) Abhinandan had been assigned to the United States Air Force, and had been assigned to India from the Department of Defense's Special Observership Program (FSPP).

So I really wanted to be able to tell stories based off images. But I needed a few lines of text based on the image to feed as context to the model. And the Google cloud APIs I found were for [individual labels](https://cloud.google.com/vision/docs/labels) and [object detection](https://cloud.google.com/vision/docs/object-localizer)^. So I left it at that. 

 But recently I came across [this](https://github.com/karpathy/neuraltalk2) open source model to auto-caption images. ([This](https://play.google.com/store/apps/details?id=com.google.android.apps.accessibility.reveal) app by Google is also really cool) Unfortunately I was unable to install it due to my laptop (and google colab) being incompatible, but I am still documenting my non technical observations in this post.
 
 ---

## Using actual [image-caption pairs](https://cs.stanford.edu/people/karpathy/neuraltalk2/demo.html) from the NeuralTalk2 model.
 
I used [this](https://deepai.org/machine-learning-model/text-generator) tool to make the text predictions as it gives large outputs. A better one is [this](https://transformer.huggingface.co/doc/gpt2-large) since GPT2 prediction parameters can be controlled, but it predicts only few words at a time. In reality I will want a combination of both like I have [done earlier](https://github.com/swahareddy/gpt2AI_whatsapp_simulation/blob/master/Whatsapp_Chat_simulation_by_OpenAI's_GPT_2.ipynb). 

><img src="ideas_box_images\picture1000words\surfboard.jpg" width="20%">
>**a man riding a wave on top of a surfboard** 
>I was riding high on a wave at Ormeau Surf and Rimming and Wetland. On the way, I stopped at the water board for a short delay.
>The guy who was riding in a wave tank was clearly a person from different parties, a lot like the one I was in Australia at the time.
>He was dressed in a green shirt with a gold hoop earring and no headscarves.
>I rode my wave there for just one second before it stopped raining.
>What prompted the ride? "I suppose I shouldn't throw up", I say confidently as I wait out the door.
>
>"My friends were out of town when they caught me surf surfing. As I stopped at a water board, I realised it was getting really long. I looked at the front side mirror and realised where I was going. I pulled the paddle out of the water, excitedly scooped it up and stepped over the side. The wave crashed out into the side of the board.
>I got out of the water and took a break to rest. When I came back on to the board, I pulled my head back and gingerly pulled it out. The other paddleboarders, who were right next to me, were still running along with me. I could feel the wind shifting in my face.

><img src="ideas_box_images\picture1000words\umbrella.jpg" width="15%">
>**a man walking down a street holding an umbrella** 
>He was wearing a gray cap. Asked why did something that made police say that he was wearing them, the man said that he saw someone wearing a light-blue shirt.
>
>Officers who were already doing a heavy-handed internal-defense stance were also being charged. Officers are prohibited to handle emergency vehicles while conducting internal-defense activities.
>Police have been the ones responsible, but most recently have been cited for the breach of public peace on a Portland Public Transit bus.
>The incident in which a man was killed last year as another suspect was being held in the same room. Two other suspects had been arrested for resisting arrest.


><img src="ideas_box_images\picture1000words\food.jpg" width="15%">
>**a group of people standing around a table with food** 
>, beer—food was distributed, but no dough. They asked me, "What are you making?" I answered, "We're from Mars."
>There's a great story here. In 2013, NASA released the Mars Reconnaissance Orbiter. The mission was a cooperative effort between NASA, the European Space Agency and several European member states.
>
>At the time, NASA had just launched its Mars Polar Satellite, an attempt to collect data on the global water circulation network in Mars. A computer model developed by Nasa meant it had a pretty complicated record: Mars Reconnaissance Orbiter was taking a detailed look at water distribution in the Martian atmosphere, it had to track the surface at a scale previously used to catalog the planet's surface and track the movement patterns of water molecules.


><img src="ideas_box_images\picture1000words\dog.jpg" width="15%">
>**a woman is sitting on a bed with a dog**
>I was born with three different minds: a two-headed dog, my two-headed cat, and I
>The man who sent me to the hospital told a girl I don't like cats because she thinks they are animals — a malevolent sort of dog that just can't be trusted.
>
>While I was at my friend's house, they had my son with me, and I told him no. I'd only have him to go to his house.
>His mom, Beth, told me an adult had come there recently to take me to her son's room — a nice, quiet room. She would never let me bring the kids to the room at home, even if they were sitting on the floor.


><img src="ideas_box_images\picture1000words\giraffe.jpg" width="15%">
>**a group of giraffe standing next to each other on a field** at the Taroomba River near Nairobi.
>The three giraffe guards are one, the head and a man who has an open air rifle with a "good eye", who is a member of the local chapter of the International Union for Conservation of Nature.
>
>"Our goal was to get a photograph and if anybody could see me they would be all over me, but I can still see them. The only thing I can get from that is a photo of them with me, because I'm an adult and I don't want them to be associated with me at all. I need someone to tell me who this guy is, the one that says there's a woman we've been having dinner with and she's saying that he was the one who started this," said Garek Menguik.


><img src="ideas_box_images\picture1000words\kidsuit.jpg" width="15%">
>**a man in a suit and tie standing in a room** with his laptop and electronic device, according to a report.
>The report was forwarded to the Department of Justice by State Attorney Bill Montgomery on an afternoon Monday. Montgomery said the FBI had no comment.
>
>On Thursday morning, an assistant attorney general for the U.S. Attorney's Office in Columbus, Ohio, was responding to an email from a department official in Washington about the matter.
>A lawyer for the FBI, Robert Burton, said he was unaware of the internal investigation.
>During a conference call on Friday, Burton told aides: "I'm not supposed to talk to this individual right now."

---
As you can see the outputs are not what anyone would have liked. But I still have not given up hope because the issue with using NeuralTalk type models is that are trained on the [COCO dataset](https://cocodataset.org/#explore) which **gives crisp outputs that are not sufficient context for a good GPT output.**

*I want to try a more raw NLP approach like comparing the embeddings of a group of ^detected labels/ objects with that of wikipedia or some other very large corpus to find well written sentence(s) that can be fed instead of crisp captions.*
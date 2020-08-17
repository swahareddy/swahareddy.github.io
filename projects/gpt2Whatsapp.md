---
layout: project
title: "gpt2 Whatsapp Simulation"
author: jill
github_repo: https://github.com/swahareddy/gpt2AI_whatsapp_simulation
---
[comment]:2020-08-16
# Simulation of Whatsapp conversations
Fine tune Open AI's GPT2 on Whatsapp Chats to generate conversations. Works for both group chats and private chats.

<!-- <a href="https://github.com/swahareddy/gpt2AI_whatsapp_simulation" class="icon brands alt fa-github"><span class="label">GitHub</span> Check out the code on GitHub</a> -->

The following steps are for running a Colab notebook, you can also run it locally. In that case it'd take longer since you don't get Colab's GPUs and you'd also have to replace the google drive folders with local ones.

There are 4 versions of the pretrained model. I have used the second largest one (774M, Large, ¬3GB). Colab (free version) was frequently crashing with the extra-large model.
I won't be describing GPT-2 in detail, instead I'd encourage you to check this out if you are not familiar with it - [https://openai.com/blog/better-language-models/](https://openai.com/blog/better-language-models/)

## How to use:
1. Export chats from Whatsapp mobile application. This will give you a file with a name like `WhatsApp Chat with Sushil Khairnar.txt`

<img src="gpt2Whatsapp_images/WhatsApp%20Image%202020-08-02%20at%2011.52.43.jpeg" height="240" width="330"> <img src="gpt2Whatsapp_images/WhatsApp%20Image%202020-08-02%20at%2011.52.43%20(1).jpeg" height="240" width="340">

2. Create the following hierarchy in your google drive 
<img src="gpt2Whatsapp_images/gdrive_structure.png" height="240" width="330">

3. Upload the `original_chat.txt` in your google drive in the folder `Original Chats`

4. Run the jupter notebook on Google colab.

5. Check your output (`gpt2_gentext_sushil_khairnar_20200802_084751.txt`) in the `Predicted Chats` folder

> _I have intentionally cleared outputs of the cells before pushing the notebook to this repository, since both the original and predicted chats should be private. But rest assured, you'll be seeing some really interesting (and probably disturbing :P) results._

## Misc

* The training checkpoints can be backed up into `Chat models` in case you want to come back and use the fine-tuned model later. This code cell is commented by default since the checkpoint size is >3GB.

* The copy of files (`generated_text`) from Colab local runtime -> GDrive is a little slow, give it a couple of minutes

* Drop a mail at swahareddy@gmail.com for any comments.

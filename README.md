Hey, this post is here to give an overview of how this site technically works. I'll be defining the components and the reasons for my choices and linking relevant tutorials at the end. After going through this you can probably clone my repo, delete couple of folders that have these posts and put in your own content.

### Where I was coming from?
Although I am a developer, I have always worked o the back-end of stuff. Honestly, my experience with any front-end technology was as limited as just knowing `<HTML>` tags. But as I started doing more and more projects for fun, I realised that I do not want to be shy about this going forward.

But at the same time I felt that it would be a shame for a professional developer to use Wordpress, Wixsite etc, although they are great solutions. And now that I have built this, I think it is as easy as any of these tools!

## What is needed for a website?
While knowing web development is not a prerequisite , Some basics of HTML (maybe Bootstrap and CSS too) would be good to have. You should be able to use Github Desktop atleast if not git command line.
### 1. Web (HTML) pages
Don't worry, you barely need to use any HTML after an initial setup. I write all these posts in **[markdown](https://commonmark.org/help/)** which is plain text with minimal formatting. But if you right-click and view page source (`Ctrl+U` on Chrome) on ony page here, or elsewhere on the internet you see HTML.

So the most important part of this website is a tool called [Jekyll](https://jekyllrb.com/). **This tool converts my simple markdown to HTML automatically along with themes, header, footers etc**.

**This is how easy it was for me to write this blog!**
```
---
layout: project
title: How does this website work?
github_repo: https://github.com/swahareddy/swahareddy.github.io
---

Hey, this post is here to give an overview of how this site technically works. I'll be defining the components and the reasons for my choices and linking relevant tutorials at the end. After going through this you can probably clone my repo, delete couple of folders that have these posts and put in your own content.

### Where I was coming from?
Although I am a developer, I have always worked o the back-end of stuff. Honestly, my experience with any front-end technology was as limited as just knowing `<HTML>` tags. But as I started doing mor..
.
.
```

1. [Get a theme](https://www.youtube.com/watch?v=u-RLu_8kwA0&t=291s)
2. [Install Jekyll](https://jekyllrb.com/docs/installation/windows/)
3. [Get started on Windows](https://www.youtube.com/watch?v=HlfvhkDuicc)
4. [Elaborate tutorial](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB)


###  2. Hosting

When you use Jekyll (or anything else like Flask, Angular etc) and get a good website ready, it is still running on a local link that only you can see like `127.0.0.1:4000/about.html` and not at a publicly accessible one like `swahareddy.github.io/about.html`. This is the simplest step.

In order to do this, you need to use a hosting service. To put it simply, it is a fancier online storage of your photos, markdown files, templates etc. Most people use paid hosting services, but now we have an option to do this for free! This is why I am using Github Pages.

   1. [This](http://jmcglone.com/guides/github-pages/) was sufficient for me.
   2. [Another option](https://towardsdatascience.com/how-to-create-a-free-github-pages-website-53743d7524e1)

### 3. Domain name
Now that you have converted `127.0.0.1:4000/about.html` ➡ `swahareddy.github.io/about.html`, you  might still want to convert `swahareddy.github.io/about.html` ➡ `swahareddy.com/about.html`.
**This is purely optional**, and the only place you'll need to pay anything. 

I am yet to make this happen. I'll update it once its done. 

---

If you have done Steps 1 and 2 from above, you can try more fun stuff like showing [PDFs](myspotify.html), [visualisation dashboards](whatsapp_analytics.md), [Google Sheets](/blogs/self_learning.html), [Presentations](/blogs/ait_macroeco.html), [Animations](/blogs), [GIFs](/blogs), [Instagram](/blogs/instagram_preview.html) etc

<p align="center"><img src="https://media.giphy.com/media/M33UV4NDvkTHa/giphy.gif" width="24%"/></p>
<!-- <div style="width:10%;height:0;padding-bottom:58%;position:relative;"><iframe src="https://giphy.com/embed/M33UV4NDvkTHa" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div> -->

### Misc
* I found Jekyll *blogs* confusing. If you can help me out, let me know! This has not been a problem for any of my posts (yet).
* I'm not able to use my layouts in nested folders 
* I've never worked with CSS, so I am relying on standard styling and a theme and not customising anything

### Backlog
1. Visitor analytics?
2. SEO optimization (XML sitemap etc)
3. Automate RSS feed file generation
4. Customise my 404 page
5. Automate a script to check if there are any broken links

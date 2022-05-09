---
layout: project
title: How biased is the news org/ person?
github_repo: https://github.com/swahareddy/political_polarisation
---

This image was the inspiration for this project. I wanted to make the X axis of this:
![alt_text](media_polarisation_images\2d_scale.jpg){: width="70%" }
<br>Like this:<br>
![alt_text](media_polarisation_images\linear_scale.jpg ){: width="50%" }

## My idea:
1. Define a right and left wing corpus with words that those wings are usually associated with 
    1. Manually decide 20-30 accounts (politicians, commentators, spokespersons etc..) each from right and left wing for loud polarised people
    2. Use Twitter API to input tweets from them
    3. For every right-wing tweet:  
        1. Run GCP entity sentiment analysis
        2. Add entities with positive sentiment to right wing corpus
        3. Add entities with negative sentiment to left wing corpus
        4. There will be entities that are in both corpuses ('army', 'mahatma gandhi' etc).
        5. Do vice-versa for left-wing tweets
2. Now stream news like I did in [my other project](news_negativity.html)
3. Run GCP entity sentiment analysis on news data
4. Compare these entity sentiments with the above defined corpora
5. Calculate difference in % match 
6. Scatter plot and clustering of different news sources

These corpora would be at a national level, not same corpora for all international sources

```
Oversimplifying the scenario into a BJP vs Congress world. These are the twitter accounts I have used to build the corpus.
## INC
### List of INC spokespersons: [Official](https://https://twitter.com/i/lists/200025713/members)
['JM_Scindia', 'RajBabbarMP', '_SandeepDikshit', 'SATAVRAJEEV', 'VijayIndrSingla', 'Meem_Afzal', 'MYaskhi', 'SinghRPN', 'sushmitadevinc', 'dineshgrao', 'plpunia', 'GauravGogoiAsm', 'DrAMSinghvi', 'drajoykumar', 'khushsundar', 'shaktisinhgohil', 'JhaSanjay', 'DeependerSHooda', 'rajeevgowda']
### Others
['RahulGandhi', 'sunilkjakhar', 'srinivasiyc', 'INCIndiaLive']
---
## BJP
### List of BJP spokespersons: (Verified accounts)
['sambitswaraj', 'ShahnawazBJP', 'NupurSharmaBJP', 'gauravbh', 'GVLNRAO', 'AshwiniBJP', 'NalinSKohli']
### Others
['BJP4India', 'rammadhavbjp', 'JPNadda', 'BJPLive']
```

Did not include cabinet ministers since their tweets are overwhelmingly about their portfolios and not about the common narrative.

This could be extended to do the same for transcripts from YouTube videos of NDTV, Republic TV etc ([a data science heavy project](https://www.aclweb.org/anthology/W19-2110.pdf))
It could also be used to validate apparent bias in platforms, Eg - FB (right) and Twitter (left), and also *gauge how various subsections (read subreddits) are aligned on our scale*.  

## Relevant reads:
1. [https://www.cjr.org/innovations/measure-media-bias-partisan.php](https://www.cjr.org/innovations/measure-media-bias-partisan.php) - Good intro read for the concept. Specifically see the ‘armchair academics’ section
2. Similar manual projects:
    1. [https://www.adfontesmedia.com/interactive-media-bias-chart/](https://www.adfontesmedia.com/interactive-media-bias-chart/) for interactive link to source of 2D image above
    2. [https://www.journalism.org/2014/10/21/political-polarization-media-habits/pj_14-10-21_mediapolarization-08/](https://www.journalism.org/2014/10/21/political-polarization-media-habits/pj_14-10-21_mediapolarization-08/) link to source of 1D image above
    3. [https://www.allsides.com/media-bias/media-bias-ratings](https://www.allsides.com/media-bias/media-bias-ratings)
    4. Can use these to validate our outputs 

Unrelated, but interesting - [http://graphics.wsj.com/blue-feed-red-feed/#/president-trump](http://graphics.wsj.com/blue-feed-red-feed/#/president-trump)

## Progress so far
I have completed upto Step 1.3.3 (described [above](#my-idea))

Here is a small sample of what I extracted for tweets from a congress party spokesperson :

<blockquote class="twitter-tweet" data-theme="dark"><p lang="en" dir="ltr">After failing to contain the large scale migration,the BJP Govt is now indulging in inhuman act by forcing labourers to take bath in chemical solution.<br><br>This is shocking &amp; deplorable that the UP Police &amp; BJP Govt is using such tactics in the name of preventing corona outbreak. <a href="https://t.co/l2Iodi2Qcd">https://t.co/l2Iodi2Qcd</a></p>&mdash; Rajeev Satav (@SATAVRAJEEV) <a href="https://twitter.com/SATAVRAJEEV/status/1244534905981128704?ref_src=twsrc%5Etfw">March 30, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
| Entity Name               | Entity Type  | Entity Salience | Entity Senti Score | Entity Senti Mag | Translated tweet                                                                                                                                                                                                                                                                                                                                               | Date             | Hashtags                   | Username    | Link                                                       | Retweet | Likes | Replies | Retweets | Quoted tweet                                                  | Tagged accounts |
| ------------------------- | ------------ | --------------- | ------------------ | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | -------------------------- | ----------- | ---------------------------------------------------------- | ------- | ----- | ------- | -------- | ------------------------------------------------------------- | --------------- |
| Aarogya Setu              | PERSON       | 0.445995        | 0                  | 0                | 'Aarogya Setu' app programming code should be made open source. What is there to hide if there is nothing fishy?<br>#RahulFightsForIndia<br>Right Now                                                                                                                                                                                                          | 08/05/2020 06:13 | \['#rahulfightsforindia'\] | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1258641041659318272 | FALSE   | 372   | 4       | 108      |                                                               | \[\]            |
| people                    | PERSON       | 0.020684        | \-0.1              | 0.1              | Another example of vandalism of Gujarat police in the middle of lockdown. Instead of helping the Dalits, poor and laborers are being harassed. The government is there to solve the problem of the people - not to increase it. https://twitter.com/gopimaniar/status/1244902345684598789â€¦                                                                   | 31/03/2020 09:58 | \[\]                       | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1244927118032560129 | FALSE   | 225   | 10      | 67       | https://twitter.com/gopimaniar/status/1244902345684598789     | \[\]            |
| GujaratModel of Elections | PERSON       | 0.422432        | \-0.1              | 0.1              | #GujaratModel of Elections exposed. Gujarat Law Minister Bhupendra Sinh Chudasamaâ€™s election victory in 2017 declared unlawful, null & void by Gujarat High Court in a land mark judgement                                                                                                                                                                   | 12/05/2020 06:23 | \['#gujaratmodel'\]        | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1260093180730540032 | FALSE   | 4998  | 115     | 1528     |                                                               | \[\]            |
| Gujarat High Court        | ORGANIZATION | 0.034117        | \-0.1              | 0.1              | #GujaratModel of Elections exposed. Gujarat Law Minister Bhupendra Sinh Chudasamaâ€™s election victory in 2017 declared unlawful, null & void by Gujarat High Court in a land mark judgement                                                                                                                                                                   | 12/05/2020 06:23 | \['#gujaratmodel'\]        | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1260093180730540032 | FALSE   | 4998  | 115     | 1528     |                                                               | \[\]            |
| labourers                 | PERSON       | 0.049935        | \-0.4              | 0.4              | After failing to contain the large scale migration,the BJP Govt is now indulging in inhuman act by forcing labourers to take bath in chemical solution.<br><br>This is shocking & deplorable that the UP Police & BJP Govt is using such tactics in the name of preventing corona outbreak. https://twitter.com/KanwardeepsTOI/status/1244508599038009344Â â€¦ | 30/03/2020 08:00 | \[\]                       | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1244534905981128704 | FALSE   | 147   | 1       | 41       | https://twitter.com/KanwardeepsTOI/status/1244508599038009344 | \[\]            |
| BJP Govt                  | ORGANIZATION | 0.667285        | \-0.6              | 2                | After failing to contain the large scale migration,the BJP Govt is now indulging in inhuman act by forcing labourers to take bath in chemical solution.<br><br>This is shocking & deplorable that the UP Police & BJP Govt is using such tactics in the name of preventing corona outbreak. https://twitter.com/KanwardeepsTOI/status/1244508599038009344Â â€¦ | 30/03/2020 08:00 | \[\]                       | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1244534905981128704 | FALSE   | 147   | 1       | 41       | https://twitter.com/KanwardeepsTOI/status/1244508599038009344 | \[\]            |
| UP Police                 | ORGANIZATION | 0.00449         | \-0.7              | 0.7              | After failing to contain the large scale migration,the BJP Govt is now indulging in inhuman act by forcing labourers to take bath in chemical solution.<br><br>This is shocking & deplorable that the UP Police & BJP Govt is using such tactics in the name of preventing corona outbreak. https://twitter.com/KanwardeepsTOI/status/1244508599038009344Â â€¦ | 30/03/2020 08:00 | \[\]                       | SATAVRAJEEV | https://twitter.com/SATAVRAJEEV/status/1244534905981128704 | FALSE   | 147   | 1       | 41       | https://twitter.com/KanwardeepsTOI/status/1244508599038009344 | \[\]            |

You can find the notebook to do this over [here](https://github.com/swahareddy/political_polarisation).
I'm retiring this project due to time constraints but *if you'd like to complete this project, the main steps remaining are #4, #5 and #6, data science related.*

<!-- ### Comments
As I have read more about this, I have come to understand that using the concepts of right and left in India is not meaningful. If we have to we can do a pro-vs-anti government scale. -->
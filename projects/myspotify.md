---
layout: blog
title: A year of my Spotify <img src="misc_images\spotify.png" width="8%">
---
One of the easiest dashboards I have made. Particularly since the [data](https://docs.google.com/spreadsheets/d/1bIxNFQmPRpb_SoXTooEJ68SAH60S7Ups5J18iCuug2o/edit?usp=sharing){:target="_blank"} need not be cleaned so you can just reuse the template. Scroll down for instructions. 19,000 streamed songs in a year.

*[GDPR]: General Data Protection Regulation
This is thanks to EU's [GDPR](https://www.spotify.com/us/privacy/#privacy-center-rights){:target="_blank"} which mandates that consumers should have access to the company's data about them. And even though I use Spotify in a non EU country, the fact that they are headquartered in Sweden (in EU) and they rely on a [cloud provider](https://cloud.google.com/customers/spotify){:target="_blank"} that would have global resources means that I am eligible for GDPR's rights too.

<iframe width="100%" height="750" src="https://datastudio.google.com/embed/reporting/882eb2bc-367d-4afa-8b93-f8574bfde6b0/page/jnxUB" frameborder="0" style="border:0" allowfullscreen></iframe>

<!-- Observations:
* Weekly distribution: I listen to music while working  -->
>Caveat: Spotify even logs the songs that you skip over (so they have 0sec play time). Hence the `record count` can be slightly misleading. For context, I have 750 records with secPlayed=0, 5,000 records for <3sec 7,000 records for <15sec out of a total of 19,000 records. 

**To make this for yourself, just follow the instructions from [here](https://thenextweb.com/tech/2020/06/19/a-simple-guide-to-visualising-your-spotify-listening-data-badass-ly/){:target="_blank"}.** I have added a lot more visualisations in my dashboard, so you might want to copy my report instead. You'll just have to add a `secPlayed` field (`=msPlayed/1000`) in `manage added data sources`.

This project leads to two other thoughts:
1. Spotify provides some amazing information of songs (happiness, dance-ability, tempo, album cover etc) through [APIs](https://developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/){:target="_blank"}. Connecting to those APIs can lead to more interesting and even [interactive](https://developer.spotify.com/documentation/widgets/){:target="_blank"} apps.
2. I should explore more of my GDPR-enabled-data to see what can be inferred. Starting with [Google](https://myaccount.google.com/dashboard){:target="_blank"}?

![](misc_images/interpretation.pdf)
<object data="misc_images/interpretation.pdf" width="70%" height="500" type='application/pdf'/>

Other more evolved projects I found based on this data:
* [https://towardsdatascience.com/spotify-sentiment-analysis-8d48b0a492f2](https://towardsdatascience.com/spotify-sentiment-analysis-8d48b0a492f2){:target="_blank"}
* [https://towardsdatascience.com/i-wrapped-my-spotify-history-the-hard-way-93dc832d9b47](https://towardsdatascience.com/i-wrapped-my-spotify-history-the-hard-way-93dc832d9b47){:target="_blank"}

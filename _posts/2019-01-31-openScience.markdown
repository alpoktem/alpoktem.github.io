---
layout: post
image: "/img/guanyadors dtic.JPG.jpg"
title: How I used the MdM-DTIC Open Science Award for advancing my PhD research
date: 2019-01-31 21:01:00
---
I was awarded with the <a href="https://www.upf.edu/web/etic_doctoral_workshop/maria-de-maeztu" target="https://www.upf.edu/web/etic_doctoral_workshop/maria-de-maeztu">María de Maeztu DTIC-UPF Open Science Award</a> in the <a href="https://www.upf.edu/web/media/enoticies/-/asset_publisher/wdGAWZ7EMj53/content/id/170996266/maximized#.XD2lU1xKjcs" target="https://www.upf.edu/web/media/enoticies/-/asset_publisher/wdGAWZ7EMj53/content/id/170996266/maximized#.XD2lU1xKjcs">6th Doctoral Student Workshop</a> organised by Department of Information and Communication Technologies of UPF in 2018. This award is given to pre-doctoral researchers that give outstanding effort in reproducibility and visibility of their research. 

<p align="center"><img src="/img/guanyadors dtic.JPG.jpg" alt="Award winners at the 6th UPF-DTIC Doctoral Student Workshop" width="600"></p>
<p align="center">Award winners at the 6th UPF-DTIC Doctoral Student Workshop</p>

In this post, I will describe how I used the prize of 1000 EUR that I received to further advance my research. (This post originally was posted in the <a href="https://www.upf.edu/web/mdm-dtic/blog/-/blogs/open-science-award-to-alp-oktem-the-heroes-corpus-dataset?_33_redirect=https%3A%2F%2Fwww.upf.edu%2Fweb%2Fmdm-dtic%2Fblog%3Fp_p_id%3D33%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-1%26p_p_col_count%3D1#.XFIlD8_0kWo" target="https://www.upf.edu/web/mdm-dtic/blog/-/blogs/open-science-award-to-alp-oktem-the-heroes-corpus-dataset?_33_redirect=https%3A%2F%2Fwww.upf.edu%2Fweb%2Fmdm-dtic%2Fblog%3Fp_p_id%3D33%26p_p_lifecycle%3D0%26p_p_state%3Dnormal%26p_p_mode%3Dview%26p_p_col_id%3Dcolumn-1%26p_p_col_count%3D1#.XFIlD8_0kWo">DTIC-MdM blog</a>.)

I have used the 2018 MdM Open Science award that I received in the DTIC 6th Doctoral Student Workshop for the collection of a prosodically annotated parallel speech audio dataset called **_Heroes Corpus_**.

<p align="center"><img src="/img/heroes-corpus-logo.png" alt="Heroes corpus logo" width="300"></p>

A part of my thesis involves building of a speech translation pipeline to be used in automatic dubbing. I research on the reasons and ways to include prosodic characteristics (intonation, rhythm and stress) of the speakers' and actors' speech into this scenario. Developing such a pipeline requires parallel data, for training the translation model; and speech data since prosody is taken into account.

Speech data production is a highly costly process that involves script preparation, speaker selection, recording and annotation. Due to the inaccessibility of such an approach, I developed a framework to exploit dubbed media material which readily contains parallel and prosodically rich speech. The framework that I call movie2parallelDB provides an automation for this process by taking in audio tracks and subtitles of a movie and outputting aligned voice segments with text and prosody annotation. **_Movie2parallelDB_** is made available as an open source software in <a href="http://github.com/alpoktem/movie2parallelDB" target="http://github.com/alpoktem/movie2parallelDB">Github</a>.

The framework requires correctly labelled subtitles for both original and dubbed version of the movie. Although this is easy to find in the original language of a movie, it is often not the case in the dubbed language. Practical differences in the dubbing process and subtitling process leads to non-matching audio and transcripts and in turn hinders automatic extraction of the speech data. This means that a manual process needs to be followed to correct subtitles to match the dubbing script.

I decided to use a TV series called *Heroes* for this work as its Spanish subtitles were close enough to its Spanish dubbing scripts. Timing and transcript corrections were done for 21 episodes by two interns, Sandra Marcos and Laura Gómez. A part of the prize was used to finance their working hours.

<p align="center"><img src="/img/heroes.jpg" alt="Heroes TV series" width="300"></p>

The corpus extraction methodology that was developed during the process and the resulting corpus were presented in the [Iberspeech 2018 conference](/publications/2018-11-21-iberspeech1).

The resulting Heroes corpus contains 7000 parallel English and Spanish single speaker speech segments. Audio segments are accompanied with subtitle transcriptions and word-level prosodic/paralinguistic information. It is made openly accessible through the <a href="http://hdl.handle.net/10230/35572" target="http://hdl.handle.net/10230/35572">UPF e-repository</a>.

The rest of the prize was used to fund my final year registration fees and also a tutorial on "Educational dialog systems tutorial" that I attended in Interspeech 2019 in Hyderabad, India.

I am very grateful to have had this boost to my PhD work by the Maria de Maeztu programme and hope that it has further positive repercussions in the speech and translation research community through the resources that were made openly available. 

Finally, here's the poster I designed for the workshop that describes my methodology for prosodic-lexical punctuation restoration. (Special thanks to <a href="https://www.herzogelisabeth.com/" target="https://www.herzogelisabeth.com/">Lisa Herzog</a> for her artistic touch.)

<p align="center"><a href="/img/punkPoster_herz_full.png"><img src="/img/punkPoster_herz_small.png" alt="Alp Öktem's Interspeech 2018 poster for publication: Visualizing punctuation restoration in speech transcripts with Prosograph." width="700"></a></p>
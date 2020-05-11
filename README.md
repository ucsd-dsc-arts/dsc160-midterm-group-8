# Project Title

DSC160 Data Science and the Arts - Midterm Project Repository - Spring 2020

Project Team Members: 
- Mizuki Kadowaki, mikadowa@ucsd.edu
- Anurag Pamuru, anpamuru@ucsd.edu
- Shutong Li, shl636@ucsd.edu
- Rakesh Senthilvelan, rsenthil@ucsd.edu
- Praveen Nair, prnair@ucsd.edu

## Abstract

(10 points) 

For the project proposal, please write a short abstract addressing the questions below. You should replace the entire contents of this section with one to two paragraphs addressing the following:

- What is the data set that you are going to analyze?
- What is your research question? 
- What is your hypothesis about the results? 
- What features of the data will you use to address your question? 
- What techniques and software tools will you use to extract these features?
- What analytic techniques will you use?
- What forms will your results take? (graphs, charts, images, sonification, Wordles, etc)
- How are you expanding on topics we have covered in class? 
- Why is it interesting? (personally, culturally, politically, other)

For this project, we are going to analyze a broad group of influential hip-hop songs from the 1970s to today. The goal of the project is to cluster hip-hop songs based on a variety of audio features to quantify their similarities and differences, and to determine whether popular terms for classifying hip hop (based on factors like period, geography, and subgenre) are visible in these audio features. Our hypothesis is that artists and songs that share these sorts of qualitative similarities will also be considered more similar in audio analysis, but also that stylistic groupings (such as soul rap and trap music) will be stronger than identity-based groupings (for example, East vs. West Coast).

In order to conduct this analysis, we will use the Python package librosa, which will allow us to extract features such as mel-frequency cepstral coefficients (MFCC’s), chroma features, zero crossing rate, and other spectral features. Then, using a dimensionality reduction technique such as PCA, we can use the package sklearn to cluster and classify our data based on the extracted features. The results of this clustering should be available as graphs based on the dimensional reduction, within which we can make distinctions for different clusters. This project expands on the feature extraction we did in class by harnessing the domain knowledge we have about hip-hop classification and history to determine whether the sorts of classifications that listeners of hip-hop make have an underlying basis in measurable audio features. This analysis is also valuable in that it provides a quantitative way to understand high-level trends in hip-hop from its inception until today, and to also understand what previously unrecognized similarities there might be between works that we would previously not associate together.


## Data

(10 points) 

This section will describe your data and its origins. Each item should contain a name of the data source, a link to the source, and any necessary background information such as:
- What is your cultural data source? 
- When was it made?  
- Who created the works?
- Is it digital native, or is it some kind of scan, recording, photo, etc., of an analog form?
  
  
  The cultural data source we went with is a the top 2 hip-hop songs for each year from 1980 to 2020 as streamed on Spotify, a music streaming application. Alongside all of these songs, we added in songs from influential artists such as Kanye West, Jay-Z, 2Pac, and Travis Scott who did not show up on the Spotify data in order to further show differentiable features of different eras of music within the eras and account for highly influential figures in the era who were very popular during the years analyzed but do not perform as well on Spotify. The dataset was made on May 1, 2020 by drawing from the Spotify API and manual research done on different highly influential artists in the genre. The manual data analysis largely draws from Billboard charts from the years 2002 to 2020 and research on hip-hop centric websites such as VH1. The works were created by a wide variety of hip-hop artists who produced the music between 1980 and 2020. The dataset encompasses numerous subgenres and styles within hip-hop through the artists represented within the set. The music is all digital native: it has been recorded and released in the form, which allows for more accurate analysis of the audio data that will be drawn from these songs for this project. 

## Code

(20 points)

This section will link to the various code for your project (stored within this repository). Your code should be executable on datahub, should we choose to replicate your result. This includes code for: 

- data acquisition/scraping
- cleaning
- analysis
- generating results. 

Link each of your notebooks or .py files within this section, and provide a brief explanation of what the code does. Reading this section we should have a sense of how to run your code.

## Results

(30 points) 

This section will contain links to documentation of your results. This can include figures, sound files, videos, bitmaps, as appropriate to your domain of analysis. Each result should include a brief textual description, and all should be listed below: 

- image files (`.jpg`, `.png` or whatever else is appropriate)
- audio files (`.wav`, `.mp3`)
- written text as `.pdf`

## Discussion

(30 points, three to five paragraphs)

As a first step to visualize the music from our dataset, we used the bokeh library for all of the named features (in other words, everything except for the MFCC and chroma features.)

This is a culturally relevant analysis of the evolution of Hip Hop. In the 1960s, New York was affected by the white flight and a decline in industry and commerce and in the 1970s, New York City entered a fiscal crisis. The emergence of early hip hop artists like Afrika Bambaataa and the Sugarhill Gang led to the birth of an East Coast-centric sound in the late 1970s. With limited infrastructure, Hip Hop emerged as music that people could dance to and have fun as an escape from daily struggles. This is reflected in the highly danceable, loud, and simple lyrics. 

Example: Beastie Boys - “Fight For Your Right”
https://www.youtube.com/watch?v=eBShN8qT4lk

As Hip Hop entered the mainstream, DJs developed many different techniques from break beating, sampling, chopping, rap-skit and remixing, diverging their styles to involving jazz as well. Eric B. and Rakim revolutionized rap by using Hip-Hop as a way of expressing his political activism through calm rapping. Hip Hop became less about partying and dancing but more about self expression and often, politically charged. 

Eric B. & Rakim - “Paid in Full”
https://www.youtube.com/watch?v=zVPZX7MPQIw

As Hip Hop gained popularity and spread to South Central LA, there was a rivalry between rappers of the east and the west coast. With rappers such as Snoop Dogg, Easy E, Ice Cube, and, most famously, 2Pac playing into a budding rivalry between the East’s distinct flow and the West’s preferred “gangsta rap”. Hip-Hop styles evolved separately in the East and West. Although these two were the first major divide, countless sub-movements, such as Mos Def and Talib Kweli’s “Conscious Rap”,  Black Street’s “new jack swing”, Afrocentrism, Native Tongues, constantly redefined what it meant to be a hip hop artist. Artists like Puff Daddy, Biggie Smalls, and Eminem brought hip-hop into the norm in the late 90s with increased presence in the 2000s.
Since its inception, hip hop has become a borderless and universal cultural experience as a form of celebration, protest, and culture. In its journey from Harlem to the globe at large, we will analyze several key artists through hip hop’s many eras. Whether it be the aforementioned East vs. West divide, the eclectic beats and flow of the 90s, or the sample heavy tracks of contemporary artists like Drake and Kanye West. 

While our final results seemed to display no characteristics of similarity, distinct style patterns overtime or any clustering, despite the vast array of features used for analysis. However, through a more traditional analysis of Hip-Hop, taking into account cultural and historical movements, there are many different styles and trends of Hip-Hop that can be easily categorized and sound completely different just by ear. 





The first paragraph should be a short summary describing your results.

The subsequent paragraphs could address questions including:
- Why is this culturally relevant?
- How does your computational approach differ from the traditional art historical, musicological, manuel/subjective approach to analyzing your cultural subject? 
- How do you think the original artists/musicians would respond to this type of analysis? Would it change/inform their practice in some way?
- How do your results relate to broader social, cultural, economic political, etc., issues? 
- In what future directions could you expand this work?

## Team Roles

Provide an account of individual members and their efforts/contributions to the specific tasks you accomplished.

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
- Blog posts

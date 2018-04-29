---
layout: post
title: Design for Wellbeing
date: 2018-04-23 13:32:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img:  # Add image post (optional)
---
In this design sprint, we used the Affectiva Libraries to develop a website that responds to user emotion and promote wellbeing. We chose to analyze a user’s reactions or emotions while listening to a song on YouTube. Using the four emotions, joy, sadness, neutral, and screaming, users can impact the video by increasing the volume, skipping the video, keeping it the same, and muting the volume respectively. Our overarching goal was to get the user to discover a song or video that they think is interesting. Below is a demo video that highlights the key features of our project:

https://youtu.be/u4Yh94ZXraU

###  Design Process
We started off the project by using the 5 Sheet Design Process to develop practical ideas for our emotion detector. The following sections are an outline of the steps we took:

###  Brainstorming (Sheet 1):
Each of us thought of a few ideas that could be used to implement our emotion detector. We then discussed if each idea could be completed within the one week time frame we were given by evaluating the technical level needed. We also discussed how each design would be able to leave an impact on the user in terms of wellbeing. For the scope of our project, we defined wellbeing as helping the user be aware of how they are feeling while performing a task or recommend a task based on their mood.

We had six proposals and narrowed it down to three that we thought were promising to carry out. These three points included displaying an emoji based on the user’s facial expression, making the user aware of how they are feeling while attempting a problem, and recommending songs based on the user’s emotion at that moment.

###  Initial Design (Sheet 2, 3, 4):
After brainstorming and narrowing down to a few potential ideas, we started to sketch and see how they would look if we implemented them. We drew a design for each idea and flushed out the pros and cons as we were not sure which proposition would be more practical and interesting to execute.

We thought about displaying a big emoji depending on the user’s facial expression such as lifting a brow (confused) or opening their mouth in an “O” form (surprised). However, we determined that it would be pretty simple and not as meaningful in terms of promoting the user’s wellbeing, unsatisfying our goal.

Another idea was to have the user be able to see their emotions while solving a math problem for example. The program would then send messages or alerts to the user advising them to take a break or skip the problem if they seemed stressed out or give a harder problem if they are bored. We determined that although it would be an interesting concept to take on, it would be difficult to develop given the amount of operations and time needed.

The idea of recommending songs based on the user’s emotion was also a fascinating idea to our team. In a nutshell, we wanted to either display the emotions the user was feeling while having a pre-made song playlist run or determine the user’s emotions while playing video songs. For this one, we made two sketches as we were unsure whether to use YouTube or Spotify to integrate our playlist. We determined that this was both a practical and technically appropriate idea to implement, however, we knew it would be challenging to manipulate the emotion data from Affectiva.

###  Realization Design (Sheet 5):
Ultimately, we decided to go with the YouTube Emotion Detector idea as it seemed to be an appropriate project considering our time and technical skills. Additionally, we chose to use the YouTube playlist over the Spotify playlist since the former would be easier to embed on our website and would also be visually appealing to the audience. Another main point is that we wanted to focus on three emotions to narrow down the concept: joy, sadness, and sleepiness. Each emotion would effect the video currently playing. For example, happiness would increase the volume as the user would want to hear it more, sadness would skip to the next video in the playlist as the user would not want to hear the content, and sleepiness would mute the volume so the user does not get disturbed.

###  Formative User Testing
We wanted to test how effective our idea for the emotion detector would be and find areas to improve so we conducted some formative user testing. We conducted this process by using the Affectiva Demonstration Site to detect the user’s emotion and a YouTube playlist. Then, as the user felt each emotion we planned on detecting, we would manually adjust the video settings. We got a lot of useful suggestions and ideas on areas we could refine our emotion detector. Below is a list of this advice:

- Detecting a sleepy state is probably not practical, but have more than just joy and sadness
- Have the YouTube video and webcam next to each other so the user can watch themselves too without scrolling
- Do something with the background to give the site a more interactive feel
- Have a search bar so that the user can find their own videos as well
- Good concept with the videos since attributes change, such as volume, depending on the user’s mood

###  Final Product Development
Since we were not well acquainted with JavaScript or jQuery, building the first site was challenging. However, we found that there were a lot of reference sites, tutorials, and documentation for various functionalities we used in the YouTube API which made the process much easier. Moreover, understanding the output of the Affectiva code and parsing the emotion variables was difficult as we expected. With the help of other students in the class, our own team effort, and using coding tutorials, we were able to deliver a working YouTube Emotion Detector.

Using our sketch for the realization design, we implemented our first website design using Javascript/jQuery, HTML/CSS, and the Affectiva library. For the first step in designing the website, we incorporated the webcam, a YouTube playlist, and a search box that allowed us to expand our project by not only having a playlist for songs but also other videos for the user to watch.

We also wanted to incorporate many more of the suggestions the users gave us during the formative user testing phase into our final product. We discussed that it would be interesting to implement a screaming emotion, instead of the sleepy emotion, that would mute the video that the user was watching. We decided that if the user were yelling to someone, they wouldn’t want to hear the video so it would automatically mute. In addition, we also thought of including a neutral emotion that doesn’t affect the video playing as the user would probably have this emotion for the majority of the video. We then added these changes and made more progress on the site which resulted in the following code:

The picture above shows the final emotions we implemented: joy, sadness, neutral, and screaming. One of the major components of this project was assimilating an instance of the YouTube player within our website, as well as passing commands to said player in response to Affectiva’s interpretation of the user’s emotion(s). This was programmatically done using various conditionals to identify the “dominant emoji” (shown above) and then have different results from the dominant emoji at the given time.

###  Final Design:
Our final product below shows an example of the user reacting happily to the YouTube video on the right side of the page.

We added a background that changes color depending on the user’s mood just as the students had suggested in the testing phase. We used yellow for joy, dark blue for sadness, grey for neutral, and light blue for screaming. Furthermore, we implemented a confirmation box that gets the user’s approval before making changes to the attributes on the video they were watching which would allow for better usability. The start, stop, and reset buttons are for the user to determine when they are ready to start the webcam.

Overall, we were happy with our final design as it satisfied our main goal of promoting wellbeing by using the user’s emotion to give a meaningful response about their reactions to a YouTube playlist.

###  Feedback
We had our demo day for this project on 4/19 where we demonstrated our design to various other students in our HCI class. We got a lot of comments on where the design went well and where we could improve using the “I Like, I Wish, What if” format. Students liked the overall concept of the site, that a confirmation box appeared for the user to agree before moving on to the operations, the user could choose the video they watch, and the user could skip the video depending on their mood. Some areas students thought we could work on were being more clear about what each emotion caused, fixing the confirmation box, creating a YouTube playlist based on songs or videos the user reacted positively to, and adding more emotions to track throughout the video.

###  Looking Back
In the future, there are areas where we can refine our design for the YouTube video emotion detector. First, we could add brief instructions or details that include what emotion can be detected and what it does to the video. Second, we can fix the confirmation box to stop the video when it appears. Third, we can add the songs or videos that the user enjoyed to a playlist as they listen to further achieve our goal of wellbeing. Next, we can expand on the project and implement more emotions, such as being surprised or confused, to pause or replay the video for example.

Overall, better understanding and more time experimenting with Affectiva would yield us more control over what is being sensed- more like the expressions rather than the emotion. This would give us more options for functionality. Furthermore, using libraries like d3 or p5 we would be able to represent user data in beautiful graphs. This would make communicating data analytics to users quite easy.

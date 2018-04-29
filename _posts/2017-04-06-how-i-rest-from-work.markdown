---
layout: post
title: Design for Tension
date: 2018-04-10 13:32:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: dog2.jpg # Add image post (optional)
tags: [Holidays, Hawaii]
---
As far as controversy goes, the modern-day climate is one of toxicity and constant in-fighting. People are more than willing to go at one another’s throats just to get a “like” or to preach to crowds of non-existent listeners over their social media platform of choice. Political turmoil has rooted itself in the minds of the populous and a plethora of issues, ranging from environmental disasters to biological horrors, linger in the thoughts of the everyday man. However, throughout time, one debate, so tense and so hotly debated, has stood out from the others and has sharply divided the human race: whether dogs are better than cats (…or vice versa).

###  Initial Design
Our team set out to solve this problem by creating a bot that would try to make cat-lovers appreciate dogs more and dog-lovers appreciate cats more. Initially, we brainstormed what tense topics we could translate into a chatbot effectively and creatively. We considered tackling tense topics such as the opioid epidemic, gun control, and advertised gender roles in the eyes of children, but ultimately decided on taking on the lighter but more creative topic of dogs vs cats.

###  Drafting Ideas
After pinning down what argument we wanted to focus on, we delved further into how the chatbot should function and how it should be structured. We each drafted our own design for possible conversation flow charts that the chatbot could run through.

In order to gain a sense of the responses that we would be receiving, we constructed a survey, which was distributed out to the class via Slack. We recorded the results of the class to gauge why people preferred one animal over the other and the results were different than what we had expected. Cat lovers’ response to “why do you dislike [dogs]?” tended to be defensive while dog lovers did not hesitate to trash on cats. We found this intriguing and considered it while making our chatbot.

We eventually decided on simplifying the potential arguments into a tree that branches off into 3 routes: dog-lover, cat-lover, and neither. The dog-lover and cat-lover trees are pretty symmetrical; they both push the user to try and appreciate the other side more than they did initially via colloquial and funny dialogue. The neither branch’s goal is to convince the user to become interested in getting a pet, hopefully a dog or a cat, and, if not, sarcastically recommends that they get a pet rock.

Ultimately, our hope is that the user leaves the experience with more information about the other side (referring to cats for dog-lovers and vice versa) that allows them to set aside their qualms and become more accepting.

###  Chatbot Structure
While drafting our ideas down, we considered a few ways we could approach the user interactions the chatbot could accept. One take we looked into was just a traditional text-message structure where the user could input whatever they wanted and the chatbot AI would take that message and derive a meaning and proceed down its conversation flow accordingly.

We agreed that it would be an interesting concept, but would be challenging to implement since you would have to predict what the user inputs, and decided to not go further with that option. Next, we looked at just a static “YES” or “NO” button response. This approach is much simpler that the previous one, but we found it to be too simple. Our chatbot had too many conversation trees that could not fit a binary response such as yes or no, so we abandoned that idea as well.

The solution that we ended up implementing was a mixture of the other two structures with ideas from this innovative chatbot. We took inspiration from the traditional text idea by having the chatbot talk to the user with a simple text alert, but then use a button system, somewhat similar to the “YES/NO” section, that allows for unique responses, but limits it enough to make the conversation flow manageable.

###  Approach to the Conversation
When approaching the conversation the chatbot would carry out, we wanted to extend the creative and fun approach that our idea evoked into the conversation itself. While exploring other chatbots, we noticed that typically chatbot designers tend to make their bots conversate with a formal voice or a casual voice.

We gave our bot, accordingly, a very casual voice that gets a little funny at times through the use of pictures, memes, and word-usage. Even though our chatbot’s tone is a little unconventional, we believe that is does fit with our theme and the conversation does end up sounding natural when interacting with it. We also had the voice change depending on which flow the user ended up taking. Based on our survey, we found that dog-lovers tended to have a strong negative opinion on cats while cat-lovers tended to harbor little ill feeling for dogs. My team thought that it would be interesting to try to play off of this in the user-chatbot interaction and, as a result, telling the chatbot that you’re a cat-lover will result in a more tame conversation that if you said you were a dog-lover. In addition to the voice, we also made sure to account for anticipation (as mentioned in Adrian Zumbrunnen’s post on “Technical and social challenges of conversational design”) by adding in typing delays for each interaction with the bot, with longer messages taking longer to type, to make it seem more natural to the user.

###  Demos and Feedback
During demo day, we gained a lot of feedback, both positive and negative, for our chatbot. Both students and guest professor, Gillian Smith, loved the language and pictures the chatbot used. They felt that the bot’s conversation was very natural and authentic, and funny, with one student even saying talking to our robot felt like talking to one of his friends.

While we believe that we succeeded in our chatbot’s voice, we did receive constructive criticism on the complexity of the dialogue trees, user input, and how we displayed our messages. Specifically addressing our largest complaint, our use of buttons made some users feel like they were pushed too much to choose an option and did not encourage enough variation in the users’ responses. While this is a valid concern that we did debate during the planing stage of our design, I think we made the right choice because implementing less options forced users to take a side and such a push creates tension. Also, using an AI instead of buttons would be significantly harder to account for, especially in such a short amount of time.

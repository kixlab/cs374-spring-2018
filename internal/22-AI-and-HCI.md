# 22-AI and HCI


# Recap

# Admin



# UI HOFS
Clippy?

AI reasons + social reasons
clipped..
Cliff Nass
ignoring user studies

http://gizmodo.com/5632237/the-man-who-lied-to-his-laptop
 Every time a user typed "Dear . . . ," Clippy would dutifully propose, "I see you are writing a letter. Would you like some help?"-no matter how many times the user had rejected this offer in the past. Clippy would give unhelpful answers to questions, and when the user rephrased the question, Clippy would give the same unhelpful answers again. No matter how long users worked with Clippy, he never learned their names or preferences. Indeed, Clippy made it clear that he was not at all interested in getting to know them. If you think of Clippy as a person, of course he would evoke hatred and scorn.
http://blog.hoaloharobotics.com/2013/11/19/a-parting-salute-to-cliff-nass-social-interface-pioneer-and-good-friend

No persistent user profiles.
No reasoning about user competence, i.e., novice versus experienced user
Small event queue with emphasis only on the most recent interactions of the user with the software interface (this means the engine was trying to guess the values of many variables using very little data.)
Separation between user interface events and word-based queries; for word-based queries the engine ignored any context and user actions.
Last and possibly most important and I quote from the paper, “The automated facility of providing assistance based on the likelihood that a user may need assistance or on the expected utility of such autonomous action was not employed.” Instead, “The Office team has employed a relatively simple rule-based system on top of the Bayesian query analysis system to bring the agent to the foreground with a variety of tips.” This is why Clippy kept popping up all the time. It was not using the mathematically correct engine that the researchers had designed. It was driven by some rule-based system that one or more of the developers from the product team thought was a reasonable substitute.

The Office team subsequently replaced their Bob implementation for the Office Assistant with Microsoft Agent. Unfortunately they also failed understand how to apply the technology effectively, creating not a helper, but an annoyance that slowed users down rather than improved their use of applications. In addition, the limited quality and accuracy of speech technology meant that speech could not be relied on as a part of a successful interface. This and the stigma of Bob’s past failure and mediocre response to the equally poor implementation in the Office Assistant resulted reluctance by the Windows team to include Agent as a core UI element; and Agent too faded from the scene, though did end up being used in some very innovative interface projects and has given me a better design perspective on what I am doing now.
All this suggests that while social interfaces can be attractive, it takes much more work than designing a conventional user interface in that you had to consider more than basic human cognitive abilities in terms of how they can interact with devices and technologies. You have to understand how humans interact with each other, and that the nuances of the choice of a word, how it is said, or a facial expression when spoken give meaning to its understanding. It is one thing to come up with design guidelines for how to present information effectively on the screen, but quite another to script social interaction to feel natural.

https://www.theatlantic.com/technology/archive/2015/06/clippy-the-microsoft-office-assistant-is-the-patriarchys-fault/396653/

# Nanoquiz (4:13)


# Overview (4:16)

- meant to be a high level overview of some of the important topics of interest these days

the ultimate UI

- think and it's done. BCI?

Give an extreme UI example: "Best UI Ever"

- three buttons for Task 1, 2, 3 lol
- if you're a TA and a student team submitted this kind of UI, what feedback would you give?
	- lack of feedback, lack of transparency, limited user control, too much abstraction, limited customizability, etc.

# Principles

- reCAPTCHA version 2
- Amazon's ML-powered star rating
- GMail's Smart Compose: show a live demo from my GMail
	- Automatically suggests words and phrases to type. How is it different from auto complete (e.g., Google search, sublime command completion, etc.)

- GMail's Smart Reply: show a live demo from my GMail
	- contrast with clippy: discuss important dimensions
		- timing
		- cost of mistake
		- type of suggestions
		- delivery of suggestions (character vs. non-obtrusive at the bottom)
	
=> Discuss the usability of them.
Cost of failure? Recovery -- related to heuristic evalution.


## Control

- Adaptive, Adaptable, Mixed-Initiative
- Algorithm Aversion: people are being overly critical.
	- https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2466040
	- https://hrtrendinstitute.com/2017/02/13/algorithm-aversion-hr-trends-2017-5/
	- https://hbr.org/2015/02/heres-why-people-trust-human-judgment-over-algorithms
- Examples of Mixed-Initiative
	- Duet Draw (Changhoon Oh's CHI 2018 paper)
	- GVM (ECCV 2016): http://people.eecs.berkeley.edu/~junyanz/projects/gvm/
	- ShadowDraw?
	- Video demo of Google Photos automated album creation

# Activity: Usability Heuristics (4:39, 9 mins)

- Test Auto Draw from Google and come up with important usability heuristics that are specific to AI-powered UI.
- https://www.autodraw.com/
- Many students use one of the pre-existing criteria from Nielsen. Need a better instruction to encourage students to think broader.


# Video Break (skipped)

- Consider doing Google Duplex
	- Focus on usaiblity issues, both from the sender and receiver
	- Sender: trust on the system
	- Receive: deceived that it's the human on the other side. But why is it necessarily bad?
- https://www.youtube.com/watch?v=bd1mEm2Fy08
- http://bigthink.com/paul-ratner/is-it-ethical-for-ai-to-have-a-human-voice


# IUI Examples

- recommender systems
	- collaborative filtering (users like you...)
	- content based
	- context based
- explanation, transparency
- chatbots, conversational UIs
- intelligent search
- design considerations

- consider covering: IoT smart devices, self-driving cars


# Threats to Usability

- AI + Humans in a single system everywhere: transparency becomes an issue.

Cost of failure

- human as gorilla labeling
- human biases in the data
	- effect of English vs foreign names in job search
	- gender bias transferred to word embedding

- minor (lake vs river) to quite bad (important email as spam) to catastrophic (ethnicity, human as gorilla)
- recommendations (medical, mission critical, military -- civilian or enemy)


Food analogy: Filter bubble and radicalizing algorithms are junk food to our minds. Then what is the organic food algorithm? "AI free products"

https://www.fastcodesign.com/90172734/this-logo-is-like-an-organic-sticker-for-algorithms-that-arent-evil?utm_medium=social&utm_source=twitter.com


# Activity: Facebook Folk Theory (5:10)

- Students submitted interesting thoughts and ideas.
- Need a follow-up discussion to make sense out of the submitted ideas.

# Diff with Reading


# Post Class Notes
- reading: consider
	- https://design.google/library/ux-ai/
	- https://medium.com/google-design/human-centered-machine-learning-a770d10562cd
	- https://distill.pub/2017/aia/

- Video: https://www.youtube.com/watch?v=11UKXaELg8M
	- Eytan Adar: Stanford Seminar - Bounced Checks at the UI/AI Intersection

- Clippy: it's difficult for students to know how it exactly works so it's difficult for them to give feedback.

- for UI HOF, maybe just do the oracle UI. It led to many interesting thoughts: 

- Try to moral machine as activity

- Show Quick Draw: https://quickdraw.withgoogle.com/

Oracle

- understanding the user's true intent
- sensors, history, users like me, context, content, etc.
- query feature graph

Data

- A lot of modern machine learning requires lots of data
- Where does data come from? Users, crowds, etc.
- Users: privacy, control (GDPR), "selling" user data
- Crowds

Other topics to cover
- Privacy, data issues
- Disinformation, fake news
- Cambridge Analytica, Biases, FAT, harassment, trolling

Terry Winograd: Shifting Viewpoints
https://hci.stanford.edu/winograd/papers/ai-hci.pdf

Grudin: AI and HCI: Two Fields Divided by a Common Focus
https://pdfs.semanticscholar.org/e22b/e3642660d6a779e477124cae7cbfdfa5b0a5.pdf


# Not used

- Video: Uninvited Guests (concept video on the limitations and dehumanization of smart devices at home): https://vimeo.com/128873380

- Video: Amazon Go
https://www.youtube.com/watch?v=NrmMk1Myrxc

- Video: Microsoft Lumiere
https://www.youtube.com/watch?v=bt-JXQS0zYc

- perils: https://www.nytimes.com/2018/03/10/opinion/sunday/youtube-politics-radical.html

"Soon I noticed something peculiar. YouTube started to recommend and “autoplay” videos for me that featured white supremacist rants, Holocaust denials and other disturbing content."

"It seems as if you are never “hard core” enough for YouTube’s recommendation algorithm. It promotes, recommends and disseminates videos in a manner that appears to constantly up the stakes. Given its billion or so users, YouTube may be one of the most powerful radicalizing instruments of the 21st century."

"What keeps people glued to YouTube? Its algorithm seems to have concluded that people are drawn to content that is more extreme than what they started with — or to incendiary content in general."

"In effect, YouTube has created a restaurant that serves us increasingly sugary, fatty foods, loading up our plates as soon as we are finished with the last meal. Over time, our tastes adjust, and we seek even more sugary, fatty foods, which the restaurant dutifully provides. When confronted about this by the health department and concerned citizens, the restaurant managers reply that they are merely serving us what we want."

Reader comment 1: "If you imagine trying to group videos into a set of bins then you can see how you would probably put vegetarian videos in the same bin as vegan videos. Similarly far-right videos and other less extreme, but still right wing, videos would occupy the same or similar bins.

What I strongly suspect that you would then find is that if you want to try and define the bin, you would find that it ends up being defined by the most extreme content, because that content is furthest from the other bins. If you start watching videos that belong to one bin, the algorithm will then naturally tend to lead you towards other videos that best fit it's idea of the archetype of that bin, i.e. the most extreme ones.

There doesn't have to have been any decision on the part of YouTube/Google to favour extreme content because it leads to longer viewing times. Though if extreme content really does naturally lead to longer viewing times then any algorithm that also factors in viewing time will clearly also tend to favour extreme content. The problem might well be in part that although these algorithms are complicated they are still, compared to a human, quite simplistic in how they look at things."

Reader comment 2: "I think this article is really misguided and ultimately a call for censorship. Is there a lot of "extreme" or radical content on YT. Of course. There's all sorts of content. It's an open platform for anyone in the public to share their views. This means you're going to get a lot of perspectives outside the mainstream, partly because people with "radical" views are going to be more eager than others to tell the world about their views, and because such people generally do not get a platform in more traditional media. YT is where they go because it's open to them, while other media aren't. This is part of why so many people like YT: you get to see a wider range of content and perspectives than you'd see on TV or other media.

Also, the article treats "extreme" content as if it's some kind of poison that should be walled off from "non-extreme" content. YT is filled with all sorts of content, which means you're going to run into both "extreme" and otherwise if you're watching on autoplay. It also works the opposite way. I start watching an "extreme" video about a current news topic then pretty soon I'm watching a CNN segment on the same topic. This doesn't prove that YT is pushing "non-extreme" content. The content and recommends tend to be driven by what topics are covered (regardless of how "extremely") and what's popular with other viewers. It's largely user-driven, just like the content in the first place, as it should be."





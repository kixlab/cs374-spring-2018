# 19-Accessibility-Internationalization


# Recap
A lot of the discussion so far has been about understanding users' capabilities and limitations, and designing solutions that adapt to them. But we kind of assumed that all users have average and homogeneous human abilities. Today is about more extreme and diverse users.

# Admin



# UI HOFS
Parking signal

Use case

- "Can I park here now?"
- "For how long?"

Existing signs

- high information density
- hard to scan

Graphical design

- Layout: grid-style design, time table (familiar way to parse time-related information)
- Time-intensive parking: yellow?
- Arrow: what for?
- Squint test: green and red colors.
- But green and red are bad combinations. Hatches have been added, which did not exist in the original designer's version.
- Time intervals are not uniform. Interval variables for time. But they are focusing on common use cases.
- Parking options are nominal.


Learnability

- intuitive calendar view that's familiar to many
- more visual, no jargon or dense text

Efficiency

- single view

Safety

Evaluation

- How to evaluate a new thing like this?
- 100 installations + ramp up if successful
- This is a common strategy for web interfaces

Refs

- https://www.youtube.com/watch?v=90TqrVXLb_Q
- http://gizmodo.com/las-new-parking-signs-are-brilliant-and-every-city-shou-1695594041


# Nanoquiz (4:11)


# Accessibility (4:15)
- Accessibility is a universal problem
- Support alternative input (e.g., keyboards)
- Support alternative output (e.g., screen readers)

- Types of assistive technology

- Best practices for web accessibility

## Activity: Explore assistive technology (4:20)
5 mins

- sip & puff: talk about design dimensions for precision of the interface, e.g., length of sipping and puffing, direction (sip or puff), strength. 

- tongue interface: fun example to talk about. 9 areas are reasonable. 16? 25?

# Video Break

https://www.youtube.com/watch?v=TiP7aantnvE

Show how blind people use digital devices in their real life.
Play from 1:48 - 3:20

(optional): https://www.youtube.com/watch?v=UzffnbBex6c

Vizwiz
https://www.youtube.com/watch?v=solWTf_KDXI

Vislens
https://www.youtube.com/watch?v=Wy0656j2eig

# Internationalization

## Internalization factors 
3 mins
- brainstorm as class, write down on the board

### Differences among locales
- Culture
- Symbols
- Color
- Left->Right
- Formatting of number, date, currency
- Photos

- high quality translation can be tricky
    - requires native speakers in both languages, plus a bilingual who does the translation, if you outsource.


## Activity: Internalization (4:38)
3 + 10 mins

3 min walk-through of the task: this exercise needs some pre-explanation. walking through the title example was useful.



## People's system usage can be affected. 

- The way people use Twitter between Korean and English users is quite different.
- Much more content can be entered in 140 Korean characters. People use Twitter almost as a short blog post sometimes, whereas in English it's mostly links and very brief comments.


## Other Factors to Consider 

- ActiveX in Korea: IE + Windows
- Browser usage stats


## Activity: Cultural Comparison (5:02)
20-25 mins

- no time for step 2: could be shared after class for student's analysis or even next class.

### Hofstede's cultural dimensions theory
- Let's try to conduct our own experiment looking at cultural differences.

- Hofstede's cultural dimensions theory is a framework for cross-cultural communication, developed by Geert Hofstede. It describes the effects of a society's culture on the values of its members, and how these values relate to behavior, using a structure derived from factor analysis.

- Power distance index (PDI): "Power distance is the extent to which the less powerful members of organizations and institutions (like the family) accept and expect that power is distributed unequally." Individuals in a society that exhibit a high degree of power distance accept hierarchies in which everyone has a place without the need for justification. Societies with low power distance seek to have equal distribution of power. [6]Cultures that endorse low power distance expect and accept power relations that are more consultative or democratic.
- Individualism (IDV) vs. collectivism: "The degree to which individuals are integrated into groups". In individualistic societies, the stress is put on personal achievements and individual rights. People are expected to stand up for themselves and their immediate family, and to choose their own affiliations. In contrast, in collectivist societies, individuals act predominantly as members of a lifelong and cohesive group or organization (note: "The word collectivism in this sense has no political meaning: it refers to the group, not to the state"). People have large extended families, which are used as a protection in exchange for unquestioning loyalty.
- Uncertainty avoidance index (UAI): "a society's tolerance for uncertainty and ambiguity". It reflects the extent to which members of a society attempt to cope with anxiety by minimizing uncertainty. People in cultures with high uncertainty avoidance tend to be more emotional. They try to minimize the occurrence of unknown and unusual circumstances and to proceed with careful changes step by step planning and by implementing rules, laws and regulations. In contrast, low uncertainty avoidance cultures accept and feel comfortable in unstructured situations or changeable environments and try to have as few rules as possible. People in these cultures tend to be more pragmatic, they are more tolerant of change.
- Masculinity (MAS), vs. femininity: "The distribution of emotional roles between the genders". Masculine cultures' values are competitiveness, assertiveness, materialism, ambition and power, whereas feminine cultures place more value on relationships and quality of life. In masculine cultures, the differences between gender roles are more dramatic and less fluid than in feminine cultures where men and women have the same values emphasizing modesty and caring. As a result of the taboo on sexuality in many cultures, particularly masculine ones, and because of the obvious gender generalizations implied by Hofstede's terminology, this dimension is often renamed by users of Hofstede's work, e.g. to Quantity of Life vs. Quality of Life.


- Power distance index shows very high scores for Latin and Asian countries, African areas and the Arab world. On the other hand Anglo and Germanic countries have a lower power distance (only 11 for Austria and 18 for Denmark). For example, the United States has a 40 on the cultural scale of Hofstede's analysis. Compared to Guatemala where the power distance is very high (95) and Israel where it is very low (13), the United States is in the middle. In Europe, power distance tends to be lower in northern countries and higher in southern and eastern parts: for example, 68 in Poland and 57 for Spain vs. 31 for Sweden and 35 for the United Kingdom.
- Regarding the individualism index, there is a clear gap between developed and Western countries on one hand, and less developed and eastern countries on the other. North America and Europe can be considered as individualistic with relatively high scores: for example, 80 for Canada and Hungary. In contrast, Asia, Africa and Latin America have strongly collectivist values: Colombia scores only 13 points on the IDV scale and Indonesia 14. The greatest contrast can be drawn comparing two extreme countries on this dimension: 6 points for Guatemala vs. 91 points for the United States. Japan and the Arab world have middle values on this dimension.
- Uncertainty avoidance scores are the highest in Latin American countries, Southern and Eastern Europe countries including German speaking countries, and Japan. They are lower for Anglo, Nordic, and Chinese culture countries. However few countries have very low UAI. For example, Germany has a high UAI (65) and Belgium even more (94) compared to Sweden (29) or Denmark (23) despite their geographic proximity.
- Masculinity is extremely low in Nordic countries: Norway scores 8 and Sweden only 5. In contrast, Masculinity is very high in Japan (95), and in European countries like Hungary, Austria and Switzerland influenced by German culture. In the Anglo world, masculinity scores are relatively high with 66 for the United Kingdom for example. Latin countries present contrasting scores: for example Venezuela has a 73 point score whereas Chile's is only 28.

- http://en.wikipedia.org/wiki/Hofstede%27s_cultural_dimensions_theory


### Part 1. Explore. (8 mins)


### Part 2. Synthesize. (5 mins) skipped

- after class, do some analysis. e.g., "Analyzed" sheet in https://docs.google.com/spreadsheets/d/1U7F5Y0fg3O5WKW0_TK_T3XAZjUEqonVvdUc09yFBL7A/edit#gid=220833591
- try to show some meaningful differences on some dimensions. e.g., Malaysis vs Austria (power distance) in num of faculty or students in photos, num of men or women in photos.

### Part 3. Compare. (5 mins) 5:10, 3 mins, 5 mins desired.

- but be aware that students lose access to their results upon submitting stage 1 results.]

### Discussion in class (3 mins)
Any interesting observations?


Implications of internationalization

- more and more ways to have worldwide population use and test your interface
- making it less WEIRD (Western, Educated, Industrialized, Rich, and Democratic)



# Diff with Reading
Accessibility

- removed dyslexia
- removed aDesigner

Internationalization

- sort order
- color convention
- formatting libraries


# Post Class Notes

Dyslexia?

Short on time: barely finished part 1 of the exercise

Coding i18n exercise worked quite well


## Postmortem Notes

- Students made good observations about some university websites maintaining multiple layouts for different locales. The Univ. of Tokyo, for instance, has completely different layouts and content organization for their English and Japanese websites.
- A student mentioned that forms.py fails to load due to security issues in beta versions of Chrome.
- In the Javascript i18n exercise, some strings are not translated to French: "date", "price".
- In the Javascript i18n exercise, a student mentioned that currency formation should be applied the current exchange rate :)
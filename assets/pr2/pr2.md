**Due: 11:59pm on 4/5 (Thu)**
**40 points (4% of your total grade)**
 -- 160 points will be scaled to 40 points

## Intro
In the last assignment, we built a layout of the capital quiz game. For PR2, we will implement interactive features of our game using JavaScript based on the layout you built.


## Where to start from?
We provide you with the starter kit, [pr2.zip](assets/pr2/pr2.zip). It includes
- `jquery/`: the code for jQuery and jQuery UI, the JavaScript libraries you will be using for this assignment.
- `country_capital_pairs.js`: an array of JavaScript objects that contains a pair of country and its capital.
- `capital_game.css`: a skeleton file for your user interface CSS code.
- `capital_game.js`: a skeleton file for your user interface JS code.
- `index.html`: a skeleton file for your user interface HTML code.

## How to submit?
- Compress your code into `studentnumber_pr2.zip`. Please do not create any subfolders.
- Then upload the zip file to [this link](https://www.dropbox.com/request/S4WNIxwoQhKkRNlA27ck) until the due date stated above.
- [Late policy](logistics.html#grading) will be applied.

## How to test my code before submitting it?
- TAs will evaluate your code on the latest stable version(65) of Chrome for OSX. We expect no browser compatibility issue in this assignment (we're not making a cutting-edge web application), but please test your code in your platform's Chrome before submission.
- If there is a browser issue between Chrome versions in different OS, TAs will follow the behavior in the student’s OS. However, please make sure that you are not using any custom stylesheet in your Chrome.
- There were many questions about using the latest features of JavaScript / CSS in programming assignments. It’s okay to use those cool features if they are supported by Chrome 65. If you are not sure about the support status of the feature you wish to use, check [http://caniuse.com/](http://caniuse.com).

## Where to ask questions?
- If you have questions about this assignment, please post it on our Piazza (in *pr2* folder as *question*). TA will answer within a day.
- If you believe your question should be kept private, please send email to [hyeungshik.jung@kaist.ac.kr](mailto:hyeungshik.jung@kaist.ac.kr). TA may share the question with other students.

## OK, what should I do?
Your job is to implement basic functionalities of the capital quiz game - Choosing a new question, checking whether the user’s answer is correct, showing history, etc.

### Step 1: Prepare a new question (45pt)
![](assets/pr2/step1.gif)
In the previous programming assignment, we placed an example question and an example correct/wrong entry. In this step, you have to display a new question every time (1) when the page is loaded, or (2) the user clicks the ‘See Answer’ button. In detail,

#### (15pt) Adding id to elements
- (5pt) The `td` containing the question(the country's name) should have an `id` of "pr2__question" (Note that there are two underscores).
- (5pt) The `input` for typing answer should have an `id` of "pr2__answer".
- (5pt) The button for submitting answer should have an `id` of "pr2__submit".
#### (5pt) Empty history
There should be no example entries when the page is refreshed.
#### (10pt) Random first question
Every time the page is loaded, the initial question should be randomly selected.
The input element for typing answer should get focus so the user can start typing as soon as the page is loaded.
#### (15pt) Behaviour of the ‘See Answer’ button
When the ‘See Answer’ button is clicked,
- (5pt) A new, randomly selected question should be prompted.
- (5pt) The input should be cleared.
- (5pt) The input should get focus again.

### Step 2: Maintain the history of previous questions (40pt)
![](assets/pr2/step2.gif)
Update your code so that when the user presses the ‘See Answer’ button, the list of previous answers gets populated with each of the user's entries. In detail,

#### (10pt) Pile up previous questions and answers
- The entry that was submitted last appears at the top of the list.
#### (15pt) Style a correct entry
- When deciding whether an entry is correct, the program only performs exact matches: differences in capitalization, blanks, etc. should be reported as incorrect answer.
- The color of the correct entry should be blue.
- There should be a check icon at the Answer column of a correct entry.
#### (15pt) Style an incorrect entry
- The color of the correct entry should be red.
- Strikethrough the user’s wrong answer.

### Step 3: Add autocomplete in answer input (35pt)
![](assets/pr2/step3.gif)
The input field accepts the user's guess. Use jQuery UI to make this field an [autocomplete widget](https://jqueryui.com/autocomplete/#folding). In detail,

#### (15pt) Start of autocomplete
- (10pt) It should suggest the capitals in the `country_capital_pairs.js` that contain letters that the user has typed so far.
- (5pt) The autocomplete widget should pop up when the user enters **at least two** characters.
#### (20pt) Selecting behaviors
When the user selects a suggestion from the autocomplete widget by clicking or hitting the ‘Enter’ key, it should behave the same as clicking on the ‘See Answer’ button. In detail,
- (5pt) A new, randomly selected question should be prompted.
- (5pt) The `input` should be cleared.
- (5pt) The `input` should get focus again.
- (5pt) Add the entry to the previous entry list.
- You don't have to handle an Enter-key event when no suggestion is selected.

### Step 4: Add filtering and deletion of past entries (60pt)
![](assets/pr2/step4.gif)
How about showing correct or wrong past entries only? Let’s add a filter for past entries. In detail,

#### (20pt) Add option elements for filter selection
- (5pt) Add 3 input elements: ‘All’ , ‘Correct’, and ‘Wrong Only’. Their type should be radio.
- (5pt) They should be placed in a row.
- (5pt) They should be placed below the row with question and input.
- (5pt) The default option is ‘All’.
#### (25pt) Filter selection behavior
- (15pt) When the user selects an option, the history should be updated accordingly (For the ‘All’ option, every past entry should be displayed. For the ‘correct’ option, every correct past entry should be displayed).
- (10pt) What if the user submits a correct answer when ‘Wrong Only’ is selected, or vice versa? In this case, change the filter to ‘All’ automatically so the user receives correct feedback.
#### (15pt) Support deletion of a past entry
- (5pt) Add a delete button to the ‘Answer’ column of past entries.
- (10pt) When the button is clicked, the row that contains the clicked button is deleted. After deletion, it should not be seen even if the user selects a new filter.

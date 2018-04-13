**Due: 11:59pm on 5/3 (Thu)**
**50 points (5% of your total grade)**
 -- 210 points will be scaled to 50 points

## Intro
In the last assignment, our capital game had a few interactive features like autocomplete, grading, and filtering. In this assignment, we will make our capital game communicate with the web, as well as make it safer from errors.

## Where to start from?
We provide you with the starter kit, [pr3.zip](assets/pr3/pr3.zip). It includes
- `jquery/`: the code for jQuery and jQuery UI, the JavaScript libraries you will be using for this assignment.
- `capital_game.css`: a skeleton file for your user interface CSS code.
- `capital_game.js`: a skeleton file for your user interface JS code.
- `index.html`: a skeleton file for your user interface HTML code.

## How to submit?
- Compress your code into `studentnumber_pr3.zip`. Please do not create any subfolders.
- Then upload the zip file to [this link]() until the due date stated above.
- [Late policy](logistics.html#grading) will be applied.

## How to test my code before submitting it?
- TAs will evaluate your code on the latest stable version(65) of Chrome for OSX. We expect no browser compatibility issue in this assignment (we're not making a cutting-edge web application), but please test your code in your platform's Chrome before submission.
- If there is a browser issue between Chrome versions in different OS, TAs will follow the behavior in the student’s OS. However, please make sure that you are not using any custom stylesheet in your Chrome.
- There were many questions about using the latest features of JavaScript / CSS in programming assignments. It’s okay to use those cool features if they are supported by Chrome 65. If you are not sure about the support status of the feature you wish to use, check [http://caniuse.com/](http://caniuse.com).

## Where to ask questions?
- If you have questions about this assignment, please post it on our Piazza (in *pr3* folder as *question*). TA will answer within a day.
- If you believe your question should be kept private, please send email to [hyeungshik.jung@kaist.ac.kr](mailto:hyeungshik.jung@kaist.ac.kr). TA may share the question with other students.

## OK, what should I do?

### Step 1: Load country and capital data from the web (30pt)
In the last assignment, the list of countries and their capitals was provided in `country_capital_pairs.js`, a JavaScript file which stored the list in a pairs variable. In this assignment, let's load the list from the csv file on the web. In other words, instead of loading from a file, load it from the web.
- Retrieve the csv file from the [link](https://s3.ap-northeast-2.amazonaws.com/cs374-csv/country_capital_pairs.csv) by making a request (e.g., by using [jQuery.ajax](http://api.jquery.com/jquery.ajax/) or [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)) and you should get a response.
- Parse the response and save the parsed data to the `window.pairs` variable. The result should be in the same format as the pairs variable from the last assignment - a JavaScript array with objects including two keys ("country" and "capital").
- TAs will evaluate the parsed result by inspecting the `window.pairs` variable in the browser console.
![](assets/pr3/check_parsed.gif)

### Step 2: Store history using Firebase (50pt)
Build every component of PR2 - autocomplete, grading, filter, etc. However, for this time, store past entries to Firebase so they are not lost even when the user refreshes the webpage.
- (40pt) Please follow **every** specification of PR2 for implementation, including elements' `id`s like **pr2__submit**.
- (10pt) Add a **Clear** button on the row below option elements. Set its `id` to **pr3__clear**. When the ‘clear’ button is clicked, all the past entries are deleted.
![](assets/pr3/show_clear.gif)

### Step 3: Show the location of countries (50pt)
How about adding a map showing the location of countries?
* (10pt) Add a map above the table using [Google Maps Embed API](https://developers.google.com/maps/documentation/embed/guide). Please read instructions and acquire your API key.
* (5pt) Set the `width` to **500px** and `height` to **400px**.
* (5pt) Set the `maptype` to **satellite** by referring to the [Devloper Guide](https://developers.google.com/maps/documentation/embed/guide).
* (10pt) Show the location of the country in the current question using the `q` parameter in the `iframe`'s `src`. If the game is asking the capital of *Easter Island*, include `q=Easter Island` in the `src`.
* (10pt) When the user clicks on any country name in past entries or the question, update the map accordingly.
* (10pt) When the user hovers on any country name, change the style of mouse `cursor` to **pointer** to provide clicking affordance.
![](assets/pr3/update_map.gif)

### Step 4: Add Undo (80pt)
Let's add the Undo feature to provide better [Safety](https://kixlab.org/courses/hci/classes/06-Safety/) in our capital game.


#### Undo (40pt)
- (20pt) Add an Undo button that, each time it is pressed, goes one step backwards in history. For example, if the user clicks Undo after entering an answer, the answer should be deleted.
- (10pt) The Undo button should have an `id` of **pr3__undo**.
- (10pt) The Undo button should only be enabled when that action is possible. For example, Undo should be disabled when you start the game. Use the `disabled` attribute to disable a button.
- The Undo button can also undo the ‘clear’ action.

#### Managing Undo History (40pt)
- (20pt) The history for Undo feature should be stored in the Firebase database, and they should be remaining after the page is refreshed.
- (20pt) Add a Reset button that clears all the past entries and undo history. The Reset button should have an `id` of **pr3__reset**.
- Reset cannot be reverted, and undo should be disabled after reset.
![](assets/pr3/undo_example.gif)
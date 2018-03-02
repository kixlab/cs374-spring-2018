**Due: 11:59pm on 3/16 (Thu)**
**40 points (4% of your total grade)**
 -- 160 points will be scaled to 40 points

## Intro
How many capitals of countries do you know? Throughout three programming assignments, we will build a simple quiz game with various countries and their capitals. For PR1, we will design a layout of the game using HTML / CSS.

## Where to start from?
We provide you with the starter kit, pr1.zip. It includes
- `capital_game.css`: a skeleton stylesheet for your CSS code.
- `index.html`: a skeleton HTML file for your HTML elements. capital_game.css above is included.

## How to submit?
- Compress your code into `studentnumber_pr1.zip`. Please do not create any subfolders.
- Then upload the zip file to the course KLMS until the due date stated above.
- Late policy in course webpage will be applied.

## How to test my code before submitting it?
- TAs will evaluate your code using the latest Chrome for OSX. We expect no browser compatibility issue in this assignment (we're not making a cutting-edge web application), but please test your code in your platform's Chrome before submission.
- If there is a browser issue between Chrome versions in different platforms, TAs will follow the behavior in the student’s platform. However, please make sure that you are not using any custom stylesheet in your Chrome.

## Where to ask question?
- If you have questions about this assignment, please post it on our Piazza (in ‘pr1’ folder as ‘question’). TA will answer within a day.
- If you believe your question should be kept private, please send email to hyeungshik.jung@kaist.ac.kr

## OK, what should I do?
Your job is to build a layout of the capital quiz app based on the starter kit. Please note that we don’t implement any interactive features(input, checking answers, etc.) in this programming assignment. Points assigned to each task will be normalized for total 40 points in the final grade.


### STEP1: Add basic components (60pt)
![](assets/pr1/step1.png)

You have to add a **title**(1) and a **table**(2) first. In detail,
#### (10pt) Title
* Your title’s font-size should be bigger than other texts below. 

#### (10pt) Shape of table
* The table should have 3 columns. 

####(10pt) Table header
* Each of the 3 columns has its own header, named ‘Country’, ‘Capital’, and ‘Answer’, respectively.

#### (10pt) Row for entering answer
* The second row (the row below the header) should contain the example country, the text input, and the ‘See Answer’ button.

#### (10pt) Row for correct past entry
* The third row should contain a correct entry example. Since Tokyo is the capital of Japan, we display ‘CORRECT’ in the answer column.

#### (10pt) Row for incorrect past entry
* The fourth row should contain an incorrect entry example. Since New York is not the capital of the USA, we display the correct answer (Washington, D.C.) in the answer column.


### STEP2: Styling components-1 (50pt)
![](assets/pr1/step2.png)
Let’s give some style to components so their functions are easily recognizable. In detail,

#### (10pt) Header
* Make text in the table header bolder than other texts in table’s body.

#### (10pt) Correct past entry
* (5pt) Change the font-color of correct entry into blue.
* (5pt) Change ‘CORRECT’ in answer column to a check icon. You can easily insert icons by using libraries like FontAwesome, without inserting images. FontAwesome is included in index.html. Check this link to learn how to use it.
* (10pt) Incorrect past entry
* (5pt) Change the font-color of an incorrect entry into red.
* (5pt) Strikethrough the wrong answer (New York in the example).
* (20pt) Alignment
All elements in a column should be left aligned.
The title and the first column should be left aligned.


### STEP3: Styling components-2 (50pt)
![](assets/pr1/step3.png)
#### (10pt) Use web fonts for the title.
* With web fonts, you can load any type of font into your web page.
* Google Fonts is one of the most popular services. If you are new to it, this tutorial and article will be helpful.

#### (10pt) Align elements to the center.
* Currently our elements are at the left of the page - let’s move them to the center as shown in the screenshot above.
* It’s okay to wrap the content in a fixed width div. However, make sure that the title is displayed in one line (no line break).
* Aligning content to the center is a deep topic indeed. Here are some recommended articles from course staff.
	* The complete guide to centering a div
	* CENTERING THINGS

#### (30pt) Apply styles to the table
![](assets/pr1/step4.png)
Let’s make our table look more like a table.
* (15pt) Add horizontal borders
	* (5pt) No border for the uppermost border (above the header).
	* (5pt) Style is up to you, but there shouldn’t be any vertical borders between borders.
	* (5pt) The borders should not be separated(You will find a CSS property called border-collapse(link) useful).
* (10pt) Add paddings
	* Add 5px of padding to every cell in the table.
* (5pt) Apply different styles to the border below the header and other borders.
	* In the example above, the border below the header is set to `1px solid black`, while other borders are `1px solid #cccccc`
	* You may apply different border-style of your own. Please show your aesthetic sense.

# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Sadia Chowdhury

Time spent: 4 hours spent in total

Link to project: (insert your link here, should start with https://glitch.com...)

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons

The following **additional** features are implemented:

- Added a background image
- Used padding and margin to properly fit the buttons
- Added a new function in js to resume audio, had to debug a lot as to why the sounds were not playing, but after I added that function it works now

## Video Walkthrough

Here's a walkthrough of implemented user stories:
http://g.recordit.co/PwTKqZkYmV.gif


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
I used W3Schools.com for css instrcutions, HTML-Color.code for different colors that I wanted, and Google Chrome Audio function from google  

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
A challenge that I encountered was the sound not playing in my project. It worked for few minutes and then somehow, it broke and did not
play the sound frequency at all. For example, I would press my colored buttons and I could see the buttons lighting up, however,
would not hear any sound. At first I thought it was just glitch being glitchy. So, I did a lot of research on how to fix this issue. 
A lot of resources suggested to try different browsers to see if it is not a google chrome thing. So, I ran my code in safari, still
was running into the same problem! Afterwards, I went to the inspect portion of the code. There I found some yellow warnings, 
"The AudioContext was not allowed to start. It must be resumed (or created) after a user gesture on the page. https://goo.gl/7K7WLu". This is 
the link that google inspect guided me towards. There I found out various options to fix this issue. I decided to use
a function that they provided in the documentation and I added that function in my javascript file. So, the piece 
of code is basically calling the resume function since we created AudioContext on page load. The resume function is called
whenever the player or the user interacts with the game. After adding that piece of code in the project, the sound problem was fixed!
 

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
Working on this project was super fun!! I have few questions about web development after creating this project. 
First, are there any other languages to create websites, besides html, css and javascript. What are some tips to become an 
effective web developer? What are some differences of becoming a web developer and a software engineer? Can a person be both 
web developer and a software engineer? After doing this project, what I think of html is that it is the skeleton of the 
website so basically it holds all the writings and structure. Then, CSS is like the "clothes" of the skeleton(html) to 
make the website look pretty and professional. Lastly, javascript is basically to make things function and interact more with the user. 
So, my next question would be is there any other language that does everything at once. Like a combined version of HTML, CSS and Javascript?


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had few more hours to work on this project, I would try to add another page, where it would say "GAME OVER" in 
big red text instead of a small alert saying that the fame is over. I would also try to make my game more complex. For example, 
speed up the pattern when the user successfully guesses a pattern. I would also add a level button where after every 5th 
successful guesses the level will go up. Also, add a lives button where it will start off as 3. Every time the user guesses 
something incorrectly, they lose a live. When there is no more lives left, that is when the game stops and says "GAME OVER".



## License

    Copyright SADIA CHOWDHURY

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Jeevan Bastola**

Time spent: **10** hours spent in total

Link to project: (https://glitch.com/edit/#!/holly-lead-unicorn?path=index.html%3A1%3A0)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Game button appearance change goes beyond color (e.g. add an image)

## Video Walkthrough

Here's a walkthrough of implemented user stories:
<img src='http://g.recordit.co/AGLxCD2BWY.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

Random pattern is created every new game:

<img src='http://g.recordit.co/eCk7htQqrs.gif' title='Video Walkthrough_2' width='' alt='Video Walkthrough' />



## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

- The outside resources I used to complete this project are stackoverflow.com and w3schools.com. I used stackoverflow.com to solve the sound issues that google chrome was 
causing and find way to make images fit on the buttons. Similiarly, I used w3schools.com to find resources to improve the design of the game. 

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

- One of the challenges I faced while creating this game was a sound error. Everytime I reopened the game, the buttons would work fine but there was no sound. 
To understand what was causing this error I opened the console using developer tools on chrome. There was an error saying "The AudioContext was not allowed to start. 
It must be resumed (or created) after a user gesture on the page.". I had no idea what the error meant so I went to stackoverflow.com to see if other people were facing 
the same problem and turns out this error was caused because of a recent update on google chrome. To fix this problem I set up a function on script.js that would tell the
browser to resume the sound context of the game as soon as the user clicks on the game. Here is the function: function touchStarted() { AudioContext().resume(); }


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
- One of the questions I have about web development is what the future of web-developemnt is going to look like as sectors such as Artificial
Intelligence, Virtual reality, Machine learning are growing rapidly. It is inevitable that these sectors are going to be a big part of web development
and some companies like Amazon are already using machine learning to increase their business. Combination of virtual reality and web development also holds a 
great future. As companies like squarespace.com have gained popularity it has become possible for anyone to develop websites which makes me wonder how web development 
businesses and web-developers are adjusting to this change.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
- If i had a few more hours to work on the project I would make the game more interactable. Most game give the user pop-up messages to let them know what is going on with the game and 
what their next step should be. I would add pop-up notifications updating the user about
the number of mistakes they have remaining before they lose the game. Similiarly, I would also program the buttons to play parts of a song rather than random tones.
I would also add an option that lets user decide the number of buttons they want on the game.


## License

    Copyright [Jeevan Bastola]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

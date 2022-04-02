# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Noor Earpy**

Time spent: **12** hours spent in total

Link to project: https://light-sound-memory-noor-earpy.glitch.me

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
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [X] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

![] (https://cdn.glitch.global/0eb8867a-1907-436a-a49e-770bec8a36aa/1.gif?v=1648796579895)


## Reflection Questions

1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

W3schools
MDN Web Docs
Stack Overflow
Google Fonts

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

The most difficult task I faced was creating a count-down timer using setInterval and clearInterval. These two functions were unknown to me, so I had to look them up on MDN Web Docs to see how they worked. To learn how to set up a countdown clock, I looked at numerous examples on W3Schools and Stackoverflow. The countDown function's design is one of the task's challenges. To calculate the time difference, I used Date().getTime() as an example from W3Schools. However, I quickly discovered that this was unnecessary because setInterval was already keeping track of the time for me. As a result, I utilized a count variable to keep track of how many times countDown() is used and to ensure that the countDown method, which is set to run every 1000 milliseconds, gets called exactly 20 times. The most challenging element is determining where setInterval and clearInterval should be placed in a complex logic circuit. In other circumstances, despite using clearInterval, I was unable to stop the countDown() method and ended up in an infinite loop (). I tried to debug by using console.log() to set breakpoints and discovered that my clearInterval() was called appropriately. I also looked for solutions on a number of different forums. And eventually, one option proves to be successful! I was able to correctly stop the countDown() by adding an extra clearInterval() before using setInterval(). I found the reason of the error was that I was running numerous setInterval() and countDown() functions at the same time when I adjusted guess() and stopGame() to reset countDown() and start again at a fresh guessing turn. I went through a torturous debugging session, but I also learnt how to call and use functions in a web project.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

It was fascinating to see how we might make an entertaining online application that runs on the user's computer. I'm intrigued to see how far we can take this. I recently created a Python web-scraper that produces statistics about a YouTube channel given the URL. Could I create this web-scraper with Javascript and make it run on the user's end, assuming we simply want to present the output without saving it in a database? Of course, this is contingent on Javascript's capabilities, and I'm eager to see how powerful it is. I also liked that I started with a simple HTML/CSS look and then utilized Javascript to fulfill the functionality. After I got all of the features, I began experimenting with color palettes, Bootstrap containers, positioning, and alignment, among other things. It was similar to putting together LEGO and experimenting with different combinations. I'd like to learn more about quickly designing elegant and user-friendly UI and UX. In addition, I'd like to see how I can apply my Adobe Illustrator talents to it. Some applications I've heard of allow you to create the website's UI first and then get the HMLT/CSS code. I'm interested in seeing how the coding and the design interact in such programs.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

I'd like to improve the game's functionality and reorganize the website layout to make it more appealing. I'd like the title and start/stop buttons to be in the center. I'd like to add difficulty levels and allow users to select them. A pattern in a simple game, for example, consists of six pieces. A pattern can have 10-15 parts in a difficult game. Alternatively, users can freely choose the amount of elements in the pattern. To accomplish so, I'll need to add a user input box, either a dropdown list or a text field, and enable the generatePattern() function to take user inputs and generate patterns based on the requests of the users. I also want to use React to restructure the code into distinct components to make it easier to manage.

## Interview Recording URL Link

[My 5-minute Interview Recording](https://baruchmailcuny-my.sharepoint.com/:v:/g/personal/noor_earpy_baruchmail_cuny_edu/EQ54i61Yzr1LvDFJuzkG7zsBuSKuTqgxU_uBGFi6Hx2E7g?e=tiTlYN)


## License

    Copyright [Noor Earpy]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
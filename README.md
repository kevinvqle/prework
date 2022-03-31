# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Kevin Le**

Time spent: **7** hours spent in total

Link to project: https://kindhearted-first-trapezoid.glitch.me/

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
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [x] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!
- added a score function and max score function 

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
-https://github.com/kevinvqle/prework/blob/main/ezgif-5-224f494716.gif

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
- GeeksForGeeks: to understand javascript,css, and html syntax
- Mozilla : understand getElementById
- HTML and CSS cheat sheets: quick and easy way to access css and html functionalities in a organized fasion

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

The main challenge with this project was fixing bugs that would occur during the process of the game. The first bug that occurred was when the player would click the button before the sound ended, this would cause the player to lose. In order to fix this issue, I had to research methods that would allow the player to increase the speed of the user's input in order to clear this error. A challenge that occurred during this project was creating a timer and a way to keep track of the points that the player has accumulated throughout the game. The first approach to building a timer method was looking at resources online like StackOverflow of people's previous attempts of making a timer and implementing that. First, what I did was set the timer at 10 and have the update timer function be called when the game starts. I used the getElementId to display it during the game and used the setTimeout function which is a global method that executes the timer function that I created once the timer expired. Within my playClueSequence, I created a condition, if the game is still playing, the timer would count down within a certain increment. This method worked well since the player can physically see the timer going down in real-time and as the player loses, the clear timer function would reset the timer and it would go back to 10 when the player wants to restart the game. Using the stack overflow, I was able to debug the issues of the timer not being able to show up due to not using the innerHTML method and using my id called in my HTML file (paragraph2) and being able to use it in my getElementId object. After completing this timer method for this project, I was able to move on and create my point system in order to keep track of my current points and the highest point the user has accumulated before refreshing the webpage. An issue that I had I faced was implementing the point method. When implementing this function, many times when clicking the right square wouldn't update the score. After researching on the web such as stackoverflow, I was able to implement a simular way to keep track of the point and highest point possible. In order to do this, I had to deal with a lot of conditions. To figure out my highest score, I had to compare it to my current score and if it was greater, I would call my update paragraph function. To increase the point every time the player got it right, I would have to use more conditionals such as progress == patternlength, the progress would increment and the current score would increase as well. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

- How do you make your code more scalable when considering different platform this web game can be played on such as an ipad, phone, or a tablet?
- What is the job prospect when it comes to web development? 
- What other ways besides projects can I get better at web development? 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

-If I had more time to finish the project, I would make my coder more neater and put more effort into implmenting more function to make the game more interactive. If I could, I would of implmented a way to have the user be able to chose a difficulty of the pattern such as easy, medium and hard. This function could be implemented by adding buttons and changing the given source code for the pattern. The main use of this function would be as the difficulty gets harder, the faster the pattern goes and it makes the game more challenging for the user. Another function I would like to implement would be the option to have color schemes such as being able to chose different colors of the boxes and customize packs to share with other people. This function is more harder to implement, but my initial thoughts would be having a save options when it comes to desinging the pattern colors. 



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright [Kevin Le]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
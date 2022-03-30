# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Folasade Oloye

Time spent: 8 hours spent in total

Link to project: (https://glitch.com/edit/#!/sound-and-light-memory-game---codepath-prework)

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
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] Create difficulty levels
- [ ] User is able to create their own pattern
- [ ] Mobile device playablity

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://recordit.co/hAGd5OGIpv)
![](https://recordit.co/AUXCbQpUwY)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

https://www.w3schools.com/css//css_font_websafe.asp
https://www.bestcssbuttongenerator.com/
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random
https://www.w3schools.com/cssref/css_colors.asp
https://www.w3schools.com/css/css_align.asp

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

The biggest challenge I encountered while creating this submission was implementing the guess function. After I had implemented the guess function to the best of my ability, I had double checked with the given solution to see if I was in proper shape. Most of my logic had matched the solution, and after implementing this function the game should have been fully playable. However, my game was still very buggy and would tell the user that they had played the incorrect note even when they had pressed the correct one. In order to figure out where in my code the problem was, I used the console.log() function to debug and see there was a problem with my variables not updating properly. After running the game a couple times through and looking at what was being output to the console, I noticed that my guessCounter variable was not updating correctly, causing the program to look at the wrong value in the pattern array. At first I was completely lost on how to fix this bug. I then took a step away from the computer for a bit, as I know getting too into the code can sometimes be detrimental. After taking a break from implementing this function, I then came back to it and looked at where guessCounter should be resetting, which was inside of the playClueSequence function. Although it resets it to 0 in the function, I added another line before playClueSequence is called in the guess function that set it equal to 0 to make sure that my value was truly being set to the correct value. After implementing that line, my game began to work and fixing this bug made me feel very accomplished and working through it was so rewarding.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

A large question about web development I have after creating my submission is how are web pages that are compatible on both computers and mobile phones created. After creating this game, I tried playing it on my phone and it was nearly impossible to play after a certain number of buttons had been added. Most websites that we use and encounter on a daily basis are compatible on both desktops and mobile devices, and I was wondering how those are implemented. Another question about web development I have is: When HTML, CSS, and JavaScript were created, was their original intent for them to be used together? The three languages truly work together so easily, so I want to know more about the origins of these languages and if this was the original intent of the languages.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours to work on this project, I would try to implement a few more features. I would first try to research how I could make this game more playable on a mobile phone. After finishing implementing the game, I tried playing it on my phone, but it was a bit difficult as the game is mainly meant to be played on a computer or monitor, as not all the buttons are visible on one screen if the user is playing on a mobile device. Another feature that I think would be fun to implement is creating levels of the game.  The user would be able to select the difficulty of the game, rather than there be a set difficulty every time. I think this would also make the game a bit more accessible, as some people may not be able to play a very difficult implementation of the game. Lastly, I think something that would be very interesting to add if I had a few more hours is to give the user more input and be able to create a pattern themselves. If a person was playing the game with a friend, they would be able to create a pattern that the friend would then have to follow. This could also be taken a step further and could be created into a player vs player game and whoever properly guesses the other player’s pattern wins.



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright Folasade Oloye

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
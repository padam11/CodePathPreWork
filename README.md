# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Rohan Buch**

Time spent: **4** hours spent in total, https://github.com/padam11/CodePathPreWork

Link to project: ripe-complete-roquefort.glitch.me

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
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!
- Make it so that it's required to press it in the same number of milliseconds (with a sizeable margin of error, of course).
- Randomize the selection of sounds AND randomize the lights that are attached to it.

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![] https://imgur.com/gallery/m6guDoa
![] https://imgur.com/gallery/LxPEIiu
![](gif3-link-here) 
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
I used StackOverflow to analyze other ways I could possibly add images to the buttons. I ended up using the CSS way to create background images. In addition, I consulted the formula for equal temperance to find the 9th note of the C major scale for the 5th button. Starts at A4 = 440 Hz.

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
There were several ways to incorporate the new images (they were images of the musical notation of the played audio). Initially using HTML, I was able to get the images to show, but the button wouldn't sound an audio unless I pressed the image in the button. In addition, the buttons were being set to the size of the images, so the buttons were all out of place. So, I decided to instead place a background image using CSS only while the specific button was active. Because the images were all from different sources and thus different sizes, I had to manually resize the images so they actually showed the notes. I put these images for fun to also make the game a learning process for music notation. Also, while overall the creation of the buttons was simply following the way it was done in the given pre-work, I initially did not understand how I would get the note I wanted, which was the 9th of the C major scale, or D5. Using the formula for a 12-tone equal-tempered scale, I plugged in 440 hertz, multiplied by (2^(1/12))^n, where n is the number of steps below or above the given note. Since D5 is 4 steps above A4, the exponent would be positive 4. If below, it's negative.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
I've always wanted to connect my passion for music-making and theory with my interests in web development and technology. What ways could I try to connect the two together uniquely? When I see sites like ESPN or Yahoo, I used to always think that developers singlehandedly update the websites with the writer's articles and whatnot. However, I now believe that it's much easier to create a framework where writers and designers can update the site. How would the developers create such a framework, almost like Wordpress for their own site? It's one thing to make a framework where you can build suites (Weebly, Wix), but it's another thing to program and entire website, then make it so that others can work on it.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
First things first, I would continue working on randomizing the array instead of creating a pre-defined secret pattern. There are several ways to do that in Javascript, and one of those methods is commented out in my code. In addition, another way I would go is to make the patterns into chords or triads (inverted sometimes to make the feature more meaningful) just to make the game more fun, even if that wouldn't add or subtract the difficulty. Third, while this would also not make a large difference in difficulty, I would space the sounds out by mere microtonal difference. This would make the game exponentially more difficult if there was no light to the game. Lastly, I would work on creating a 3-strike system like in the optional features.



## Interview Recording URL Link

[My 5-minute Interview Recording](https://youtu.be/KblSdJ-OlZI)


## License

    Copyright [YOUR NAME]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

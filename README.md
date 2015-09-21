### Lab 1, Advanced Track

1. On GitHub, fork the <a href="https://github.com/codefellows/F2-JavaScript-lab1-adv-track">lab 1 repo</a> by clicking the "fork" button in the upper right.
2. On your version of the repo, copy the "HTTPS clone url", midway down the right-hand side of your repo. It should be something like this: https://github.com/yourusernamehere/lab1-adv-track.git
3. Open your terminal and navigate to your projects directory.
4. Run this: `git clone thelinkyoujustcopiedgoeshere`
5. Change directories into your lab folder: `cd lab1-adv-track`
6. Run `npm install`.
7. Your assignment is in lab1.js. There are detailed instructions in the
comments. Be sure to read everything. Run lab.js with `node lab1.js`.
8. Before you turn in your assignment, run `grunt` to check for jshint and jscs errors/warnings. Fix all the errors.
9. List any resources you used (blogs, stack overflow questions, etc.) or collaborators below.


#### Resources and Collaborators

For the meerkat questions I used split & join, both of which I have used during the freeCodeCamp bonfire tests, but still I referenced the w3schools pages for each.
  Split: http://www.w3schools.com/jsref/jsref_split.asp
  Join: http://www.w3schools.com/jsref/jsref_join.asp
  I also discussed this very briefly with Jose Tello.  For the second part of this I used a while loop, which I largely just referenced the javascript & jQuery book.
For the Favorite / Next Animal I knew that I wanted to just be able to randomly grab one of the values from the array.  I knew Math.random would need to be in there and with a moment of searching I came up with this from stackoverflow:
  http://stackoverflow.com/questions/4550505/getting-random-value-from-an-array
    I do however still have a question regarding this question.  with my solution every time I run 'nextAnimal' it will return the same array value.  It will continue this way until I re-type: nextAnimal = favoriteAnimals[Math.floor(Math.random() * favoriteAnimals.length)];
    So technically I am getting a random animal, its just that nextAnimal needs to be re-initialised every time?
    I also worked with Kuk-rim Choe to help him establish a solution to this problem, his uses much more code but is still very functional, we also had fun trying to debug his issues.
  Now the fun one. The Hungry Lion.  This question took me a while.  I knew that I wanted to average the array total as it was incrementing.  I did some research but all of what I found was for averaging the full total.
  http://stackoverflow.com/questions/29544371/finding-the-average-of-an-array-using-js
    this link helped a bit but I really liked that this problem wasn't something I could easily find an answer to.  After putting down the laptop and working just in my mind and on paper I worked through what needed to happen for each iteration of the loop.  Once I had a clear cut series of steps the code came fairly quickly (with a bit of debugging).
    Last was the Code styling.  I was able to fairly quickly eliminate all of the style errors (indenting, correct use of spacing between operators etc...) but I still hit the yoda errors on my assertions.  I first established a solution where I assigned all of my values to variables (including the examples) and this eliminated the yoda errors (but seems a bit unnecessary). I researched yoda errors and can understand why its something to be weary of, but in these assertions it wasn't a valid concern.  Vi helped by suggesting that I could fix my grunt file to ignore yoda errors.  I used this solution because it made my code much DRYer.

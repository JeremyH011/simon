# Web Development Pre-Task Notes/Challenges:
## Echo (Easy Pre-task) <br>index_echo.html with echo.js:
* I didn't have too much difficulty with this task, it was just a matter of figuring out what exactly I wanted to happen every time 
I clicked one of the buttons.
  * I started by figuring out how to concatenate the user's inputs into a larger pattern so that the entire pattern would play
  back rather than only one note. I did this by continually adding to an array, and resetting the 2.5 s timer everytime this happened
  using clearTimeOut(), and only letting the pattern play out after a full uninterrupted 2.5 s.
  * Pattern was played back using the function provided in the skeleton code.

## Simon (Challenge Pre-Task) <br>index.html with simon.js:
* This task was a little more challenging, and my implementation does not follow the specification completely (mostly due to time 
constraints on my part. I apologize for my shortcomings). Rather than waiting for the user to select a note every time the game generated one, my implementation 
generated a random four note pattern and asked users to follow that instead (the spirit of Simon Says is essentially alive). The moment
they make a mistake in the pattern, the game tells them about it and asks whether they want to restart the game by generating a new
pattern or not.
* I approached this problem by separating it into parts that I tackled individually before integrating them together:
  * I began by adding HTML and CSS to add the necessary method of starting the game (the 'Generate Pattern' button)
  * I then worked on how I would generate the random pattern. I did this through by generating an array of length 4 with 4 randomly generated
  numbers between 0 to 3 that corresponded to indexes in the provided key array. The game would then play out the pattern.
  * Then I simply implemented the onClick function to check between user input and the pattern.
  * As a way of improving usability, I also implemented prompts at the top of the screen for users to have a better understanding of what
  they needed to do.
 
 ## Misc:
 * An oddity I found was that in the HTML file, for all references (e.g. the src for audio files) I had to delete the starting '/' for 
 my system to read anything properly (e.g. in index.html, I had to turn '/media/c_note.mp3' into 'media/c_note.mp3'). I am unsure if this was intentional, a mistake, or a hint that I was supposed to use full paths, but that
 is what I ended up doing.

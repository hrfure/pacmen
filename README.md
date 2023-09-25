# pacmen
Program that creates endless pacmen and has them moving at random within the borders of the page

**Overview:**
This is a simple PacMan game where you can add multiple PacMan icons to the screen and watch them move around bouncing off the window edges.

**HTML Layout:**
The HTML is comprised of two buttons:

"Add PacMan" - Adds a new PacMan to the screen.
"Start Game" - Starts the movement of all PacMans on screen.

**JavaScript:**
Key Variables:
pacArray: An array holding the image sources for the PacMan animations.
pacMen: An array that will contain all PacMan objects currently on the screen.
Key Functions:
setToRandom(scale): Takes in a scale and returns an object with random values scaled. Example: {x: 33, y: 21}.

makePac(): Creates a PacMan object at a random position with a random velocity. Adds a PacMan image to the game screen. Returns the PacMan's details, including position, velocity, and the image element.

update(): Loops over each PacMan in the pacMen array. Adjusts its position based on its velocity.
Checks for collisions with the window edges and makes the PacMan bounce if it hits an edge.
Updates the PacMan's image position in the DOM.
The function runs repeatedly every 20ms to update the positions of all PacMen.

checkCollisions(item): Takes a PacMan object as a parameter. Checks if the PacMan has hit any of the window's edges.
If it has, the PacMan's velocity is reversed, making it bounce.

makeOne(): Creates a new PacMan using the makePac() function and adds it to the pacMen array.

**How to play:**
Go to hrfure.github.io/pacmen to see the game in action
Click the "Add PacMan" button to add PacMan icons to the screen.
Click the "Start Game" button to make the PacMan icons start moving.
Watch the PacMen bounce around the screen!

**Further improvements**
You could look to enhance the program by changing the pacmen to "ghosts" that move at random and then create a new pacman which the player controls and try to avoid the ghosts.

**Dependencies:**
Make sure the "pacmen.js" file is located in the same directory as the HTML file and ensure that the referenced PacMan images (e.g., 'PacMan1.png', 'PacMan2.png' etc.) are also available in the directory or path.








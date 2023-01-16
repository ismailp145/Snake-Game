# Snake-Game
A snake game. 

![ezgif-3-636133a578](https://user-images.githubusercontent.com/100822861/212577660-407a445f-614a-4b3a-a673-11a20b14ff00.gif)


The game is designed to have your snake increase as it passes over the yellow fruit. By moving the arrow keys the
user controls the snake. The snake cannot go back in the same direction it is coming from, cannot touch itself, or
touch the walls. If the user does the last two, the game is over and the user is promted to restart or cancel the game. 


The index.html file sets the game board to its prefered colors, and measurements. A border, game board, snake and food
are created. And the appropriate file game.js is linked. 

The game.js is the main file that is being run. It imports many different functions from other files for the sake of 
simplicity. game.js runs the game, and updates time, draws and updates the snake. 


snake.js is the file that controls things such as snake speed, drawing the snake and updating the snake when it 
"eats" a fruit etc. It takes input from the input.js file and uses that to change the snakes direction in the x and y 
plane. 

input.js is a simple file that takes the user input and correlates that with the direction the snake will go. 
If the user selects the Up arrow key, the snake will go upwards, etc. The user is also not allowed to move the snake 
in the same direction that it came from. So if the up arrow key is pressed, the down arrow key will not do anything 
to the snake if it is pressed right after. Either the left or right must be pressed first in order to reverse the 
direction and the same is true for left and right arrow keys. 

The food.js file draws the fruit and updates its new loctation based on a function that randomly places it in a new
location on the grid in the grid.js file.

The grid.js file uses the Math.floor and Math.random methods to randomly select a location in both the x and y plane
for the fruit in the grid. 





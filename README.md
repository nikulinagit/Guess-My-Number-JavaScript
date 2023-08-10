# A simple game Guess My Number using CSS, HTML and JavaScript

**A "Guess My Number" project is a simple and fun interactive game that can be implemented using HTML, CSS, and JavaScript. The main goal of the project is to create a game where players can guess a randomly generated secret number within a specified range. This is one of the educational projects from the course "The Complete JavaScript Course 2023: From Zero to Expert!" by Jonas Schmedtmann on the Udemy**  

This JavaScript code is for a simple guessing game where the player tries to guess a randomly generated secret number between 1 and 20. Let's break down the main components and functionalities of JS code:  

**secretNumber:** This variable holds the randomly generated secret number that the player needs to guess. The line let secretNumber = Math.trunc(Math.random() * 20) + 1; generates a random decimal number between 0 and 1 using Math.random(), multiplies it by 20 to get a value between 0 and 19, then adds 1 to ensure the range is between 1 and 20. Math.trunc is used to remove the decimal part and get a whole number.  

**score** and **highscore:** These variables keep track of the player's current score (initially set to 20) and the highest score achieved in the game.  

**displayMessage:** This is a function that takes a message as a parameter and updates the text content of an HTML element with the class .message to display the given message. This is used to show different messages to the player during the game.  

**Event Listeners:**  
The code attaches an event listener to the 'Check' button (.check element) that responds to a click event. When the button is clicked, the code inside the event listener is executed.  
Inside this event listener, the code reads the player's guess from the input field (.guess element) and converts it to a number using Number() function.
The code then checks different scenarios:  
* If there is no valid guess, it displays an error message.  
* If the guess is correct, it displays a winning message, updates the highscore if applicable, and changes the background color to green.  
* If the guess is wrong, it displays whether the guess is too high or too low and updates the score accordingly. If the score reaches 0, the game ends.  

Another event listener is attached to the 'Again' button (.again element). This listener resets the game when clicked:  
* It resets the score, generates a new secret number, and resets the message to its initial state.  
* It also resets the displayed number, input field, background color, and number display width.  

Overall, this code provides the basic logic and interactivity for a number guessing game where the player can make guesses, receive feedback, and reset the game for a new round.

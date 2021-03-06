# Alexa Football Recruiting App
## How the Game Works:<br/>
This was a basic text adventure game I made when I first started learning Python my sophomore year of college. The main idea of it was to teach myself basic logic and persistent variables. When I completed it I decided to take it a step further and turn it into an Alexa skill. While not changing the structure of the original code by a lot, I did need to add things to work with the Alexa API. For instance, in the original game I used print statements to give the user information. However, this would not work for Alexa. Alexa requires a JSON to speak text. This is what the speak function achieves. While basic, this game is near and dear to my heart as one of my first projects in Python, and converting it to an Alexa skill was even cooler. <br/>

## The Backend:<br/>
This game is hosted in an AWS Lambda function. The link to that Lambda function is posted in the Alexa Skills portal and every time the user plays the game and takes their turn the script is ran. For this reason it is very important that every time the game runs the users event attribute is passed into the main statement because their session state is saved within the Alexa API, not by the script. Essentially, every time a user states a command a new instance of the game.py is run.

<br/>
Check it out here: https://www.amazon.com/joerm-Football-Recruiting/dp/B07L8FJ3MK/ref=sr_1_1?dchild=1&keywords=football+recruiting&qid=1604555711&s=digital-skills&sr=1-1

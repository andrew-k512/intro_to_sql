Your task is to compose SQL queries for the following questions:

1.    Find all the robots from Star Wars.

intro_to_sql=# Select * FROM robots WHERE source='Star Wars';

C3PO, R2D2

2.    Find the robot with an "anxious" personality.

intro_to_sql=# SELECT * FROM robots WHERE personality='anxious';

C3PO

3.    Find all recipes that are nut free.

intro_to_sql=# Select * FROM recipes WHERE nut_free=true;

Butternut Squash Bake, Vegetarian Bibimbap, French Veggie Loap, Quinoa & Black Beans, Juicy Roasted Chicken, Garlic Green Beans, Stout Slow Cooker Corned Beef and Veggies.

4.    Count the number of recipes that are gluten free but not vegetarian.

SELECT Count(name) FROM recipes WHERE gluten_free='true' AND vegetarian='false';

2

5.    Find the animal with the most legs.

SELECT * FROM animals WHERE number_of_legs > 4;

Octopus

6.    Find the board game that takes the least amount of time to play.

SELECT name, mins_to_play FROM board_games WHERE mins_to_play < 20;

Sushi Go and Quixo = 15 minutes to play

7.    Find the recipe that takes the most time to prepare.

MIN & max_players

Select min and max on whatever column.



8.    Find all the robots whose name starts with the letter M.


9.    Count the number of board games that can be played by 8 people.

SELECT * FROM board_games WHERE max_players > 7;

Cards Against Humanity & Game of Things


10.    Find all animals that are swimming and egg-laying.

SELECT * FROM recipes WHERE swimming='true' AND egg_laying='true';

Octopus and Duck.

11.    Find all animals that are swimming and egg-laying but not flying.

SELECT * FROM recipes WHERE swimming='true' AND egg_laying='true' AND flying='false';

Octopus


12.    Find the board game that supports the largest number of people.

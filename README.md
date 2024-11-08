## SDSS Computing Studies Python Assignment


Objectives:
* Retrieve data from lists of lists 
* Retrieve data from lists of dictionaries
* Retrieve data from dictionaries with lists

Once we start needing to track more data, we need to start incorporating multiple dictionaries, or data structures that are dictionaries that might contain lists, or dictionaries that might contain dictionaries!

You can imagine a game like Pokemon, where there are multiple Pokemon that have some basic statistics, and we could track their stats with a dictionary.

Consider:
```
pokemon = {
    'name' : 'Tinkatink',
    'category' : 'Metalsmith',
    'types' : ['Fairy','Steel'],
    'hp' : 3,
    'attack' : 3,
    'defense' : 3,
    'spAtk' : 3,
    'spDef' : 4,
    'speed' : 4
}
```
Notice that we have included a list in the definition of this dictionary, because it belongs to multiple types.
However, there are many pokemon, so we might create a Pokedex to keep track of them:
```
pokedex = []
pokedex.append(pokemon)
```

So how do we access data within this array?  Let's take a look at the code in example1.py

##### Task 1 Simple extraction
data from
Advanced Dungeons and Dragons Dungeon Masters Guide p74 Cleric Table
https://s3.amazonaws.com/arena-attachments/804915/348b48a0cbd967122dcb76f5cc6f5a01.pdf

This list of lists contains Table 1a Attack Matrix for Clerics, Druids and Monks 
The index specifies the level of the character, and the entry within the row specifies the target to hit Armor Class with 10 on the far left, and -10 on the far right.

Write a function that finds the target based on the level and the armor class
Check the assertion tests for expected output.

##### Task 2 Home and Away
There are teams representing each province and territory playing in a new E-Sports league.  The records for each game are included in the list titled 'games'
Iterate throught the list and determine the wins and losses for each team.

Create a dictionary for each team and store their number of wins, games played,
goals for and goals against.  A dictionary template has been prepped for you to 
use, although you can probably build one faster using iteration or list comprehension


##### Task 3 Pokedex
This assignment is inspired by the work of Purukitto on his github at:
https://github.com/Purukitto/pokemon-data.json

Use the data in this giant list to help create a Pokedex lookup.
You will ask the user to enter in the name of a pokemon, and your
program will find the entry (if it exists) and display some of
the relevant data for it.

All of the data you need is included in the variable pokemon.
Note that you can fold/hide the code by clicking on the symbols to the left of the line
to help make it easier to show only the relevant information you need.

A sample run of the program might look like this:
```
Choose a pokemon by
1. ID
2. English Name

Choice: 1

Enter the ID of your Pokemon: 2

IVYSAUR! I CHOOSE YOU!
Ivysaur is a Grass, Poison type Pokemon
Ivysaur has the following stats:
HP 60
Attack 62
Defense 63
Sp. Attack 80
Sp. Defense 80
Speed 60
Description:
There is a bud on this Pokémon’s back. 
To support its weight, Ivysaur’s legs and trunk grow thick and strong. 
If it starts spending more time lying in the sunlight, it’s a sign that the bud will bloom into a large flower soon.

Choose a pokemon by
1. ID
2. English Name

Choice: 2

Enter the English Name of your Pokemon: Mr. Yang

I'm sorry, I can't find the name of the Pokemon. Did you spell it correctly?
Enter the English Name of your Pokemon: Charmander

CHARMANDER! I CHOOSE YOU!
Charmander is a Fire type Pokemon
HP 39
Attack 52
Defense 43
Sp. Attack 60
Sp. Defense 50
Speed 65
Description:
The flame that burns at the tip of its tail is an indication of its emotions. 
The flame wavers when Charmander is enjoying itself. 
If the Pokémon becomes enraged, the flame burns fiercely.
```

Possible Extensions:
There's a lot of data here, try creating a better layout using spacing/formatting.
Some different ways to improve spacing/padding can be found at :
https://sparkbyexamples.com/python/pad-string-with-spaces-in-python/


### Table of Contents
[Game Description](#game-description)   
[Code Analysis](#code-analysis)   
[User Interface](#user-interface)   
[Output Screenshots](#output-screenshots)    

Game Description
================

## Why is it important or interesting to you?
I find board games to be repetitive and follow the same format. Monopoly has had no exciting developments to the game over the years other than re-skins for the places to rent and quippy chance tie cards.
In a game where the goal is to bankrupt the other person, some monopolies now have back loans you can take.
In an attempt to add more elements to the game, I hope to make people think about their decisions and make it not more so of luck but of money management and predictability.

## What Languages/tools/technologies did I use?
- Python
- Tykl

## What are the input and outputs for the project
### Output:
- Display of the game board, including player properties and rent values.
- Prompts for players to set rent, purchase properties, and interact with in-game items.
- Real-time minimap visualization.
### Input:
- Player responses for purchasing properties (yes/no).
- Rent percentage selection for owned properties.
- Choices for in-game items and interactions.

## What are the features that the project provides?
- 2-player board game with customizable rent settings
- Players can set their own rent prices for properties they purchase, adding a strategic element to the game.
- Properties are visually represented on the game board, with a real-time display of ownership and rent values.
- The game prompts players with decisions for purchasing properties and setting rents.
## Dynamic rent adjustment and property management
- Players can adjust rent percentages within a specified range when they land on their properties, influencing opponent decisions.
- If another player lands on a property, they can choose to pay rent or opt for a hotel stay, adding variability to gameplay.
- Option to increase hotel rent for properties, further intensifying the competition.
## Interactive in-game shop and item management
- Players can purchase items like Money Shoes or Invisibility Shoes from an in-game shop, impacting their gameplay strategy.
- Items provide temporary advantages, such as earning extra money per space traveled, introducing a tactical layer to movement and resource management.

Code Analysis
=============
- Property Inheritance: Each property in the game inherits from a base Property class, allowing for consistent management of properties.
- Rent Calculation: Each property has a function to calculate the rent based on the percentage set by the owner, ensuring dynamic and adjustable rent values during gameplay.
- Player Interaction: When a player lands on a property, the game checks ownership and prompts the player with the option to buy or adjust rent.

## Board Controls
### Buy Property:
- If the property is unowned: The player is prompted with the option to purchase it.
- If the property is owned by another player: The player must pay rent or choose to pay half the property cost to stay at a hotel, depending on their strategy.
### Adjust Rent:
- If the player owns the property: They can adjust the rent within a defined range (0.1 to 0.7) whenever they land on it. The game enforces this limit to balance gameplay







# Code analysis
# User interface 
# Output screenshots
![Screenshot 2024-08-28 013514](https://github.com/user-attachments/assets/e03d0669-8135-4a29-a27a-7d17cfb140c2)

![Screenshot 2024-08-18 175607](https://github.com/user-attachments/assets/b7a521f8-04da-4006-ad58-aed491f14e8b)


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

Output Screenshots
=============
[Shop Scenario](#shop-scenario)  
[Viewing player-owned properties](#viewing-player-owned-properties)  
[Example turn of gameplay](#example-turn-of-gameplay)  

## Shop Scenario: 

The player is introduced to the shop with two timed images: a quick shot of a surprised character and a longer shot of the shop. If the player closes the images, they can skip the timing and proceed directly to the store. 

![Screenshot 2024-08-28 020557](https://github.com/user-attachments/assets/89aed88c-d0c9-47d2-abf0-0510afcca9c3)
![Screenshot 2024-08-28 020512](https://github.com/user-attachments/assets/b7f67801-8902-4e6d-9147-d8f1429e5a60)

Once the images are displayed, the player is prompted to view item descriptions and prices. After reviewing the descriptions, they're asked if they want to make a purchase, concluding the shopping scenario.

![Screenshot 2024-08-28 021538](https://github.com/user-attachments/assets/33f60a44-33d2-4ff5-a7fd-a36bdc91ca56)

## Viewing player-owned properties

At the end of each turn, the player is prompted to choose whether to view their properties, the other player's properties, both, or none. The prompt displays the property spaces, their costs, and the rent set by the player, helping them decide whether to pay for a hotel or not.

![Screenshot 2024-08-28 022245](https://github.com/user-attachments/assets/6c74a451-682e-44fc-8e36-2d43c9317442)

## Example turn of gameplay

![Screenshot 2024-08-18 175607](https://github.com/user-attachments/assets/b7a521f8-04da-4006-ad58-aed491f14e8b)


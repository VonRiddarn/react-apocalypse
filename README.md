# React apocalypse

## Important note
This project will be made once I have a grasp on how to make components dynamic in React.  
As of now, this is just a blueprint / idea sheet.  

# The idea
A card game where the user draws a card each turn.  
The cards can be one of several types. The player can then use cards until 
their turn is over.  
This is either when a card cancels the turn by force, or the player chooses to end their turn.  
A player can use as many cards as they whish during their turn.  
At the very start of the game the player draws `X` cards that are guaranteed to not be enemies.  

## Card types
* Event - Encounter, Draw, Etc
* Enemy
* Weapon
* Food
* Health
* Armor
* Special

## Day / Night cycle
Days last for `X` turns and nights last for `Y` turns.  
Some cards can only be drawn during night or day.  
Other cards will act different during night or day.  

## Card explanations / brainstorm / moodboard

### Event
The player experiences an event with some result.  
Maybe draw `5` random cards?  
Draw `2` guaranteed `Weapon` cards?  
Recieve `X` damage?  

### Enemy
The player encounters an enemy and cannot continue until they've died to, defeated or fled from the enemy.  
The player will always have the ability to attack the enemy even if no weapons are present.  
Different enemies have different loot pools.  
When defeated the enemy will display a limited amount of categories (maybe 2?)  
The player can then choose a category and recieve a random card from that enemy's loot pool within the category.  
This will use a weighted random for rarity.

### Weapon
A weapon card have a limited amount of uses.  
If a weapon card uses ammo, some even cards will restore the ammo pool for some weapons.  

### Food
Food cards have limited uses.  
They restore hunger and / or hydration.  
In very rare instances, health.  

### Health
Limited uses, restores health.  

### Armor
Limited hitpoints.  
Will be worn until depleated or replaced.  
Will apply positive or negative effects.  
Examples:
* Thorns - Attacker takes damage.
* Heavy - Hydration decreases faster.
* Padded - Imune to getting shook / stunned.

### Special
Not sure if this is needed yet.  
The idea is to have something like a activated eventcard or something.  

Like: 
**Military interferance**  
*The military comes to your aid!*  
*Clears the board of all current enemies.*  
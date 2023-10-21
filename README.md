# Howling Frontline Dev Log
## Developers: Jackson McCall, Jack(Xinyu) Li, Nick(Qinzhou) Song

## Patch Notes for 10/21/23

### Features
- Enemy now plays an animation when it dies
- When the enemy's HP hits 0, it will stop the attack animation and start the death animation
- Enemy AI now follows player location
- Added functionality to the health and power potions that the player can buy in the shop
- Enemy AI now pauses to attack when it reaches player location, before resuming the chase

### Bug Fixes
- Made it so the player could not spam attacking, must wait for the attack animation to finish
- Fixed issue where the player's attack would not hit the dragon enemies
- Fixed issue where the enemy AI did not continuously follow the player's location after initially reaching the player
- Fixed gold so that it properly subtracted from gold bank when purchasing an item
- Fixed issue where the enemy AI's attacks would continue while chasing the player, instead of stopping to attack

### Known bugs
- After opening and then closing shop/inventory, the players movement is a LOT less responsive
- Enemy AI attacking still hits player even if player is far away at the end of the attack animation
- Health and Power potions do not do anything
- After exiting shop/inventory, the player could no longer attack, likely same delay associated with movement
- Cannot see a CameraBoom object attached to player, providing difficulties when trying to implement a zoom feature for the camera

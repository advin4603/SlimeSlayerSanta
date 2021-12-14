# Slime Slayer Santa 🎅

A puzzle game where you play as Santa and slay hordes of slimes. Submission to the IIIT-Hyd OTS-21 25KB Game Jam.
## Installation and Usage

 1. Download [SlimeSlayerSanta.zip](https://github.com/advin4603/SlimeSlayerSanta/releases/download/1.0.0/slimeSlayerSanta.zip) and extract it to a folder in your pc.
 2.  Run SlimeSlayerSanta.html using the latest version of Chrome or Firefox.
## About Slime Slayer Santa
##### Main Concepts
<details>
    <summary>Spoiler Warning (Read only after finishing the game)</summary>
	<p>
	At the surface Slime Slayer Santa is a simple "defeat the slimes" game.
	But, the main mechanic of the game is its ability to recognize changes in the game files and react accordingly.
	For example: Removing the collision file causes all collisions to be disabled. This causes santa's snowballs to pass through the enemy and causes all enemy attacks to pass through santa.
	The game's ability to react to file changes is subtly hinted to the player with the use of an intended error message during the first launch of the game asking the player to either remove audio.js to the trash folder or to edit the audio.js files hence demonstrating the two primary ways the game recognizes file changes.
	This leads to interesting puzzles forcing the player to constantly change files to complete rounds which would be otherwise impossible to do.
	The game also provides hints in the form of intentional "accidental logs" below the game canvas.
	</p>
</details>

## Walkthrough
<details>
	<summary>Spoiler Warning (Read only if stuck)</summary>
	<details><summary>Chasers</summary><p>Chasers will chase santa in a slow snail like way. Use the speed advantage to quickly shoot them down.</p></details>
		<details><summary>Shooters</summary>Shooters spew slimeballs at the Santa, slowing Santa and doing damage on impact. Disable the slimeBallEffect.js file by moving it from the GameFiles folder to the Trash folder, or setting globalState.slimeBallEffect = false; using any text editor. This will effectively disable the effect of all slimeballs in the game.</details>
		<details><summary>Excreters</summary>Excreters excrete out slime, covering almost the whole canvas. This causes Santa to use slimeballs instead of snowballs. Make sure to reenable slimeBallEffect.js file by moving it from the Trash folder to the GameFiles folder, or setting globalState.slimeBallEffect = true; using any text editor. This will reenable all slimeballs. </details>
		<details><summary>Dashers</summary>Dashers dash at Santa at high speeds and instantly kill him on impact. Disable collision.js by moving it from the GameFiles folder to the Trash folder, or setting globalState.collision = false; using any text editor. This will disable all collisions in the game causing the dashers to miss and go off the screen. This also results in santa being able to go offscreen and causes all snowballs/slimeballs to pass through Santa and the slimes. Make sure to reenable collision.js by moving it from the Trash folder to the GameFiles folder, or setting globalState.collision = true; using any text editor after the round ends.</details>
		<details><summary>Absorbers</summary>Absorbers absorb Santa's attacks and increase their health by negating the damage done to them. Make the player do "negative" damage by setting globalState.playerDamage = -1; in playerDamage.js in the GameFiles folder using any text editor. This will cause the Absorber to take damage. Make sure to set globalState.playerDamage = 1; after the round ends to prevent Santa from healing any subsequent enemies.</details>
		<details><summary>slimeMaster64</summary></details>
</details>


---
layout: project
title: Cassiopeia
description: Prototype of 2D space shooter with crafting
image: assets/images/cassiopeia-title.png
date: 2020-09-17
tags:
  - UE4
  - C++
---

<ul class="actions">
	<li><a href="https://lowcase.itch.io/cassiopeia" class="button special icon fab fa-itch-io">Download from itch.io</a></li>
</ul>

**(Solo project)**

I wanted to create something with similar mechanics to [Vigor](https://vigorgame.com/) by [Bohemia Interactive](https://www.bohemia.net/) but with simple graphics. I thought about some old arcade games. One of them seemed to be a perfect match for crafting mechanics and battle areas with resources to collect. That game is [Asteroids](https://en.wikipedia.org/wiki/Asteroids_(video_game)).

## Initial idea

At first, the game meant to be a competitive multiplayer experience where multiple players will be in the same area as the asteroids. Players will fight with each other to collect more resources and other materials. They will be able to return to the mothership at any time. After some time, the wormhole will open to bring an alien shipwreck into the area. One player will be able to collect rare resources and try to carry them back to the mothership. Other players would like to take all the loot for themself, so the finale of the battle session will be dramatic. When the player's ship is destroyed, everything taken to the battle will be lost as all the collected loot.

## Strip out the multiplayer

The first issue was multiplayer. Initially, everything seemed to be fine. But as I added more and more features the multiplayer started to be really time-consuming as I am still learning how Unreal Engine works. I had a working network synchronization for my custom movement component. But when I added [Gameplay Ability System](https://docs.unrealengine.com/en-US/Gameplay/GameplayAbilitySystem/index.html) the complexity of necessary network code quickly grew over my head. Because the deadline I set for myself was getting closer, I decided to strip out the whole multiplayer idea and continue with a much simpler single player.

## Prototype

I was able to finish the prototype at the set deadline. Some more features were stripped out, some others were simplified, but the main game loop is present.

![Screenshot](/assets/images/cassiopeia-game2.png)

![Screenshot](/assets/images/cassiopeia-game3.png)

![Screenshot](/assets/images/cassiopeia-game1.png)

![Screenshot](/assets/images/cassiopeia-game4.png)
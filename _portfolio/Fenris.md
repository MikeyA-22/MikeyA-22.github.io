---
title: "Fenris"
excerpt: "An isometric hack and slash action-adventure game where the player must traverse a frozen wasteland and defeat various types of enemies."
header:
  video:
    id: A_HaC_iI9Qw
    provider: youtube
  teaser: assets/images/fenris-title.png
  
sidebar:
  - title: "Role"
    text: "Technical Artist, UI Designer, Level Designer, Lead Artist"
  - title: "Responsibilities"
    text: "UI and UX design, User research through playtesting, concept art, 3D assets and Animations, ideation and creation of VFX, Rigging characters etc."
  - title: "Tools Used"
    text: " Unity, C#, HLSL, Blender, Cascadeur, Figma, Krita, GitKraken, Gitbash, Github Desktop, Visual Studio, Jetbrains rider, Asana"
gallery:
  #- url: /
  - image_path: assets/images/skeleton-enemy-model.png
    alt: "placeholder image 1"
  #- url: /
  - image_path: assets/images/boss-enemy-model.png
    alt: "placeholder image 2"
  #- url: /
  - image_path: assets/images/character-sword-model.png
    alt: "placeholder image 3"
gallery2:
  - url: assets/images/ice_bridge.jpg
  - image_path: assets/images/ice_bridge.jpg
    alt: "ice_bridge"
  - url: assets/images/attack_sequence.jpg
  - image_path: assets/images/attack_sequence.jpg
    alt: "ice_bridge"

---
[DOWNLOAD IT HERE!](https://dezrts.itch.io/fenris){: .btn .btn--primary}

An isometric hack and slash action-adventure game where the player must traverse a frozen wasteland and defeat various types of enemies.

## Research and Development

In the Research and Development phase of Fenris, the team initially planned to represent the five stages of grief, each with unique themes, enemies, and bosses. Due to time constraints, the scope was narrowed to focus on the "Denial" stage, featuring a snowy terrain. This shift influenced character designs, incorporating Norse elements like runes translating to "wolf" and attire inspired by Norse culture. The game drew inspiration from titles such as The Legend of Zelda, Death’s Door, and Tunic.

Playtesting revealed areas for improvement:

* **Directional Guidance**: After the sword pickup, players were uncertain of their where to go next. Implementing text cues addressed this issue.
* **Difficulty Adjustment**: The initial gameplay was too challenging. Player feedback led to difficulty balancing for a more accessible experience.

<figure class="align-right">
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/skeleton-enemy-concept.png" alt="">
  <figcaption>Concept art for a skeleton enemy</figcaption>
</figure>


## Gameplay and Level Design

The gameplay and level design of Fenris emphasizes exploration, progression, and environmental puzzles inspired by games like The Legend of Zelda, Death’s Door, and Tunic. It features a large, snowy environment where players face various enemies with unique strengths and weaknesses. 

Key mechanics include:

* **Hack and slash combat mechanics**: The player can attack with a sword shoot a long range ice shot, and roll to dynamically dodge attacks.
* **Puzzle Integration**: Using an ice shot to create bridges and a sword to clear debris, enhancing exploration and navigation.
* **Linear Progression**: Levels guide players toward a final boss while encouraging exploration through subtle environmental cues.
* **Thematic Design**: The snowy setting reflects the "Denial" stage of grief, integrating narrative and design seamlessly.

This thoughtful level design balances challenge, story integration, and player engagement.

{% include gallery id = "gallery2" layout = "full"  caption="Gameplay captures" %}

## Tutorialization

To save time on tutorialization, the game uses text based cues to direct the player in the right direction and to give them a way to easily overcome challenges they may not be fully aware of yet.


## UI and Poster Art

I created the poster and background art, and helped ideate the UI used in the game.

The UI features a simple text displayed when the player needs information, for example, when the player has a healing orb in their range. The HUD features simple hearts to indicate player's health, inspired by those used in zelda games, and the shot uses a cooldown system, indicated by a quick filling animation for the cooldown time.

## Asset Modelling(Environment And Character Art)

As the lead (and only) artist on the team, I was tasked with creating virtually all the 3D assets in the game, including the characters and environmental assets.

{% include gallery caption="Some 3D Assets I modelled." %}

## Rigging and Animation

I rigged and animated all the characters in the Game.

All the animations were done by me personally with blender and cascadeur. I used cascadeur to help block out more complex animations, such as the skeleton enemies walk
Majority of the characters were rigged with Mixamo, but for special cases where Mixamo could not match the proportions, like the rock monster and the wolf, I had rigged personally.

<div style="display: flex; justify-content: space-between;">
  <iframe src="https://drive.google.com/file/d/18eREtWtLDXI1qvew9EnOkglgi1DDirOQ/preview" width="200%" height="240" allow="autoplay"></iframe>
  <iframe src="https://drive.google.com/file/d/1d2ih3Co7Kx2URPSQtF9JcEfXJIYGiD5p/preview" width="200%" height="240" allow="autoplay"></iframe>
</div>

## VFX and Shaders

I created some of the VFX and shaders used in the game including:

* The water depth, which had to be adjusted for the isometric view, so depth could still be seen in the water.
* The slash vfx
* The dappled lighting, made using cloud cookies, as seen in games like Tunic and Death's door

<div style="display: flex; justify-content: space-between;">
  <iframe src="https://drive.google.com/file/d/11NUaRDnglhB44KkTzfWWIbDYVbY3HRdm/preview" width="200%" height="240" allow="autoplay"></iframe>
  <iframe src="https://drive.google.com/file/d/10BchQBqbshbvzYG__4-1Ww5-Dl_TBYf2/preview" width="200%" height="240" allow="autoplay"></iframe>
</div>
<div style="display: flex; justify-content: space-between;">
    <iframe src="https://drive.google.com/file/d/1ZjbGBvXADU6nvnhvYT6JUOucsYNs5rRP/preview" width="200%" height="240" allow="autoplay"></iframe>
    <iframe src="https://drive.google.com/file/d/1UasAifRMueZwevoGGhIyOhyB7UspmsKS/preview" width="200%" height="240" allow="autoplay"></iframe> 
</div>
<iframe src="https://drive.google.com/file/d/1NZH6Hpus3sazNLeHeCoctvtn4k-W7Ulq/preview" width="640" height="480" allow="autoplay"></iframe>
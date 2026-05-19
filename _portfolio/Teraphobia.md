---
title: "Teraphobia"
excerpt: "A first-person asymmetric multiplayer game where up to 3 Survivors and 1 Void Monster battle it in an abandoned facility."
header:
  video:
    id: Ah3SFiK0x1s
    provider: youtube
  teaser: assets/images/teraphobia.png
  
sidebar:
  - title: "Role"
    text: "Lead Artist, Technical Artist, UI Artist, AI Programmer"
  - title: "Responsibilities"
    text: "UI and UX design, User research through playtesting, concept art, 3D assets, Dynamic Animation and Rigging etc."
  - title: "Tools Used"
    text: " Unity, C#, HLSL, Blender, Cascadeur, Figma, Krita, GitKraken, Gitbash, Github Desktop, Visual Studio, Jetbrains rider, Asana etc."
gallery:
  - url: assets/images/void20concept.png
    image_path: assets/images/void20concept.png
    alt: "concept art"
  - url: assets/images/void20concept_other.png
    image_path: assets/images/void20concept_other.png
    alt: "concept art"
  - url: assets/images/teraphobia-set-test.png
    image_path: assets/images/teraphobia-set-test.png
    alt: "set test"
    caption: "Caption test"
  - url: assets/images/OGcharacter-Terraphobia.png
    image_path: assets/images/OGcharacter-Terraphobia.png
    alt: "set test"
  - url: assets/images/final_Character.png
    image_path: assets/images/final_Character.png
    alt: "set test"    
gallery2:
  - url: assets/images/Terphobia-AI-Diagram.jpeg
    image_path: assets/images/Terphobia-AI-Diagram.jpeg
    alt: "set test"    
---
[Check it out here!](https://www.gamecon.ca/2025/third/100-ideas){: .btn .btn--primary}

Based in a post apocalyptic world, you and your team fight against another player, playing the monster, to 
collect all the batteries and escape the area!
Made with a team of 7, 
Inspired by games such as Dead By Daylight and Lethal Company.

## Research and Development
We initially planned for the game to have procedural level generation, 
which would have allowed us to create multiple levels quickly without the need to 
have more hands on deck for overall game design, But had to scope down to one level, due to our usual foe, 
time constraints. 

## Art

As the Lead Artist, I had to:

* Create seamless textures that could be used throughout the environment, giving us a distinct style. 
* Create some concept art for the game, including the monster's concept art.
* Design and Create the Character.
* Coordinate with both programming and design teams to make sure the assets would work within the engine.
* Oversee the assets being produced by myself and my colleague.



<div style="max-width: 50%">
    {% include gallery id = "gallery"  caption="Various works" %}

</div>

## AI Programming

While the game did not originally feature enemy AI, a teammate and I added an AI monster version.

This version made use of two Artificial Intelligence Systems, a custom behaviour tree and a custom GOAP (Goal Oriented Action Planner) System.

We accomplished this by first creating the behaviour tree system, then making a GOAPNode as a custom node, which could have actions as children, and internally planned the best possible action depending on the moment.


This allowed for the enemy AI to operate based on the current state of the world to act dynamically and uniquely when attacking the enemy.

Below is a Diagram outlining our system and it's implementation.


<div style="max-width: 50%">
    {% include gallery id = "gallery2"  caption="Various works" %}
</div>






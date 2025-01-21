---
title: "Table tennis 3D"
excerpt: "A personal project for a week long game jam inspired by games like rockstar table tennis and mario tennis aces, smash into an immersive and challenging table tennis experience."
header:
  video: 
    id: 8LHRVPG-6gs
    provider: youtube
  #image: /assets/images/Table-tennis-level1.png
  teaser: assets/images/tt_level1.jpg
sidebar:
  - title: "Role"
    text: "Sole creator: Designer, Developer and Artist."
  - title: "Responsibilities"
    text: "Character Design, Artificial Intelligence Programming, Shaders, VFX, Animation"
  - title: "Tools Used"
    text: "Godot, Figma, GDScript"
gallery:
  - url: /assets/images/Level 1.png
    image_path: assets/images/Level 1.png
    alt: "placeholder image 1"
  - url: /assets/images/Level 2.png
    image_path: assets/images/Level 2.png
    alt: "placeholder image 2"
  - url: /assets/images/Level 3.png
    image_path: assets/images/Level 3.png
    alt: "placeholder image 3"
---
[DOWNLOAD IT HERE!](https://mikey-a.itch.io/table-tennis){: .btn .btn--primary}

## Research and Development
As a big fan of sports games, NBA 2K,EA F.C., Madden and the like, I would always ask myself, how does the AI replicate the player's tendencies so well? To try and answer this question for myself, I decided to use a simple game as a first look into the world of creating different variations of advanced AI for games.

My points of inspiration for this game comes from two games in particular, Mario tennis aces, and rockstar present: Table tennis. Both these games have crafted characters with such different play-styles and attacks from one another that I knew I had to see for myself how this could possibly work.

I decided to use Godot not only as a challenge to myself, though I had some experience with it in the past, it was not my go-to engine, but also for the easy readability and deployment of GD script, which allowed for rapid development and iteration, making it the perfect engine for quickly creating in a game jam environment.


{% include gallery layout = "half" caption="The three levels and AI enemies in the game." %}

## Playtesting
Due to the short time period, my playtesters were mostly my friends and roommates! I was able to make the following changes due to their contribution:
* **Targeting system**: The targeting originally featured an aim that moved to where you aimed at at a set speed, but this was too slow, so I made it snap from one spot to another on the table
* **Statistics Balancing**: The power used by each player and AI was tested by my friends, and through this we were able to determine what is a good balance of power and control.

## Implementation

The concept that I used as my starting point for the project was that of a finite state machine, as I had experience with this in the past, with my pomodoro timer project, using this as a jumping off point was really helpful to me in the sense that I could easily visualize the different states that I would be using for the characters.

After implementing the basic gameplay with FSMs included, I continued to experiment to improve upon the game's original design, as originally all the collisions were handled using collision boxes, but when I realized that this was causing a physics issue, I switched to raytracing to help improve the functionality of the collision and this worked wonders to fix the error.

## Art/ Effects
I also made use of godot's shader system to create a simple slash vfx for the forehand and backhand(A bit of tennis lingo for you) and to create a trail for the ball, as well as to help me create multiple characters, using a simple color masking shader to allow me to alter the color of my initial texture to help easily create variants of my original character to create my enemies for the different levels.

## Final AI implementation
The final and most important part of my implementation is the tendencies feature. I wanted all the player to have their own unique and totally malleable features controllable in-engine, allowing me, the designer, to make simple changes to their abilities, speed, force they put on the ball, to help create the perfect enemies for each level.

I did this by giving each of the AI their own variable, and making the shots unique individual resources, or in unity terms, scriptable objects, that each had their own settings for the different types of shots that could be executed. 

For the AI's decision-making there were numbers that would decide how likely the AI was to use a certain shot, and a variable for how high the ball should be as a consideration for this shot as well. the code would then give a random number, and depending on where this number falls in the range of the tendencies, and how high or low the ball is, the AI would then decide what shot it would use. This worked very effectively to make the AI decide how it would attack the player, and to create variants of this attack, allowing each AI to have a unique attack pattern.

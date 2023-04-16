# Prompting Galaga

So the idea here is to create the arcade game Galaga (or as much of it as possible) with AI prompts only. There are going to be a lot of stock images that I'll need to use, like the ship and enemy sprites, but a lot of the sounds could probably be AI generated, and of course, the code.

I'm going to play it pretty fast and loose with the journal / documentation for this project because I don't want to get bogged down writing everything down. I'd rather just build stuff!

## The Basics

Without knowing very much about game development, I should probably ask about the generalities of game development so I have a better idea of how to approach this project.

### Getting the First Prompt

I'll start with ChatGPT. I've tried to build some games in the past, but I've never really gotten past the basics of it, and any attempt was before I actually learned to code for data science. I expect it'll be much easier when I have a machine to write it all for me, and I can focus more on the design ("much easier" I say. More like "best laid plans"...)

Considering that I know almost nothing about game design or development, I should probably start with some basic questions. First thing I want to write up is a prompt I can reuse to get ChatGPT into the best role for answering the questions that I have.

**Here's the prompt I will use to begin:** "You will act as a video game developer and designer with more than 30 years of experience. You have developed games using all prebuilt game engines, like Unreal Engine and Godot; you have even developed custom game engines yourself. You have created games for triple-A companies, small indie developers, and everything in between. You have an extensive knowledge of how games are designed and developed, how a developer chooses which game engine to use for their project, what makes games engaging, and how to plan out the development process. <br>
I will be your student, and I will ask you questions about video game design and development. Your responses should be clear and concise, and written at an eighth-grade reading level. Your responses should be tailored to assume that I have very little knowledge of game design and development, but I do have a background in data science and some coding / programming experience in Python. <br>
If you do not understand my question, or it is too vague, you will ask clarifying questions until you understand my request. If you understand, summarize our respective roles, and ask for my first question."

**GPT's Response:** "Great! I will be your video game developer and designer with over 30 years of experience, and you will be my student with some coding and programming experience. Please feel free to ask me any questions about video game design and development. What would you like to know first?"

An excellent start. I have several questions to begin.

### Basic Game Development Questions

**Q1.** What are the first 5 things I should know as a new video game developer?

**GPT's Response:** "As a new video game developer, there are several things that you should keep in mind. Here are five key points to consider:
1. Choose a game engine: A game engine is a software framework that game developers use to create video games. There are many different game engines available, ranging from beginner-friendly tools like Construct and GameMaker Studio to more advanced engines like Unity and Unreal Engine.
2. Learn a programming language: While many game engines have visual scripting tools, knowing how to code is essential for game development. Some popular programming languages used in game development include C++, C#, Java, and Python.
3. Focus on gameplay: The most important aspect of any game is gameplay. Make sure that the core mechanics of your game are fun and engaging. Take inspiration from games that you enjoy playing and try to understand why they are fun.
4. Start small: Game development can be overwhelming, so it's important to start with small, manageable projects. This will help you build your skills and gain confidence as a developer.
5. Get feedback: It's important to get feedback on your games from other people. This can help you identify areas for improvement and make your games more enjoyable for players. You can share your games with friends, family, or online communities to get feedback."


**Q2.** What are the 5 most important concepts a game developer should understand?

**GPT's Response:** "As a game developer, there are several important concepts that you should understand in order to create successful and engaging games. Here are five of the most important:
1. Game mechanics: Game mechanics are the rules and systems that govern how a game works. Understanding game mechanics is essential for creating fun and engaging gameplay. Some common game mechanics include movement, combat, puzzles, and resource management.
2. Player psychology: Understanding player psychology is crucial for creating games that are enjoyable and engaging. This includes understanding what motivates players, how they think and behave, and what keeps them coming back to play your game.
3. Game design principles: Game design principles are the guidelines that game developers use to create successful games. These principles cover everything from player feedback and balance to level design and pacing. Understanding game design principles will help you create games that are well-designed and enjoyable to play.
4. User interface design: User interface design is the art of designing interfaces that are easy to use and understand. In game development, this includes designing menus, HUDs, and other on-screen elements that are intuitive and easy to navigate.
5. Project management: Game development is a complex process that involves many different tasks and team members. Understanding project management principles such as agile development, milestone tracking, and task prioritization will help you manage your projects more effectively and deliver high-quality games on time and within budget."

**Q3.** What are the 5 most important concepts of game design?

**GPT's Response:** "As a game designer, there are several important concepts that you should understand in order to create successful and engaging games. Here are five of the most important:
1. Player engagement: Players are the most important part of any game, and understanding what engages them is crucial for creating successful games. Engaging games offer players challenges, rewards, and a sense of progression.
2. Game mechanics: Game mechanics are the rules and systems that govern how a game works. Understanding game mechanics is essential for creating fun and engaging gameplay.
3. Narrative design: Narrative design is the process of creating a compelling story for your game. A well-crafted narrative can help players connect with the game world and feel invested in the game's characters and events.
4. Level design: Level design is the process of creating the environments and challenges that players will encounter in your game. Good level design can help create a sense of immersion and challenge for players.
5. User experience design: User experience design is the process of creating interfaces and interactions that are intuitive and easy to use. In game development, this includes designing menus, HUDs, and other on-screen elements that are easy to navigate and understand. Good user experience design can help keep players engaged and immersed in the game world."

**Q4.** What are the common phases of game development?

**GPT's Response:** "Game development typically involves several phases, each with its own set of tasks and objectives. While the exact phases and their names may vary depending on the development team and project, here are some of the most common phases of game development:
1. Pre-production: This phase is where the initial concept and design for the game are created. It involves creating a design document, developing a game prototype, and conducting market research to determine the viability of the game.
2. Production: This is the main development phase where the game is created. It involves creating game assets, programming game mechanics, developing levels, creating sound effects and music, and testing the game.
3. Alpha: This phase involves creating a playable version of the game that includes all the core features and content. The game is not yet complete, but it is playable and can be tested by a limited group of people.
4. Beta: This phase involves polishing and refining the game based on feedback from alpha testing. Additional features may be added, and bugs are fixed. The game is tested by a larger group of people, including external playtesters.
5. Release: This is when the game is completed and made available to the public. The game is launched on various platforms, and marketing efforts are focused on promoting the game to potential players.
6. Post-release: After the game is released, ongoing support is necessary to maintain the game and address any issues that arise. This includes bug fixes, patches, and updates, as well as creating additional content and expansions to keep players engaged."

**Q5.** What are the 5 most important personality traits of a game developer?

**GPT's Response:** "Game development is a complex and demanding field that requires a range of different skills and personality traits. Here are five of the most important personality traits for a game developer:
1. Creativity: Game development is a creative process, and game developers need to be able to come up with new and innovative ideas. Creativity is also important for problem-solving and finding new solutions to challenges that arise during development.
2. Perseverance: Game development is a long and challenging process, and setbacks and roadblocks are common. Game developers need to be able to push through these obstacles and keep working towards their goals.
3. Collaboration: Game development is a team effort, and game developers need to be able to work well with others. This includes communicating effectively, sharing ideas, and being open to feedback and critique.
4. Attention to detail: Games are complex systems with many different elements, and game developers need to be able to pay close attention to detail in order to ensure that everything works together seamlessly. This includes debugging code, testing gameplay mechanics, and ensuring that all game assets are properly integrated.
5. Passion: Game development is a demanding field, and game developers need to have a genuine passion for creating games. This passion drives them to work long hours and to continuously strive to create better games."

### Galaga Questions Round 1

These are some good responses. Now I have a better idea of what I'm doing overall.

Since I'm going to be recreating Galaga, I should more explicitly understand the elements of Galaga. I expect ChatGPT will know the game, and be able to explain its elements to the degree of specificity I desire.

**Q6.** I am going to be recreating the arcade game Galaga. I need to know that you know Galaga, since you will be helping me recreate this game, so to confirm that you know about Galaga, please provide a surface-level description of Galaga and its main gameplay loop.

**GPT's Response:** "Yes, I am familiar with Galaga! Galaga is a classic arcade game that was first released in 1981 by Namco. The game is a fixed shooter, where the player controls a spaceship at the bottom of the screen, and must fight off waves of enemy ships that fly in formation at the top of the screen.<br>
The main gameplay loop of Galaga involves shooting down the enemy ships while dodging their attacks. The player can move left and right to avoid enemy fire and can also fire a stream of bullets to destroy the enemy ships. The game is divided into stages, with each stage consisting of several waves of enemy ships. The gameplay becomes more challenging as the player progresses through the stages, with the enemy ships becoming faster and more difficult to defeat. <br>
One unique feature of Galaga is the ability for the enemy ships to capture the player's spaceship using a tractor beam. If the player manages to shoot down the enemy ship that has captured their spaceship, they will be able to control both ships simultaneously, doubling their firepower. If the player loses a life, however, the captured spaceship is lost as well. <br>
Overall, Galaga is a classic and challenging arcade game with simple but addictive gameplay that has remained popular for decades."

I want to test the AI a little bit, so I'm going to follow up with this:

"Describe the win condition and the loss condition for Galaga if they exist."

**GPT's Response:** "The win condition for Galaga is to complete all of the game's stages, defeating all of the waves of enemy ships and bosses. The game loops back to the first stage once the final stage is completed, so players can continue playing to achieve higher scores. <br>
The loss condition for Galaga is to lose all of the player's lives by being hit by enemy fire or colliding with enemy ships. The player starts with three lives, and can earn extra lives by achieving certain score milestones. Once all lives are lost, the game is over, and the player must start again from the beginning."

A solid response. Now I need a game engine to develop Galaga (and by association, the scripting language of choice). I want to test the AI's ability to remember information from the initial prompt, and see if it makes any disclaimers about "recommending" a game engine.

**Q7.** Given what you know about Galaga, and given what you know about me as your student, and given that you will be writing most of the code / scripting for me, choose the best game engine I should use to recreate Galaga. Provide a detailed explanation of your reasoning for the game engine you choose, including how the strengths of the engine coincide with the project needs, and some possible barriers I may encounter while developing Galaga with this engine. Also provide two other game engine choices, and for each, provide a short explanation of why they are inferior to your first choice.

**GPT's Response:** "Based on what I know about Galaga and your background, I would recommend using the Godot game engine to recreate Galaga. <br>
Godot is a powerful, open-source game engine that is well-suited for 2D game development, which is the format of Galaga. The engine includes a robust set of tools for creating and managing game assets, as well as a powerful scripting language that can be used to implement gameplay mechanics and other features. The Godot engine is known for its flexibility and ease of use, which makes it a good choice for both experienced and novice game developers. <br>
In addition to its strengths in 2D game development, Godot is also well-suited for developing arcade-style games like Galaga, with its customizable physics engine and support for particle effects, animations, and other visual effects. <br>
One potential barrier you may encounter while developing Galaga with Godot is that it may require some learning to become proficient in the engine and its tools, especially if you are not familiar with game development. Additionally, because Godot is an open-source engine, there may be fewer resources and tutorials available compared to more widely used commercial engines like Unity or Unreal. <br>
As for two other game engine choices, one option could be Unity. Unity is a widely used game engine that is known for its versatility and cross-platform compatibility. However, Unity may not be the best choice for recreating Galaga, as it is not specifically tailored towards 2D game development and may require more setup and configuration to work effectively. <br>
Another option could be Unreal Engine. Unreal Engine is a powerful game engine with advanced tools and features, but like Unity, it may not be the best choice for a 2D game like Galaga. Unreal Engine is also known for its steep learning curve, which may be challenging for beginners. <br>
Overall, I believe that Godot is the best choice for recreating Galaga due to its strong support for 2D game development, customizable physics engine, and ease of use."

GPT recommended that I start small, but I should have an understanding of the design of my game, and know what elements in that design are required for a minimum viable product.

In the initial prompt, I asked GPT to ask clarifying questions if the question I asked was too vague. I know I need a design document of some kind, but I'm not sure what should go into it, or how it should be structured.

**Q8.** Create a high-level outline for a Game Design Document for Galaga. OUTPUT: Markdown format with #Headings, ##H2, ###H3, + bullet points, + sub-bullet points

**GPT's Response:** <br>
"""
#### Game Design Document: Galaga <br>
##### Overview
- Brief description of the game and its genre
- Description of the target audience and intended platform(s)
##### Gameplay Mechanics
- Description of the game's core gameplay loop
- Overview of the player's controls and abilities
- Description of enemy behavior and abilities
- Power-ups and other special gameplay elements
##### Game World
- Description of the game world and setting
- Overview of the game's visual style and tone
##### Levels and Progression
- Overview of the game's level structure
- Description of enemy waves and boss battles
- Progression and difficulty balancing
##### Audio and Music
- Description of the game's audio design and music
- Overview of sound effects and other audio elements
##### User Interface
- Description of the game's user interface
- Overview of menus, HUD, and other interface elements
##### Technical Requirements
- System requirements for the game
- Overview of required assets and resources
- Description of the game engine and development tools used
##### Team and Development
- Description of the development team and roles
- Overview of the development timeline and milestones
- Budget and resource allocation
##### Marketing and Distribution
- Description of the game's marketing strategy and target audience
- Overview of the distribution strategy and platform(s)
- Description of any promotional campaigns or events
##### Legal and Intellectual Property
- Overview of the game's legal and IP considerations
- Description of any licensing agreements or contracts
- Overview of trademark and copyright protections

This is just a high-level outline, but it should give you a good starting point for creating a more detailed Game Design Document for Galaga. <br>
"""

It's pretty good, a little generic, but I gave it a generic prompt, so I'm not mad. 

I don't really need to specify System Requirements (any modern computer will run it), Marketing and Distribution (I'm not selling it), or Legal and Intellectual Property (again, not selling it). I also don't need to describe team and roles, since it's just me building it, nor budget and resource allocation (there is no budget).

The plan is to ask GPT about each of these sections in more detail, and have it complete the design document for me.

In the meantime, I want to see what it recommends if I ask it to jumpstart development and dive right in without the design document.

**Q9.** I don't want to spend a lot of time working on a design document before I've even started building anything. Explain step-by-step what I should do to jumpstart my development and immediately start building Galaga in Godot. Limit your response to ten easy steps that should take no more than an hour each. Provide one or two supporting sentences per step.

**GPT's Response:** "Sure, here are 10 easy steps to jumpstart your Galaga development in Godot:
1. Download and install Godot - download Godot from the official website, and follow the installation instructions.
2. Create a new Godot project - start a new project in Godot and give it a name.
3. Set up the game window - adjust the game window size and other settings in the project settings.
4. Create a new scene for the player - create a new scene for the player and add a sprite and a control script.
5. Implement player movement - add code to the control script to allow the player to move left and right.
6. Add player shooting - add code to allow the player to shoot bullets at enemies.
7. Create a new scene for enemies - create a new scene for the enemies and add a sprite and a control script.
8. Implement enemy movement - add code to the control script to make the enemies move down the screen.
9. Add enemy shooting and spawning - add code to allow the enemies to shoot at the player and to spawn new enemies.
10. Implement collision detection - add code to detect collisions between the player, the enemies, and the bullets.

These steps should get you started on building the core gameplay loop of Galaga in Godot, and allow you to iterate and build upon it as you refine and expand the game."

I like this a lot better than writing up a whole design document! I'm going to get started on this.

## Jumpstarting Development

GPT has given me a good set of starter instructions for creating Galaga. No need for all the wordy design documents - just jump in and get my hands dirty.

### Preparing Development

I need to install Godot, but I should be careful. Since the model is only trained on data since about 2021, I should choose the most recent version of Godot that GPT is aware of, since I don't want to install a newer version that may have deprecated features (I won't be able to ask GPT to write code with a Godot version from the future!).

I am curious to see if GPT can rank its "confidence" in something.

**Q10.** What is the most recent Godot version you are aware of? What version of Godot are you most confident in scripting?

**GPT's Response:** "The most recent stable version of Godot at the time of my knowledge cutoff date of September 2021 was Godot 3.3.4. However, it's possible that a newer version has been released since then. <br>
As an AI language model, I am not capable of coding, so I do not have direct experience scripting in any particular version of Godot or any other game engine. However, I have been trained on a large corpus of information about Godot and other game engines, so I should be able to provide general advice on how to use them."

Interesting - I've had GPT write code before, but it doesn't think it can. I wonder if it thinks it's providing "general advice" when it provides code snippets.

I'm looking at the Godot downloads page for 3.3.4 and I'm pretty confident the download I'm looking for is "Godot_v3.3.4-stable_win64.exe.zip".

It's installed. Easy step 1 is down! Time to start a new project and give it a name. I like "Prompt2Galaga".

Alright. Easy step 2 is down! I have a new project open and I have no idea what I'm doing. Let's see if GPT can guide me to victory.

**Q11.** I have a new blank Godot project open in Godot 3.3.4. I need to create a new scene for my Galaga game, add the player, add a player sprite, and add a player control script. Provide a step-by-step explanation of how to create a new 2d scene.

**GPT's Response:** "Sure! Here are the steps to create a new 2D scene in Godot: <br>
1. In the Godot editor, click on the "File" menu at the top left corner of the screen.
2. Select "New Scene" from the dropdown menu. This will open the Scene panel.
3. In the Scene panel, click on the "2D Scene" button to create a new 2D scene.
4. In the new 2D scene, click on the "Node" button in the top left corner of the screen to add a new node.
5. In the "Add Node" window that appears, type "KinematicBody2D" into the search bar and select it.
6. With the KinematicBody2D node selected in the Scene panel, click on the "Node" button again to add a child node.
7. In the "Add Node" window, type "Sprite" into the search bar and select it.
8. In the new Sprite node, click on the "Texture" property in the Inspector panel on the right side of the screen, and select a sprite image for the player from your computer.
9. With the player Sprite selected in the Scene panel, click on the "Node" button to add a new script.
10. In the "Add Script" window, select "New Script", give it a name like "PlayerControl.gd", and click "Create". This will open the new script in the Godot editor, where you can start writing code to control the player.

With these steps, you should now have a new 2D scene in Godot with a player character and a player control script attached to it. You can continue building your Galaga game from here!"

I followed all steps except for 8. I don't have a sprite to upload from my computer.

### Generating Sprites

I could go online and quickly find a Galaga ship sprite, and upload it into the game, but as an exercise in prompting, I'd like to have an AI generate the sprites. Time to do some research on image generation AI's. This is probably a task for Google, but I'll let GPT put in its two cents.

**Q12.** I would like my game's sprites to be created by an image generation AI. The images should be easily convertible to sprite files compatible with Godot. What image generation AIs are best suited for this task?

**GPT's Response:** "There are several image generation AIs that could be used to generate sprites for a game like Galaga. Here are a few options to consider:
1. DALL-E: DALL-E is an AI model developed by OpenAI that generates images from textual descriptions. It could be used to generate sprite images based on textual descriptions of the game's assets. However, it may require additional processing to convert the generated images into sprites.
2. StyleGAN2: StyleGAN2 is another AI model that generates high-quality images. It could be trained on existing sprite images to generate new ones that are similar in style. However, training the model may require significant computing resources.
3. GANbreeder: GANbreeder is a web-based tool that allows users to generate images by mixing and matching different images. It could be used to generate sprite images by combining different visual elements.

Once the images are generated, they can be easily converted to sprite files compatible with Godot using a tool like TexturePacker or by importing them into Godot and manually creating sprite frames."

I think for projects where I will be using online images as concept art, StyleGAN2 and GANbreeder would be interesting choices. I'd like to stick with generation using text, since that's my prompting focus. I've worked briefly with DALL-E before, but I'll ask Google for some more options.

It's crazy to see the web already flooded with art generation AI.
- neural.love
- replicate
- fotor
- pixelz.ai
- hotpot.ai

And many, many more. There's a lot of "sign up for free" sites. I don't need any more emails, thanks. I'll need to find one that generates free sprites with no generation limit.

Craiyon looks promising, but it's really slow.<br>
pixray looks like my best bet so far. It's free, and the API looks relatively simple, if I wanted to try it.<br>

I've been researching for the past hour or so, and I've come to a conclusion - Slow, free or good: pick 2. I expect that if I want to do this with any degree of consistency, I'll have to create the initial art in a more photorealistic generator, move the image into a "pixellator", then convert to a sprite file. I don't love the idea of all the extra work to make it happen. I expect I'll find a better solution in the future. It was a nice idea, but I don't want to spend all my time waiting for image generators to run when I could just use the stock Galaga images.

### Importing Sprites

I went to Google and searched for Galaga sprites. Now I have a sprite sheet of (mostly) all of the different Galaga sprites downloaded locally. The sheet says to give credit if used; here's to you, JDASTER64.

I'm not sure how I'm supposed to use this in my project, but GPT does.

**Q13.** I have a Galaga sprite sheet downloaded to my local files. How do I import the sprites into my Godot game project?

**GPT's Response:** "To import a sprite sheet into a Godot game project, you can follow these steps:

1. Open your Godot project and navigate to the FileSystem panel on the left-hand side of the editor.
2. Locate the folder where you want to import the sprite sheet and right-click on it to open the context menu.
3. Click on "Import" to open the Import dialog box.
4. In the Import dialog box, click on the "Add..." button and browse to the location of your sprite sheet file. Select it and click "Open".
5. In the Import dialog box, you can specify the import settings for the sprite sheet, such as the pixel filter and import resolution. Adjust these settings as needed.
6. Click on "Import" to import the sprite sheet into your Godot project. This may take a few moments depending on the size of your sprite sheet.

Once the sprite sheet is imported, you can create a Sprite node in your scene and assign the sprite sheet texture to it by selecting the node and opening the Inspector panel. From there, you can set the Sprite's frame size and adjust its position on the screen. You can also create an AnimationPlayer node to animate the Sprite by assigning different frames of the sprite sheet to different animation frames."

I didn't see an import button when I tried to follow these steps so I just dragged the sprite sheet from my local files into the Godot folder in the FileSystem window. That seemed to work okay, but I didn't have the option to specify import settings for the sprite sheet.

The rest of the instructions aren't clear enough for me to follow.

### Assigning the Sprite to the Player Object

**Q14.** I have a sprite sheet in my Godot game files. I would like to create a sprite node and assign the sprite sheet texture to it. Explain how to do this step-by-step.

**GPT's Response:** "Sure! Here's a step-by-step explanation of how to create a sprite node and assign the sprite sheet texture to it in Godot:

1. In the Scene panel on the left-hand side of the Godot interface, right-click on the node that you want to add the sprite to, and select "Add Child Node" from the context menu.
2. In the "Create New Node" window that appears, select "Sprite" from the list of available node types, and click "Create."
3. In the "Inspector" panel on the right-hand side of the Godot interface, scroll down to the "Texture" section, and click the "Load" button next to the "Texture" property.
4. In the file browser window that appears, navigate to the location where your sprite sheet is saved, select it, and click "Open."
5. You should now see the sprite sheet texture displayed in the "Texture" property of the sprite node in the Inspector panel. If you want to adjust the position or size of the sprite within the node, you can use the "Region" and "Scale" properties in the "Texture" section.

That's it! You now have a sprite node with the sprite sheet texture assigned to it in your Godot game project."

I did as instructed, but now the entire sprite sheet is assigned to the sprite, instead of just the part that I want (the player ship sprite). I'm not sure how to write these instructions, but here's a shot.

**Q15.** I do not want to assign the entire sprite sheet as the texture of my sprite because my sprite sheet contains multiple sprites. I want only one of the sprites on the sprite sheet to be the sprite assigned to the Sprite object. How do I assign only a single sprite on the sprite sheet to the Sprite object?

**GPT's Response:** "To assign only a single sprite on the sprite sheet to the Sprite object, you need to create a new Rect2 object that defines the region of the sprite sheet that contains the sprite you want to use, and then assign this Rect2 object to the sprite's region_rect property. Here are the steps to do this:

1. In the FileSystem panel, select the sprite sheet that contains the sprite you want to use.
2. In the Import panel, make sure the "Split mode" is set to "Individual".
3. Click the "Reimport" button to re-import the sprite sheet.
4. In the FileSystem panel, expand the sprite sheet to see the individual sprites that were created when you re-imported the sprite sheet.
5. Select the sprite that contains the sprite you want to use.
6. In the Import panel, note the "Offset" values for the sprite. These values indicate the position of the sprite on the sprite sheet.
7. Create a new Rect2 object with the same dimensions as the sprite, and set its position to the negative of the "Offset" values you noted in the previous step.
8. Assign the Rect2 object to the sprite's region_rect property.

Your Sprite object should now display the single sprite you selected from the sprite sheet."

I'm not seeing a "Split mode" option from instruction 2. Off to Google.

So after about an hour of googling for answers, I should've just used my brain for two seconds when looking at the "Region" section in the Inspector. It turns out that it does pretty much exactly what I want when I set {x:80, y:21, w:11, h:12} for the player sprite. I could work on prompting GPT for this, but I'll have plenty of prompting practice with the rest of the project.

It's also interesting to see how the overcomplicated Q15 caused GPT to hallucinate an overcomplicated response. Garbage in, garbage out.

I clicked the play button in Godot just to see what it would do. It does load the scene and shows my sprite (in the upper left corner) but that's about it. Good! Exactly as expected.

### Letting the Player Move Back and Forth

Now for the fun part: I need to give the player an opportunity to move back and forth with the arrow keys. Time to have GPT code the PlayerController!

**Q16.** I have a 2D player object with a PlayerController script. The player is able to move left and right with the left and right arrow keys, respectively. Write the PlayerController code in GDScript, then explain your code step-by-step.

**GPT's Response:** "Certainly! Here is an example implementation of the PlayerController script in GDScript:

```
extends KinematicBody2D

const SPEED = 200
const GRAVITY = 1000
const JUMP_FORCE = -500

var velocity = Vector2()

func _physics_process(delta):
    var input_vector = Vector2()
    input_vector.x = Input.get_action_strength("ui_right") - Input.get_action_strength("ui_left")

    if is_on_floor():
        if Input.is_action_just_pressed("ui_up"):
            velocity.y = JUMP_FORCE
    else:
        velocity.y += GRAVITY * delta

    velocity.x = input_vector.x * SPEED
    velocity = move_and_slide(velocity, Vector2.UP)
```

This script uses Godot's KinematicBody2D class to control the player's movement. Here is a step-by-step explanation of how the code works:

1. extends KinematicBody2D: This line indicates that the script extends the KinematicBody2D class, which is a built-in Godot class that provides movement and collision detection functionality for 2D objects.
2. const SPEED = 200: This line sets a constant variable SPEED to 200, which will be used to control the player's horizontal movement speed.
3. const GRAVITY = 1000: This line sets a constant variable GRAVITY to 1000, which will be used to control the player's vertical acceleration due to gravity.
4. const JUMP_FORCE = -500: This line sets a constant variable JUMP_FORCE to -500, which will be used to control the player's vertical velocity when jumping.
5. var velocity = Vector2(): This line declares a variable velocity as a Vector2, which will be used to store the player's current velocity.
6. func _physics_process(delta):: This line declares a function _physics_process that will be called every frame to update the player's physics.
7. var input_vector = Vector2(): This line declares a variable input_vector as a Vector2, which will be used to store the player's input direction.
8. input_vector.x = Input.get_action_strength("ui_right") - Input.get_action_strength("ui_left"): This line sets the x component of input_vector to the difference between the strength of the ui_right and ui_left input actions. This allows the player to move left and right using the arrow keys.
9. if is_on_floor():: This line checks if the player is currently touching the ground.
10. if Input.is_action_just_pressed("ui_up"):: This line checks if the player has just pressed the ui_up input action.
11. velocity.y = JUMP_FORCE: This line sets the y component of velocity to JUMP_FORCE, which causes the player to jump.
12. else: velocity.y += GRAVITY * delta: If the player is not on the ground, this line updates the y component of velocity to apply gravity to the player.
13. velocity.x = input_vector.x * SPEED: This line sets the x component of velocity to the product of input_vector.x and SPEED, which moves the player left or right based on the input.
14. velocity = move_and_slide(velocity, Vector2.UP): This line moves the player using the move_and_slide method, which takes the current velocity and a direction to slide against. In this case, the direction is Vector2.UP,"

Looks like GPT ran out of response tokens. There are a few things that are wrong with this code / concern me as a newbie:
1. GPT marks this code as 'Java' despite the fact that I asked explicitly for GDScript. I don't know Java or GDScript well enough to determine which language GPT is actually using.
2. I didn't explicitly say that the player object was a KinematicBody2D, which means GPT remembers that from previously in the conversation, but now it's gone and written a jump button! I don't need the spaceship to jump, or even have gravity applied. Maybe I should have a different kind of object instead of a KinematicBody2D, since I don't need it to have any special physics except collision interaction.

I'll start with removing the gravity and jump, then ask GPT if we should be using a different child node instead of KinematicBody2D.

**Q17.** The player object will not be affected by gravity, and does not need the ability to jump. Modify the code to remove the gravity and the ability to jump. Provide the code only, without an explanation.

**GPT's Response:** "
```
extends KinematicBody2D

const SPEED = 200

func _physics_process(delta):
    var motion = Vector2.ZERO
    if Input.is_action_pressed("ui_right"):
        motion.x += SPEED
    if Input.is_action_pressed("ui_left"):
        motion.x -= SPEED
    move_and_slide(motion)
```
"

I have no idea if this will work. Let's paste it into the PlayerController script and try it out.

Well, code me surprised, it works perfectly. I had to move the script from the Sprite to the KinematicBody2D object, but the code runs smooth. The arrow keys must be the default UI input, since the right arrow key is `Input.is_action_pressed("ui_right")`.

### Add Player Shooting

I had to go watch a video of Galaga to refresh my memory of the game. I wasn't sure if the player shots went straight up, or were affected by the player's movement.

Now the player should be able to shoot missiles at the enemy. I need to be aware of a few things:

1. The player should be able to spawn multiple missiles into the scene.
2. The player missile spawning should have a short cooldown (about 8 missiles fired per second)
3. The player missiles only go forward
4. If a player missile leaves the screen region, remove the missile from the scene (garbage collection)
5. The player should be able to hold down the spacebar to fire missiles continuously (rather than having to press the spacebar for every shot)

**Q18.** Modify the PlayerController script so that the player fires a missile if the spacebar is pressed. Explain in no more than 500 words how the new code works.

**GPT's Response:** "To modify the PlayerController script to enable the player to fire missiles when the spacebar is pressed, we need to first create a new Missile scene, add a missile sprite, and create a MissileController script that defines the behavior of the missile. Once we have these resources, we can modify the PlayerController script to create and launch a new missile every time the spacebar is pressed.

Here are the steps to achieve this:

1. Create a new scene for the Missile. To do this, right-click on the Scenes folder in the FileSystem dock, select New Scene, and name it "Missile."
2. In the new Missile scene, add a Sprite node, and set its texture to the image of the missile sprite.
3. Create a new script called "MissileController.gd" and attach it to the Missile node. This script will define the behavior of the missile when it is launched.
4. In the MissileController script, define the _process() function, which will be called every frame. In this function, move the missile upwards at a fixed speed. For example:

```
extends Node2D

export var speed = 400

func _process(delta):
    position.y -= speed * delta
```

5. In the PlayerController script, add a new function called _input(). This function will be called every time there is input from the player. In this function, check if the spacebar is pressed, and if so, create a new Missile node and add it to the game. For example:

```
extends KinematicBody2D

var missile = preload("res://Missile.tscn")

const SPEED = 200
const GRAVITY = 0

func _input(event):
    if event is InputEventKey and event.scancode == KEY_SPACE and event.pressed:
        var m = missile.instance()
        m.position = position
        get_parent().add_child(m)
```

In this modified PlayerController script, we preload the Missile scene, and define a new _input() function that checks for input events. If the event is a spacebar press, we create a new Missile node using the preload() function, set its position to be the same as the player's position, and add it as a child of the game's root node.

By default, the missile will be created and launched every frame that the spacebar is held down. To limit the number of missiles that can be launched, we can add a delay between missile launches or limit the number of missiles that can be active at any given time. We can also add collision detection logic to detect when a missile hits an enemy or other game object.

In summary, to modify the PlayerController script to enable the player to fire missiles, we created a new scene for the Missile, added a Sprite node with a missile sprite, defined a MissileController script that moves the missile upwards, and modified the PlayerController script to create and launch a new Missile node when the spacebar is pressed."

I've made the changes. There were a few small modifications to make, like I had to delete the extra "extends" and "const SPEED", but the instructions worked. I did find a couple interesting bugs:
1. When the spacebar is held down, a single shot is fired, then a half-second delay, then missile gun go brrrr. With our current setup, missile gun should go brrr immediately.
2. If the spacebar is held down, and the player is firing missiles, the firing stops when the player changes direction.

Let's let GPT handle both of these bugs.

**Q19.** This is the current PlayerController script:

```
extends KinematicBody2D

const SPEED = 200

func _physics_process(delta):
	var motion = Vector2.ZERO
	if Input.is_action_pressed("ui_right"):
		motion.x += SPEED
	if Input.is_action_pressed("ui_left"):
		motion.x -= SPEED
	move_and_slide(motion)

var missile = preload("res://Missile.tscn")

func _input(event):
	if event is InputEventKey and event.scancode == KEY_SPACE and event.pressed:
		var m = missile.instance()
		m.position = position
		get_parent().add_child(m)
```

When the spacebar is pressed and held down, a single first shot is fired, followed by a short delay, then a missile is generated every frame. Modify the code so that there is no delay after the first shot, and explain your code modification in less than 200 words.

**GPT's Response:** "To remove the delay after the first shot when the spacebar is held down, the `_input` function can be modified to create missiles every frame while the spacebar is held down. This can be accomplished by checking if the spacebar is being held down instead of only checking if it has been pressed. Here is the modified code:

```
extends KinematicBody2D

const SPEED = 200

func _physics_process(delta):
	var motion = Vector2.ZERO
	if Input.is_action_pressed("ui_right"):
		motion.x += SPEED
	if Input.is_action_pressed("ui_left"):
		motion.x -= SPEED
	move_and_slide(motion)

var missile = preload("res://Missile.tscn")

func _input(event):
	if event is InputEventKey and event.scancode == KEY_SPACE:
		if event.pressed:
			var m = missile.instance()
			m.position = position
			get_parent().add_child(m)
```

By removing the `and event.pressed` condition from the if statement in the `_input` function, the code will create missiles every frame while the spacebar is being held down."

I copied and pasted the new code into the PlayerController. It did not fix the issue. I know GPT has a tendency to start hallucinating after only a few attempts to fix bugs, so I'll have to be careful with my prompts if I ask it to fix anything.

I think for now I'll just make sure that the player has to press the space button down for every shot, rather than try to incorporate multiple button presses at once. That still leaves the issue of having to create a short delay after every shot.

I wonder how GPT does with semicolons. Maybe I'm changing too many variables at once, but this is an experimental process.

**Q20.** Modify the PlayerController script so that the player must re-press the spacebar to fire a missile; the player cannot hold the spacebar down to continuously fire missiles. The missiles must have a 0.2 second cooldown; the player cannot fire another missile until 0.2 seconds after the last missile was fired, even if the player presses the spacebar again before the delay time has passed.

**GPT's Response:** "Here is the modified PlayerController script:

```
extends KinematicBody2D

const SPEED = 200
const MISSILE_COOLDOWN = 0.2

var missile = preload("res://Missile.tscn")
var missile_timer = 0.0

func _physics_process(delta):
	var motion = Vector2.ZERO
	if Input.is_action_pressed("ui_right"):
		motion.x += SPEED
	if Input.is_action_pressed("ui_left"):
		motion.x -= SPEED
	move_and_slide(motion)

	# decrease the missile timer each frame
	if missile_timer > 0:
		missile_timer -= delta

func _input(event):
	if event is InputEventKey and event.scancode == KEY_SPACE and event.pressed and missile_timer <= 0:
		var m = missile.instance()
		m.position = position
		get_parent().add_child(m)
		# reset missile timer
		missile_timer = MISSILE_COOLDOWN
```

In the modified code, we introduced a missile_timer variable which keeps track of the cooldown time after the last missile was fired. The missile timer is decreased every frame in the _physics_process() function. In the _input() function, we check if the spacebar is pressed, and if the missile timer is less than or equal to 0. If the conditions are met, a new missile instance is created and added to the game world, the missile position is set to the player's position, and the missile timer is reset to the MISSILE_COOLDOWN value. This ensures that the player cannot fire another missile until the cooldown period has passed."

The cooldown works, but the hold-spacebar still works, too. Maybe I'll try to keep that, because it seems more in line with the original game.

The PlayerController script is already pretty janky, having to deal with two different types of input (both the physics process using delta and the input event) so I'm wondering if I can get GPT to combine everything. Since we have so few buttons to use (three keys in total) I think I'll try to get it to operate conditionally on if each key is pressed, rather than on an "input event" basis.

I expect GPT's hallucinations to worsen if I continue to have it modify the current PlayerController script. I'll have it write a new script, but loosely reference the original PlayerController script in the new script's creation, and see what GPT does.

**Q21.** The current PlayerController script fails to consider some instances with multiple inputs. Write a new PlayerController script called PlayerControllerMult that has independent conditional execution for the right arrow key, left arrow key, and spacebar.

**GPT's Response:** "Here's an example of the PlayerControllerMult script that allows for independent conditional execution of the right arrow key, left arrow key, and spacebar:

```
extends KinematicBody2D

const SPEED = 200
var missile_cooldown = 0.0
var missile_delay = 0.2
var missile = preload("res://Missile.tscn")

func _physics_process(delta):
	var motion = Vector2.ZERO
	if Input.is_action_pressed("ui_right"):
		motion.x += SPEED
		move_and_slide(motion)
	if Input.is_action_pressed("ui_left"):
		motion.x -= SPEED
		move_and_slide(motion)
	
	if missile_cooldown > 0.0:
		missile_cooldown -= delta
	
	if Input.is_action_pressed("ui_fire") and missile_cooldown <= 0.0:
		var m = missile.instance()
		m.position = position
		get_parent().add_child(m)
		missile_cooldown = missile_delay
```

In this modified script, each input event is handled separately. The right arrow key and left arrow key movements are handled independently in the same way as the previous script. The missile firing is now handled by a separate conditional statement that checks whether the missile cooldown time has expired. If the spacebar is pressed and the missile cooldown is less than or equal to 0.0, then a missile is fired, and the missile cooldown time is set to the missile delay time. This ensures that the player can only fire missiles once every 0.2 seconds."

Now the ship doesn't even fire. Back to the previous code.

Another interesting result: GPT tried to copy the original PlayerController script into PlayerControllerMult with the desired modifications. I'll ask it to completely forget the current code in the PlayerControllerMult, and have it create a template that allows for multiple inputs.

**Q22.** Remove the _physics_process function from the PlayerControllerMult script. Write the rest of the PlayerControllerMult script as a template that moves the player in the direction of the most recent left or right arrow press, and executes the spacebar action independently of the left or right arrow presses.

**GPT's Response**: "
```
extends KinematicBody2D

const SPEED = 200
var motion = Vector2.ZERO

var missile = preload("res://Missile.tscn")
var last_shot_time = 0
const COOLDOWN = 0.2

func _input(event):
	if event is InputEventKey:
		if event.scancode == KEY_SPACE and event.pressed and (OS.get_ticks_msec() - last_shot_time) > COOLDOWN * 1000:
			var m = missile.instance()
			m.position = position
			get_parent().add_child(m)
			last_shot_time = OS.get_ticks_msec()
		elif event.scancode == KEY_RIGHT:
			if event.pressed:
				motion.x += SPEED
			else:
				motion.x -= SPEED
		elif event.scancode == KEY_LEFT:
			if event.pressed:
				motion.x -= SPEED
			else:
				motion.x += SPEED
				
	move_and_slide(motion)
```

In this modified script, the _physics_process function has been removed and replaced with a _input function. The _input function handles all user input, including the arrow key presses and spacebar presses. The motion variable is now defined outside of any function so that its value can be updated based on the most recent arrow key press. The missile and last_shot_time variables are also defined outside of any function so that they can be used in both the _input and _physics_process functions. When the spacebar is pressed and the cooldown time has passed since the last shot, a new missile instance is created and added to the parent node. The arrow key presses update the motion variable in the appropriate direction. Finally, the move_and_slide function is called to update the player's position based on the motion variable."

Now it's *really* janky. The sprite is moving even when I'm not pressing any buttons!

Sometimes, what's needed is a fresh set of eyes. In this case, that fresh set of eyes will also be GPT!

Now that I've narrowed what I'm doing, I'm going to redefine the initial prompt. Then, I'll tell GPT what I'm doing, where I am in the project, provide it the code, and ask for advice on how to fix my code.

(Initial Prompt) **Q1.** You will act as a video game developer and designer with more than 30 years of experience. You have developed games using all prebuilt game engines, like Unreal Engine and Godot; you have even developed custom game engines yourself. You have created games for triple-A companies, small indie developers, and everything in between. You have an extensive knowledge of how games are designed and developed, how a developer chooses which game engine to use for their project, what makes games engaging, and how to plan out the development process. <br>
I am a game development novice, and you will be my teacher. I will ask you questions and make requests. My questions will be about video game design and development, and my requests will be for code snippets. Your responses should be clear and concise, and written at an eighth-grade reading level. Your responses should be tailored to assume that I have very little knowledge of game design and development, but I do have a background in data science and some coding / programming experience in Python. <br>
If you do not understand my question, or it is too vague, you will ask clarifying questions until you understand my request. <br>
We are working on recreating the arcade game Galaga using the Godot game engine. You will provide any code snippets in GDScript. <br> 
If you understand, summarize our respective roles, and ask for my first question or request.

**GPT2's Response:** "As a video game developer and designer with more than 30 years of experience, my role is to assist you, a game development novice, in understanding the process of video game design and development, and to help you recreate the arcade game Galaga using the Godot game engine. You can ask me any questions related to video game design and development or make requests for code snippets in GDScript.

What is your first question or request?"

**Q2.** I am currently working on a PlayerController script for the recreation of Galaga. Write a PlayerController script in GDScript such that the following is true: <br>
The PlayerController script is a child of a KinematicBody2D node. <br>
The player is able to move left and right using the left and right arrow keys, respectively, and is also able to fire missiles using the spacebar. The missile object can be referenced as "Missile.tscn". <br>
The script is able to handle multiple inputs simultaneously. For left and right movement, the player moves in the direction of the most recently pressed or held input, even if the opposite direction's button continues to be held down from a previous press. For example, if the player pushes and holds the right arrow and moves right, then presses and holds the left arrow button while continuing to hold down the right arrow button, the player moves left, and when the left arrow button is then released while continuing to hold down the right arrow button, the player then moves right. <br>
The spacebar input operates independently of the directional movement; if the spacebar is pressed and held down, the ship continues to fire missiles regardless of any right and left arrow button presses or releases. Additionally, missiles should have a 0.2 second delay between firing, even if the spacebar is held down or pressed again within the delay window.

**GPT2's Response:** "Here is an example of a PlayerController script in GDScript that satisfies the requirements you mentioned:

```
extends KinematicBody2D

const SPEED = 400
const FIRE_DELAY = 0.2
var fire_timer = 0.0

func _physics_process(delta):
    var velocity = Vector2.ZERO
    if Input.is_action_pressed("ui_right"):
        velocity.x += 1
    if Input.is_action_pressed("ui_left"):
        velocity.x -= 1
    velocity = velocity.normalized() * SPEED
    move_and_slide(velocity)

    fire_timer -= delta
    if Input.is_action_pressed("ui_space"):
        if fire_timer <= 0.0:
            var missile = load("res://Missile.tscn").instance()
            missile.position = position
            get_parent().add_child(missile)
            fire_timer = FIRE_DELAY
```

Here's how the script works:

- The extends KinematicBody2D line indicates that this script is a child of a KinematicBody2D node.
- SPEED is a constant value that determines the speed of the player's movement.
- FIRE_DELAY is a constant value that determines the delay between missile firings.
- fire_timer keeps track of the time since the last missile was fired.
- _physics_process(delta) is a function that is called once per frame, where delta is the time since the last frame. Inside this function:
- The velocity vector is set based on the input from the left and right arrow keys, and the SPEED constant.
- The move_and_slide function moves the player according to the velocity vector.
- The fire_timer is decremented by delta.
- If the spacebar is pressed and the fire_timer has elapsed, a new missile object is created, positioned at the player's position, added as a child of the parent node, and the fire_timer is reset to FIRE_DELAY.

The script uses move_and_slide to handle the movement of the player, which ensures that the player will move correctly even when colliding with other objects. The script also uses the delta value to ensure that missile firing is consistent across different frame rates.

I hope this helps you with your project!"

This is definitely cleaner. The movement system doesn't work exactly as defined (the ship doesn't move at all if both left and right arrow buttons are held) but it's fine for now. The problem is that the ship won't fire again! I'm seeing a lot of errors appearing in Godot. I'll ask what causes them.

**Q3.** The code you provided has the following errors when the game is run:
1. "The function 'move_and_slide()' returns a value, but this value is never used."
2. "is_action_pressed: Request for nonexistent InputMap action 'ui_space'.

Explain what causes these errors and how to eliminate them.

**GPT2's Response:** "I apologize for those errors in the code. Here is the corrected code with explanations:

```
extends KinematicBody2D

const SPEED = 400
const FIRE_DELAY = 0.2
var fire_timer = 0.0

func _physics_process(delta):
    var velocity = Vector2.ZERO
    if Input.is_action_pressed("ui_right"):
        velocity.x += 1
    if Input.is_action_pressed("ui_left"):
        velocity.x -= 1
    velocity = velocity.normalized() * SPEED
    move_and_slide(velocity)

    fire_timer -= delta
    if Input.is_action_pressed("ui_spacebar"):
        if fire_timer <= 0.0:
            var missile = load("res://Missile.tscn").instance()
            missile.position = position
            get_parent().add_child(missile)
            fire_timer = FIRE_DELAY
```
Explanation:

The `move_and_slide()` function returns a Vector2 value representing the player's final velocity after applying movement and collision. This returned value can be used for advanced collision handling, but is not necessary in this example. To fix the error message, simply remove the returned value like this:

```
move_and_slide(velocity)
```
The `is_action_pressed()` function checks if an InputMap action is currently active. The original code used the non-existent InputMap action 'ui_space', which caused the error message. To fix the error message, change the argument to "ui_spacebar" like this:

```
if Input.is_action_pressed("ui_spacebar"):
```
This should eliminate both error messages and allow the code to run as intended. Let me know if you have any further questions."

I already know that this is going to cause another error, since the previous GPT already tried to use "ui_spacebar" with no success. I'll try it anyway to confirm.

Just as I predicted. More errors. I'll give GPT2 another try at solving the problem itself, but if that fails, I'm going to ask it how to go into my Godot project settings and map the spacebar to one of the recommended inputs.

**Q4.** The code you provided has the following error when the game is run: "is_action_pressed: Request for nonexistent InputMap action 'ui_spacebar'." Explain what causes this error and how to eliminate it.

**GPT2's Response:** "I apologize for the error in my previous response. The correct InputMap action for the spacebar is simply "ui_space", not "ui_spacebar". 

ETC..."

GPT2 is going in circles! It doesn't even remember that it already tried "ui_space". Oh well, I'll just move forward with plan B.

**Q5.** Give a step-by-step explanation of how to map the spacebar to "ui_space" in my Godot project.

**GPT2's Response:** "Sure! Here is a step-by-step guide on how to map the spacebar to "ui_space" in your Godot project:

1. Open your Godot project and select "Project Settings" from the "Project" menu.
2. In the "Input Map" tab, scroll down to the "UI" section and click the "+" button to add a new action.
3. In the "Add Action" dialog that appears, enter "ui_space" as the name for the new action, and click "Add".
4. Select the newly added "ui_space" action in the list, and click the "+" button next to the "Keys" property.
5. In the "Add Input Event" dialog that appears, press the spacebar on your keyboard to map it to the "ui_space" action. The key should appear in the "Keys" property.
6. Click "Close" to close the "Add Input Event" dialog.
7. Click "Save" to save the changes to the Input Map.

Once you have completed these steps, the spacebar should be mapped to the "ui_space" action in your Godot project, and you should be able to use it in your scripts as shown in the previous example."

I made the recommended changes (I had to add "ui_space" to the Input Map) and it all works like a charm!

The only thing I would personally change about the PlayerController script was written previously by the first iteration of GPT, which is to preload the missile scene rather than loading it every time.

Maybe the fire delay, too. It seems too long compared to the original game.

Here's the new, improved, as-clean-as-can-be (kappa) PlayerController:

```
extends KinematicBody2D

# define constants
const SPEED = 200
const FIRE_DELAY = 0.12
var fire_timer = 0.0
var preloaded_missile = preload("res://Missile.tscn")

func _physics_process(delta):
	# left and right movement
	var velocity = Vector2.ZERO
	if Input.is_action_pressed("ui_right"):
		velocity.x += 1
	if Input.is_action_pressed("ui_left"):
		velocity.x -= 1
	velocity = velocity.normalized() * SPEED
	move_and_slide(velocity)
	
	# fire missile if button pressed and off cooldown
	fire_timer -= delta
	if Input.is_action_pressed("ui_space"):
		if fire_timer <= 0.0:
			var missile = preloaded_missile.instance()
			missile.position = position
			get_parent().add_child(missile)
			fire_timer = FIRE_DELAY
```

### Creating the Game Window

In the future, when prettying up the game, I'll need to create an animated background with glittering stars that moves down in an endless loop. Or maybe I'll just do a particle effect... For now, I'll just keep a black background, but I still need to set the size of the window. My spaceship is tiny in the current window, and moves too quickly.

I don't think I need the first iteration of GPT anymore. I'll stick with GPT2 for now.

**Q6.** This is the new PlayerController script. 

[I Included the new script here]

If you understand, compare this new code to the previous code written and summarize the differences in a few sentences.

**GPT's Response:** "Yes, I understand. Here are the differences between the new code and the previous code:

1. The constant value for the missile firing delay has been changed from 0.2 seconds to 0.12 seconds.
2. A variable "fire_timer" has been added to keep track of the time since the player last fired a missile.
3. The "fire_timer" variable is decremented by the delta time in each frame to keep track of the time since the last missile was fired.
4. The code that fires the missile has been modified to only execute if the "fire_timer" has expired, preventing the player from firing multiple missiles in quick succession.
5. The reference to the "Missile.tscn" scene has been preloaded and stored in a variable "preloaded_missile" for improved performance.

Overall, these changes improve the gameplay experience by preventing the player from spamming missiles and making the firing more responsive with a shorter delay between each shot."

I wasn't going to include this prompt in the journal, but I found the response interesting because:
1. Only 1 and 5 are actual differences.
2. I only asked it to summarize in a few sentences, but it instead created a numbered list of the differences, and *then* provided a summary of the differences.

**Q7.** The default Godot game window is too large, and the default background is the wrong color. Explain step-by-step how to change the size of the game window and set the background color to black.

**GPT's Response:** "Sure, here's a step-by-step guide on how to change the size of the game window and set the background color to black in Godot:

1. Open your project in Godot and click on the "Project Settings" button at the top of the screen.
2. In the "Project Settings" window, click on the "Display" tab on the left-hand side.
3. Under the "Window" section, change the "Width" and "Height" values to your desired size. For example, you can set the width to 800 and the height to 600.
4. Under the "Stretch" section, change the "Mode" value to "2d".
5. Under the "Viewport" section, change the "Background" color to black. You can either enter the color code (#000000) or use the color picker to select black.
6. Click the "Save" button to save your changes.

Once you've made these changes, the game window will be resized to your desired dimensions, and the background color will be black."

For the most part, GPT was correct. "Viewport" was actually "Environment" but close enough.

I've made a handful of small modifications to the scripts again, just making small adjustments to the player and missile speed. I have a tendency to get stuck on the small stuff but I definitely wanted to get the player movement and fire rate nailed down because of how crucial the input is to the playability of the game.

### Creating Enemies

This one's going to be a doozy, I just know it. We need enemy sprites, animations, and collisions for the simple enemies, to say nothing of the enemies that fire missiles (or the abduction enemies!)

First, I'll see what GPT thinks about how we should implement enemies.


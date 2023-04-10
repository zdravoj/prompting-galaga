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

Now I have a sprite sheet downloaded locally. It has a bunch of 8-bit images of the Galaca sprites. No idea how to use it properly.
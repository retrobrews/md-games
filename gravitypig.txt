Gravity Pig - A simple platformer for the Genesis.

Most info can be found within the game, but you can also E-mail me at ComradeOj@yahoo.com if you have other questions.

It is Highly recommended that you don't run the game in FUSION or GENS! 
Those two emulators don't emulate the VDP's sprite collision detection quite right, and it will cause the final boss 
stage to constantly steal lives from you, even if you don't get it. 
It works fine in the REGEN emulator, or on real hardware via a flash cart.

You may freely distribute and play the game, but not for commercial use.

(C)2015 ComradeOj


It is Highly recommended that you don't run the game in FUSION or GENS! Those two emulators don't emulate the VDP's 
sprite collision detection quite right, and it will cause the final boss stage to constantly steal lives from you, 
even if you don't get it. It works fine in the REGEN emulator, or on real hardware via a flash cart.

What is Gravity Pig?
It's a simple platformer game, with (very) light puzzle elements but without jumping. Instead, you must get around 
by reversing gravity. I have showed it to a few people, and one compared it to VVVVVV. I've never actually played 
that game, but I watched a video of it and I could see the similarity. Gravity Pig was actually inspired by a 
flash game called This Is The Only Level. The gravity flip mechanic was used because it was easier to program than jumping.

There are 3 different themed areas, each with 5 stages. That's not whole lot of levels, especially considering their 
small size. It was a lot harder to come up with challenging stages than you might imagine. I didn't want to re-hash 
too many obstacles or ideas, so I was only able to come up with 15.

How is it played?
You make your way through the levels to reach the goal post at the end. Along the way, you can collect extra lives, 
coins, and extra "Gswaps". You can only switch gravity a limited number of times, and a "Gswap" icon lets you do it 
an additional time. The game is what I call a "semi-scroller". The levels do scroll left and right, but not very far. 
You will be moving right about as often as you move left.
The Genesis resolution is 320x224, and the levels are all 512x224. So, the levels can scroll 96 pixels in either direction.

The story
There is a simple story but it's only about as deep as the plot of sonic 1. An evil mystic kidnapped all the pigs, 
and you have to journey to her lair to confront her and free the pigs.

Development diaries
One challenge was creating levels out of tiles that could be used for collision. I could draw a static image that 
looked like a stage, but the game's engine would have no way of working out collision properties. So, I figured 
out a way of using the same chunk of data for design, art cues, and collision. The level data is basically a chunk 
of text with each letter corresponding to a different type of block. This chunk of text is loaded into VRAM to 
display the graphics, and RAM for the engine to probe sections of the stage and determine collision.
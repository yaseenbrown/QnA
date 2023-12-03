1. - They are all 2d vectors made in Affinity Designer then imported into Blender and turned into grease pencil objects. But they are 2d objects stacked so like 2.5D I guess.

-also they not all controlled by lattices, some parts like the eyes and eyebrows are just parented to a bone and but they all have a 2nd lattice on that moves everything at once to add a secondary layer of animation on top of everything


![1](https://github.com/yaseenbrown/QnA/assets/38442534/ae4bb3f3-4199-4a7b-9222-f81a08f43b25)


2: I make the shadows by create a large “shadow” object then inside the grease pencil object as the  face and just mask it with in face layer.


Then I parent just the shadow layer to the to the lattice that controls the hair and the lattice that controls the face. 


that way when every I move the hair lattice the shadow moves with it making to look like a cast shadow without worrying about lighting and also generated shadows dont have the same fidelity as 2d ones so I can keep the whole thing sharp. 





No- the outlines are done one of two ways, the first and most common is just the “stroke” effect in photoshop, since I have convert the renders into gifs in photoshop anyway. 
The other way I do it is using the compositor using this nodes




The eyes are just grease pencil layers and using the grease pencil masking feature.

the inside of the eye and the white eyeball are to assigned to 2 different vertex groups and attached to the armature to make it move, the masking feature does the rest.


The blinking is something I dont want to animated everytime so what did was make the shape keys for the 2 lattices the control the eyes, one for the eyeball and one for the eyelash, you can see they very messy but blinking is so fast it doesnt matter, its just 3 shape keys that I animated the value froms 1 to 0 everytime I want to blink  and its not connected to the armature at all so I can animate the whole emote then add blinking whenever I want.



Pretty much, the but the bendy bones control the lattices that control the hair. You dont have to use lattices for this and skin the hair directly to the bendy bones but I was learning lattices and it just became put of the process.

What I also then do is use a lattice on all the other lattices so I can control the whole rig with a separate armature to add squash and stretch to the whole model. 



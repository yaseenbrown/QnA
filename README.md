1. - They are all 2d vectors made in Affinity Designer then imported into Blender and turned into grease pencil objects. But they are 2d objects stacked so like 2.5D I guess.
![1](https://github.com/yaseenbrown/QnA/assets/38442534/bb1b2283-6896-414f-84c7-ac1880f2f23f)

-also they not all controlled by lattices, some parts like the eyes and eyebrows are just parented to a bone and but they all have a 2nd lattice on that moves everything at once to add a secondary layer of animation on top of everything

![2](https://github.com/yaseenbrown/QnA/assets/38442534/172c31b1-ac98-4979-8e64-7d47b7133e11)



---
2 .  I make the shadows by create a large “shadow” object then inside the grease pencil object as the  face and just mask it with in face layer.

   ![3](https://github.com/yaseenbrown/QnA/assets/38442534/277cc295-b558-496b-8a62-582750f76876)
   
   
   Then I parent just the shadow layer to the to the lattice that controls the hair and the lattice that controls the face.
   
   ![4](https://github.com/yaseenbrown/QnA/assets/38442534/4b6bd0a0-6743-4eb5-9619-fbf4de3b8b3e)
   
   
   that way when every I move the hair lattice the shadow moves with it making to look like a cast shadow without worrying about lighting and also generated shadows dont have the same fidelity as 2d ones so I can keep the whole thing sharp.
   ![5](https://github.com/yaseenbrown/QnA/assets/38442534/fa3d612c-2dda-4797-bd23-0274ab3403cf)
   
   
   Its really just a seperate shadow object with about a 50% opacity and now a projected shadow from a source of light.
   
   ![6](https://github.com/yaseenbrown/QnA/assets/38442534/c7f15831-0177-4186-b96a-3218dab3916e)




---
3. No- the outlines are done one of two ways, the first and most common is just the “stroke” effect in photoshop, since I have convert the renders into gifs in photoshop anyway. 

   The other way I do it is using the compositor using this nodes
   ![7](https://github.com/yaseenbrown/QnA/assets/38442534/32b6e880-7377-46da-a86f-d0f403ca6226)



---

4. The eyes are just grease pencil layers and using the grease pencil masking feature.
   
   ![8](https://github.com/yaseenbrown/QnA/assets/38442534/a5188304-b307-4c4d-a629-13f5cd9e24b8)
   
   the inside of the eye and the white eyeball are to assigned to 2 different vertex groups and attached to the armature to make it move, the masking feature does the rest.
   
   ![9](https://github.com/yaseenbrown/QnA/assets/38442534/29e28f54-c4dd-489f-a678-ad5b5795c0a0)
   
   
   The blinking is something I dont want to animated everytime so what did was make the shape keys for the 2 lattices the control the eyes, one for the eyeball and one for the eyelash, you can see they very messy but blinking is so fast it doesnt matter, its just 3 shape keys that I animated the value froms 1 to 0 everytime I want to blink  and its not connected to the armature at all so I can animate the whole emote then add blinking whenever I want.
   
   ![12](https://github.com/yaseenbrown/QnA/assets/38442534/1bef15f5-d7a1-4576-a52e-93b60218e4d7)
   ![11](https://github.com/yaseenbrown/QnA/assets/38442534/959fd0f1-cd87-45be-b547-424989d1d5d9)
   ![10](https://github.com/yaseenbrown/QnA/assets/38442534/f8f56218-af2e-4659-a89a-eae5459b5446)


---

5. Pretty much, the but the bendy bones control the lattices that control the hair. You dont have to use lattices for this and skin the hair directly to the bendy bones but I was learning lattices and it just became put of the process.
   ![13](https://github.com/yaseenbrown/QnA/assets/38442534/8b9354df-b427-43c8-b57b-e27dc290594b)
   they
  
   What I also then do is use a lattice on all the other lattices so I can control the whole rig with a separate armature to add squash and stretch to the whole model. 
   ![14](https://github.com/yaseenbrown/QnA/assets/38442534/204bcc5b-0ebb-4073-b6a7-868d0080c601)




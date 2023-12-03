1. - They are all 2d vectors made in Affinity Designer then imported into Blender and turned into grease pencil objects. But they are 2d objects stacked so like 2.5D I guess.
![1](https://github.com/yaseenbrown/QnA/assets/38442534/ae4bb3f3-4199-4a7b-9222-f81a08f43b25)
-also they not all controlled by lattices, some parts like the eyes and eyebrows are just parented to a bone and but they all have a 2nd lattice on that moves everything at once to add a secondary layer of animation on top of everything

![Untitled](https://github.com/yaseenbrown/QnA/assets/38442534/c1a37808-a834-4e1b-871b-a194bf3ffb0b)


---
2 .  I make the shadows by create a large “shadow” object then inside the grease pencil object as the  face and just mask it with in face layer.

![2](https://github.com/yaseenbrown/QnA/assets/38442534/0fe306e9-997a-48c5-83eb-1fd4233cdeb3)

Then I parent just the shadow layer to the to the lattice that controls the hair and the lattice that controls the face.

![3](https://github.com/yaseenbrown/QnA/assets/38442534/6e5556e0-2987-430d-a2ac-98d676adc3bd)

that way when every I move the hair lattice the shadow moves with it making to look like a cast shadow without worrying about lighting and also generated shadows dont have the same fidelity as 2d ones so I can keep the whole thing sharp.

![4](https://github.com/yaseenbrown/QnA/assets/38442534/a2fc7d72-3f2b-4541-ba6a-170fa6b0e2eb)
Its really just a seperate shadow object with about a 50% opacity and now a projected shadow from a source of light.

![5](https://github.com/yaseenbrown/QnA/assets/38442534/0079a753-1de1-4cc6-a35b-cb406db26c72)



---
3. No- the outlines are done one of two ways, the first and most common is just the “stroke” effect in photoshop, since I have convert the renders into gifs in photoshop anyway. 

The other way I do it is using the compositor using this nodes

![6](https://github.com/yaseenbrown/QnA/assets/38442534/6517e801-ad47-48c8-b993-70fa805fc35a)

---

4. The eyes are just grease pencil layers and using the grease pencil masking feature.
   
![7](https://github.com/yaseenbrown/QnA/assets/38442534/a5dc5f1b-bfad-4e0b-8d41-0a129f7bd7d9)

the inside of the eye and the white eyeball are to assigned to 2 different vertex groups and attached to the armature to make it move, the masking feature does the rest.

![8](https://github.com/yaseenbrown/QnA/assets/38442534/887050e1-1e9d-4b96-9cbd-0c0864efee31)


The blinking is something I dont want to animated everytime so what did was make the shape keys for the 2 lattices the control the eyes, one for the eyeball and one for the eyelash, you can see they very messy but blinking is so fast it doesnt matter, its just 3 shape keys that I animated the value froms 1 to 0 everytime I want to blink  and its not connected to the armature at all so I can animate the whole emote then add blinking whenever I want.

![9](https://github.com/yaseenbrown/QnA/assets/38442534/15165efc-2d8f-4462-a55e-38d0bcf9e543)
![10](https://github.com/yaseenbrown/QnA/assets/38442534/8745c897-7c2d-40f8-b228-ab5f56bfb4ad)
![11](https://github.com/yaseenbrown/QnA/assets/38442534/f1a7eed2-30d1-4d27-9bb4-756ba02af1b2)

---

5. Pretty much, the but the bendy bones control the lattices that control the hair. You dont have to use lattices for this and skin the hair directly to the bendy bones but I was learning lattices and it just became put of the process.
   
![12](https://github.com/yaseenbrown/QnA/assets/38442534/a4ae8ae1-89f9-42cb-9560-16166405b4d1)


What I also then do is use a lattice on all the other lattices so I can control the whole rig with a separate armature to add squash and stretch to the whole model. 
![13](https://github.com/yaseenbrown/QnA/assets/38442534/50d9ba7c-1ac3-43b6-9bf8-59629febdd01)



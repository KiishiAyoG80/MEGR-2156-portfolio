# A8 – Gear Box

## Objective

For this assignment, I created a gearbox and modeled it with Solidworks. The assignment gives the gear ratio, rotational speed, and output torque of the gearbox. I used parametric design to create my gearbox and casing.


## Analyze

Shaft Design: 

I started with designing the shafts using equations from the Handbook. There were just enough given values to solve for everything.
<img width="591" height="632" alt="image" src="https://github.com/user-attachments/assets/046358bc-6442-499b-b32a-4f8a5f47ac71" />

 Journal Bearing:

In this section I designed the journal bearing. Ultimately, I was trying to find the PV value which I would use to find a suitable material and thickness. 
<img width="582" height="687" alt="image" src="https://github.com/user-attachments/assets/f3d57b81-ead8-44f5-b951-ed1daf425ea5" />
<img width="582" height="292" alt="image" src="https://github.com/user-attachments/assets/3939ce89-4cc2-4ff4-92b3-9d086ec72cd0" />

 Sketches:

My sketch wasn’t completely accurate to the final design so I used it as there were small changes here. I did continue to go with a design that had a hollow interior with a flange surrounding it with screwholes.

Solidworks:

The first parts that I designed were the shafts. I had already known what the shaft diameters should be but before I began modelling I went ahead and downloaded the two McMaster-Carr gears to sanity check my dimensions. For either of the shafts, I began with creating a circle that would be extruded and then a slight chamfer added to the end.

Output Shaft:

<img width="512" height="490" alt="image" src="https://github.com/user-attachments/assets/c7f1f866-de13-4ca4-a381-1034cdfdc7c5" />

Input Shaft: 

<img width="420" height="497" alt="image" src="https://github.com/user-attachments/assets/263f1f68-81cd-44b1-8e39-a1252415abac" />

Then I started to work on my Journal Bearing. I made this part completely parametrically. I started by filling out all of the Global Variables I would need. I then sketched a circle with another circle inscribed in it. I used the equation for diameter plus thickness where I took the diameter and added two times the thickness to achieve the diameter of the part. I then extruded the part to a length "L" and set the thickness to "th" which was defined.

<img width="585" height="631" alt="image" src="https://github.com/user-attachments/assets/4a8dbd6d-e4a1-4622-adc2-0ae2e446b812" />

My final step before I assembled was to create the actual housing for the gearbox. I began by sketching a rectangle and extruding it to create a solid block. I then used the shell tool to obtain a cutout in the center where I could house the gears. I then started a new drawing in the housing where I created centerlines. I used centerlines because I had already calculated the distance from the center for both gears. I then applied construction lines that represented where the actual gears would be, this was a sanity check to ensure that the gears would actually fit inside of the housing. I then for the other side of the case, copied the case to another part file and changed the hole size. This was only possible because of the symmetry of the casing. I also added #2 Flathead screw holes. There was no specific design intent with this other than the outer diameter of the screw fitting nicely.

<img width="467" height="687" alt="image" src="https://github.com/user-attachments/assets/e3fc1f05-ca90-4e36-b13c-059d80887cbf" />


## Decide

Assembly:

I started to import my parts into an assembly in Solidworks. I began with the shafts and gears. I simulated press fitting the shafts into the gear holes. I then added the back of the case which is the part attached to the output of the gearbox. I mated the output shaft with the hole I created in this box. I then imported the form of the housing and did the same with the input shaft. I then added a gear mate to both of the gears, allowing them to be manually turned by the user. Additionally, I made the front of the housing transparent just to see the mechanism inside clearly.

<img width="520" height="685" alt="image" src="https://github.com/user-attachments/assets/8d15d8fc-2b5a-4ab7-adfa-0e318a1d676b" />


## Communicate

Lessons Learned:

This was the most difficult assignment for me so far whether it came from the initial calculations or the assembly and there were plenty of lessons learned. I believe the most important lesson was that I need to work on assemblies much more. I have been in University for two years and I have never truly had to do much with assemblies other than two other assignments and it really showed here. I am going to dedicate time to truly learning and understanding the ins and outs of assemblies because I spent a large chunk of my time figuring out what I can and can't do.

This assignment took me 9 hours to complete.

Download links:

[Output Shaft:](https://instructure.charlotte.edu/eportfolios/5064/entries/37232/files/nWH4scps4F3SqoGyH74KpHpEJAlMwH5C5T4P83J1)

[Input Shaft:](https://instructure.charlotte.edu/eportfolios/5064/entries/37232/files/6GHXH5CBgjy1EQTKMoQ7ndab6cl2IVUOMhQQRYSN)

[Journal Bearing:](https://instructure.charlotte.edu/eportfolios/5064/entries/37232/files/RO53QHkK8nUYsgo07C4F60RuNCBzfOVincGt5rtL)

[Casing part:](https://instructure.charlotte.edu/eportfolios/5064/entries/37232/files/5eosI2yui9MNSfZtnH0oq7rryDe23eSJjjNI0Jmz)

[Final Assembly:](https://instructure.charlotte.edu/eportfolios/5064/entries/37232/files/zLPpCjfCeOWxUc7a6N2SCXzvmY6fIQTXiC7ZpV5r)



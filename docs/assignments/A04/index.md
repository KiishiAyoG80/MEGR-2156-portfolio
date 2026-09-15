# A4 – Motor Mount

## Purpose

The purpose of this lab is to design and analyze a motor mount that attaches to a 24B DC hear motor to rigid wall A while supporting an applied shaft load of 300 N. The mount is designed using beam-bending equations to find the required cross-sectional geometry based on yield strength and a maximum allowable free-end deflection of 0.30mm. The final design will have features such as gussets, clearance holes and appropriate mounting geometry to minimize deflection and provide adequate structral support.

<img width="123" height="99" alt="image" src="https://github.com/user-attachments/assets/6e8d9d1f-0173-4699-a4ae-a901c1484fc8" />


## Feature 1- Motor attachment arm

This feature is part of the motor's mount and connects to the motor directly while carrying the applied load the shaft. It is also treated like a cantilever beam fixed at the wall.

Known values include the applied force, safety factor, and the assumed length of the feature. The unknown values were the cross-sectional dimension to satisfy the strength and deflection requirements. I created a free-body diagram to find the shear force and bending moment caused by the applied load

The beam bending equations were used to determine the maximum bending stress and the deflection requirement at the end of the fixed beam. I used these equations to find the required dimensions afterwards. Since the stress requirement is less than the deflection requirement, deflection governed the final design of Feature 1. However, both stress and deflection constraints are satisfied by the geometry that I chose.

<img width="540" height="733" alt="image" src="https://github.com/user-attachments/assets/d16bd24d-9a83-4f7c-917f-1fee8946b1c8" />

<img width="508" height="712" alt="image" src="https://github.com/user-attachments/assets/b7d23a50-8215-4aa5-8e95-6abc1575eaa6" />

## Feature 2- Wall attachment arm

This feature represent the section of the mount that attaches to the wall and takes the applied load and put it towards the bolted connections. It was also analyzed with the same bending approach as feature 1, with the wall the fixed surface that connects to the beam.

My know values are the applied load, safety factor, and the properties of the beam. Another know value is the values in feature 1 but they were not relevant to this calculation process. I chose the length of Feature 2 based the motor's body length and the added tolerance to make sure the motor runs smoothly.

I made a free-body diagram to find the bending moment acting on feature 2. I used the same beam-bending equations from feature 1 to find the stress and deflection requirements of feature 2. Like Feature 1, deflection controlled the final design because the value I calculated was larger than the strength requirement value. These dimensions provide enough stability and strength to support the load.

<img width="556" height="735" alt="image" src="https://github.com/user-attachments/assets/c855024f-790b-40a4-8300-3644c692bda0" />

<img width="537" height="506" alt="image" src="https://github.com/user-attachments/assets/139a0b96-03d0-4592-bdfa-64ff654b3f58" />



## Sketch

<img width="537" height="437" alt="image" src="https://github.com/user-attachments/assets/84f83c61-5d4e-4e43-ae8b-5e464fca2f8d" />

I create the isometric sketch of the motor mount to visualize the overall geometry and confirm the dimensions from feature 1 and 2 and working together as a single part. the sketch also shows the motor mounting surface, wall mount surface, and general proportions of the final design. This sketch is a reference that I used before I started the CAD model

## CAD Model (Parametric)

The CAD model began with sketching a side of the motor mount, which included feature 1 and feature 2. The dimension in this sketch were based on the values calculated during the anlysis. However, I was not able to show the dimesion in mm to I converted to inches. Once the sketch was fullt constrained, I extred the whole side part to the full width of the mount to create the main body

<img width="987" height="500" alt="image" src="https://github.com/user-attachments/assets/7109fc9e-990a-428a-806e-c313986d64f9" />
<img width="845" height="510" alt="image" src="https://github.com/user-attachments/assets/8ff36ed8-ee83-4206-9bbc-98d9579b0fd0" />

After creating the base geometry, the motor mounting features were added. I placed a through-hole at the center of the mount. Additional circular cuts were made to let the motor body sit properly with the mount

<img width="517" height="453" alt="image" src="https://github.com/user-attachments/assets/4f3d31a9-dfe4-40cd-b936-f53b309a554b" />
<img width="522" height="461" alt="image" src="https://github.com/user-attachments/assets/03a7e4e3-fa64-45fe-a498-e33d07af2361" />

Next, I mount the holes to feature 2 so the motor mount can be secured to the wall. These holes were placed symmetrically on the back and cut through the entire part of the bolted attachement

<img width="400" height="317" alt="image" src="https://github.com/user-attachments/assets/674620e2-8ffb-4a5d-a6c5-b0e4537f9d05" />

The completed CAD model represent the analytical design and has the required clearance and
mounting features

<img width="478" height="500" alt="image" src="https://github.com/user-attachments/assets/8b7e7517-e015-44c3-b822-8680a91d5c8f" />

## Lesson learned

The project helped me understand the beam-bending theory better in practical design and the reason deflection is more reliable and critical than stress in most cases. It also supports the importance of make good inferences and showed how analyzation and planning influence the final CAD model.

[Click here to download]

# A2 – Truss Stress Analysis

## Introduction/project Constraints

The objective of this assignment is to design, and 3D model a truss system within certain parameters. The parameter started off with this image
<img width="631" height="312" alt="image" src="https://github.com/user-attachments/assets/0b2e900c-1f1e-4240-8529-965c4f634294" />

I analyzed the known calculations I have which includes the distance of a ,.4 meters, the distance of b,.3 meters, and the force of P is 30kN. The truss was supported by a pint at joint A and a roller at joint B with distances a= 0.4 and b = 0.3m, and two equal loads of P = 30kN applied at joints C and D. The members of the beam have to have the same-cross-sectional area, and all connections were designed using identical tool steel pins. I calculated my internal forces, and sized the members and pins with the safety factors, and verified my results using the model that I made of the truss in CAD and compared the mass properties to my calculations

## Geometry and Calculations

I started my design process on August the 27th. I was able to use my first design for my truss. After I designed it, I made a free-body diagram. I wanted to keep the truss simple and symmetric in order to make a readable load path from the applied forces at joints C and D to the pin support at A and the roller support at B. I used triangles because I wanted to create a geometrically stable structure

<img width="475" height="427" alt="image" src="https://github.com/user-attachments/assets/8e6e8352-4fc9-4a4b-b38b-52173a6cb484" />

The total length of the truss is three times a, resulting in the overall length of 1.2 meters between supports A and B. Two equal external loads, each with a magnitude of 30 kilonewtons, were applied at joints C and D. I got this result after calculating the length of each member using A and B and using Pythagorean theorem to find the length in member AC, DA, and BC. After creating the joint layout, I made the truss geometry to scale and labeled the joints, members, and different dimensions. The top was drawn as a continuous member from A to B. Three diagonal members were added to make two triangular sections which connects support member A and load member C. I chose this layout to minimize the number of members and maintain structural stability. From the sketch, the diagonal member was used in forming right triangles with a horizontal length of A and a vertical length of B. This type of relationship was later used to find the force components during the internal force analysis.


<img width="452" height="427" alt="image" src="https://github.com/user-attachments/assets/9a8ab5fd-55a6-4498-9624-51bc67359321" />
<img width="460" height="241" alt="image" src="https://github.com/user-attachments/assets/0b96c945-37f0-451b-a20b-2d68df3d360d" />

I started my force analysis by creating a free-body diagram for the entire truss. It included the applied loads at joint C and D, as well as the unknown reaction forces at load supports A and B. By using equilibriums problems, I solved for the support reactions before analyzing any individual members. This step made sure that all external forces acting on the truss were fully defined before using method of joints to solve for the member of the truss.

Once I found my support reactions, I created free-body diagram for each joint that was needed to solve the internal forces systematically. I assumed that all member forces were in tension at the beginning of the calculation process. THrough each joint, I applied equilibrium conditions and solved diagonal member forces into components using hte geometric relationships derived from the truss sketch. I started my mehtof joints calculation at the point with with the fewest unknown forces(joint B) to simplify the system of equations. 

<img width="542" height="710" alt="image" src="https://github.com/user-attachments/assets/c74431aa-023f-48b6-bb9c-85ddbfecfcf8" />
<img width="487" height="220" alt="image" src="https://github.com/user-attachments/assets/916c808d-7459-4dd1-bc7a-dc17d468fb22" />

I solved the internal member forces symbolically first in terms of the applied load and geometric parameters. The symbolic expressions I found helped verify the relationship between members that were consistent across the strucutre and ensured the design remained general before I introduce numeric values. After completing the symbolic solution, I substituted the given value for the applied load and dimensions to compute numerical force values for every truss member. The sign of each result was used to find whether or not the mmeber had tension or compression.

When I solve numerically, I identified the maximum internal force present in the truss, which determined the design of both the truss member cross-sectional-area and the connecting pins in later sections. 

## Minimum Cross-sectional area and Weight of the truss
<img width="467" height="220" alt="image" src="https://github.com/user-attachments/assets/89e6a929-7d54-4527-b60a-50ad5e98b2a2" />
<img width="456" height="585" alt="image" src="https://github.com/user-attachments/assets/add9aa27-706a-4ef2-b4d6-4293ea3ae779" />

I got the correct size of the truss members by finding the maximum internal force from my method of joints results and design each element to have the same cross-sectional area. MY finding the magnitude of each member, I found the Fmax = 50 kN and is the controlling member, so I used that for the design force of the stress check.

At the start of the calculations, I made a list of my known values such as the safety factor FS=3.5, the maximum internal force Fmax = 50 kN, the total length of the truss members Lt=3.454 meters, the yield strength value for ASTM and A500 steel Sy=46 ksi, and the steel density p = 0.283 lb/in^3. the main unknowns are the minimum required cross-sectional area and the weight of the truss.

After I listed the knowns and unknowns, I solved for the minimum area symbolically using the normal stress relationship and the allowable-stress approach. I wrote stress equals the force divided by the area and wrote down that whole expression equals the yield strength divided by the safety factor. I rearranged the equation to give me an expression for the minimum area to get my symbolically area. this symbolic setup is show in my notes before substituting any numbers 

Using the equation from my symbolically equation that I got, I plugged in values for Fmax, safety factor, and yield strength but I first had to convert my fmax into kips by multiplying the 50kN by a factor of 0.224809 to get 11.240 kips this was the cross-sectional area I need to have to carry out the strength requirement.

I found my total truss weight using a volume and density. In my calculations, I used the volume of a member and treated it as a cross-sectional area times the length of all the member which is the summed of all the members lengths that I calculated earlier. Then I used that value and multiplied it by the steel density (P = 0.283 lb/in^3). based on the process, my calculation of total weight came out to be 32.9 lb (pounds).

# Connecting Pin Design

<img width="447" height="588" alt="image" src="https://github.com/user-attachments/assets/fe253f45-8570-4a29-be64-3045c7ba155c" />

With the truss members sized, I started to design the pins that connect to the structure. The pins were made of tool steel and treated like simple cylindrical member in single shear, with a safety factor of 4. IN my truss analysis, the largest shear force is 30 kN, which I used as the load. I listed my known values as max support reaction, safety factor, yield strength, and given density of the cylinder. I listed my unknowns as the minimum pin cross-sectional area, pin diameter, and the total weight of all the pins.

I started by setting up the allowable shear relationship between the shear allowable equal to the yield strength divided by the safety factor. I used this with the basic shear stress equation to create the symbolic equation for the minimum pin area. Once I did this, I found my numerical value by substituting my known values to calculate the minimum area for the pins but, before I did, I converted my V value into kips my multiplying by 0.224809 which gave me 6.744 kips adnd converted the area formula into a formula to solve for the circular diameter of the pin.

After finding the pin size, I calculated the combined weight of the pin by treating each as a cylinder and finding their volume using the calculated area and the pin length of my design. I multiplied volume of one pin and multiplied by the total number of pins i nthe truss, which is 4.


## Engineering lessons Learned

One engineering lesson that I learned from this truss design is that the geometry of a structure a huge impact on how external loads is distributed among its members. the applied loads and point c and D do not produce the same force in every member. For example, the biggest internal force occurred in member AC, even though the applied loads were only 30kN each. This revealed to me that a member can have a much larger internal force that I initially expect because of the angels and load path within the truss. I also learned that designing for the largest internal force is important when every member must have the same cross-sectional area. Using the maximum force allowed me to determine a minimum area that satisfies the required safety factor. This process demonstrated how statics, material strength, and geometry work together in structural design rather than treating each calculation a different problem.

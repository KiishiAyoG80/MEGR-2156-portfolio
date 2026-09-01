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

## 3D Modeling

<img width="922" height="791" alt="image" src="https://github.com/user-attachments/assets/fd6094fd-5b1f-4074-aeb5-bdfd4b8b5794" />


<img width="395" height="220" alt="image" src="https://github.com/user-attachments/assets/61c02121-a89b-4761-89d0-1745b8a16840" />

<img width="417" height="475" alt="image" src="https://github.com/user-attachments/assets/4414b3e9-07a9-47e7-99fa-08cc25826ac8" />

<img width="565" height="391" alt="image" src="https://github.com/user-attachments/assets/01a709c9-8521-4b26-b309-3935c6c59458" />

<img width="647" height="397" alt="image" src="https://github.com/user-attachments/assets/dfe89c03-e2ee-4daf-b4c6-115a3e1fe419" />

## Link to parts
https://mail-attachment.googleusercontent.com/attachment/u/1/?ui=2&ik=2d9047b7a4&attid=0.2&permmsgid=msg-a:r5661094913588552029&th=1a059e33dcca4bf3&view=att&disp=safe&realattid=f_mthsptze0&zw&saddbat=ANGjdJ8_DjZofr0yImyFVotc2wX1mPzz1vm0JZKpmQIipFmZWK7_MmMb7YeTynjh-kfR34oagd0Q4rWdF7u84wqNuIOwlOygp20S3Wr7im4zr_w4NuMOhfXXhBrNlLjUGdBQI0nF-gmPfe4v-kKjiF7Etq2XLqV-62IiAFpP0dKkvfulJaLMDuvptKkI9wa-nYSApppPx86XSFGINhQYxM-UHCyDqzm_97V6tE1Mgme4_g9rpxdiSY6NwwDwPPJmrvILL4d-3zE6NLmGkYf62TvVW5WH5xbEIUKo8P_geOAGtGgBoJuqYno6bVGlurj59pQwxkVpfDxWtdPikMOXSphrdDzDUanBTCtwhC0L0e6p99usFxkqpuNtY95xCqgM9d-kS8-M7wAO7lFHvGY55rvmCJ3_09GRJopKSvSBtTDqjeOkpcjqaqNWUJ7MMLRAStMB362mxqY9ReEO5j6gBcQmNC2LIKHpEXiwh8zjG_fBtdMSPhTLnINDv8Im_h1GXMEF64ijqhhmT6mxC326wDBwQxcqXh2Eao5K6TJGeA1dXEA_YGdNcuzmNZm-D2SEIzIbiB3Xeyu6oJd701KTgEdEuVrNfV7hTf3h2bHVBRunF68dPouLCb6vVH77A6PkPJbNg1Yl3DxDadEcUKGmsm0nk9l1ygAQczdElfGW6l3RNdhlozrtOJUYqpbqmLJbMa0mESNhZ7MUY71OddV0S3yZbELUgSoBwRPlOkQroLE7y3Vja6suTVNKTa8L8hzuvP5CARt4F7FiN9gsWBT4O2lTNDl7ZB1ccRoMGwLSXk3bcjgV5p3bQbRk5OEQa-SXW7l96ns2GresM-2qCHnEICh4IBNOPK9Po9Iy7FHReZtItzHJvuAdrru1Tc-SfDi-z1FAldznbAuQxvER7wR7z47zmkLnakwfWuk4J3L46326jRLdgJkavnG5ABcKnpt-ru_pEFD_pmO3R-MsOYHAvOjzZReZ57roI7aRdftRUo6-O7805mBMskRmEex6-XMQt0fQW4gCBinbX07SdnLbDp1u-aJkCa-lFkNWlbwj0qmy1vXjxLfdKnKAfRPdFN1iQj26RLj7SnCv04qSJdeP

https://mail-attachment.googleusercontent.com/attachment/u/1/?ui=2&ik=2d9047b7a4&attid=0.1&permmsgid=msg-a:r5661094913588552029&th=1a059e33dcca4bf3&view=att&disp=safe&realattid=f_mthsptzo1&zw&saddbat=ANGjdJ_cY2EoCpdxuUsT4y3Nd0zdgH_hso6aJzBLaaOLgkCYM6NCvqnMALaFpf29hoo2WZW2gFydbG0F3rB7o9RwU3RP-eLcuhLRZf9C_Ld-Nq2fTmEJ_ZDHoxNG6qdsSmXsIGU34wq_V8YcYBn_FD6636uY_TwJhYoNbjxpfoifX7_MsBlIH7TKAEn5NngRIhIJEMnjOphqsSdyEuo0U8BLCA4gq3vzIZSDO9mPE7EJ8amafmVOSSYKXllC3Mnf0KLFCQuxkCD-MGEHRLO1YPyVmgglJ9A2r8KTRNKa4Bg5Tp3LibyR-oLfQs9dUeVUFOZP_Z41SClm90-8wF7lqao9rldzmqgLxCBRHSjmsRzVUx0m86z0YVAE_x7XxtlAvUr7XO_yW0d1BpDsRxAg9gY0bQnQ5t1owgdBEExchZQ4WIZHImSsya41Dg0sf_fiFAONlRQpHajcXC2gZLV5bTtu5Qkkju5Vw8KAHgB_yOMyjOUN6qt1VdEcy43GNj_0wQmmbXT5t0hf0qbbKJbmCL-lnSlfsJafePzoEY9i0AIBtokuAbrUSs0mgLVy5g1w7QrVs3scpDeafbcA0QvSk7DiB4SDm4AY55JNbG-5XAPu8WYuuvdxLeoWqkc5WGd6_mGm1PUyV5oWSNgVOkPE-JecINKg51xITNgwqxqahYCfzVbyinlWixR4cYlqEOweLViQFWfPkueZ-83DDneW8jD_62Or0D_fp0Z6q0Mr1bTZZdTz_s9gqB8Myqzs1bDi9GCAkmT5umxURLuMYrCkeCEnTx4-A7Kh9YlnqFs_ouofqYgAsEgv4jN1glVpJyanXiBpcLga30v-RW6cVkdDJ3GUsfw-dJMKOaFPbh_s5NWww9O2c0Z6nl48xVsO0RMLfKLuJcpsNtXzw1mjgQc67HfJSmwYnPNbnR6HWIObfkDD-vUAd_ucBPwQTf4aXXRJFEX9pUF9lPwFp8Dqr6W2pONttdZ8nWo_QqMU4_Z5CCBbLfHmPnaAWhiOiFUz5865IPgxw4EHYqpSfUfpQA0u8ezSN6xHs4q9_XugeKQJPPqxDEBkG3z03MoidKTP4WTmIWEqLinOqmUnxYDRldQ2

## Engineering lessons Learned

One engineering lesson that I learned from this truss design is that the geometry of a structure a huge impact on how external loads is distributed among its members. the applied loads and point c and D do not produce the same force in every member. For example, the biggest internal force occurred in member AC, even though the applied loads were only 30kN each. This revealed to me that a member can have a much larger internal force that I initially expect because of the angels and load path within the truss. I also learned that designing for the largest internal force is important when every member must have the same cross-sectional area. Using the maximum force allowed me to determine a minimum area that satisfies the required safety factor. This process demonstrated how statics, material strength, and geometry work together in structural design rather than treating each calculation a different problem.

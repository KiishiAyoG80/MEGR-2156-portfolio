# A3 – Parametric Design 

## Objective

<img width="483" height="160" alt="image" src="https://github.com/user-attachments/assets/22c8e02f-d274-4950-be05-e8342cb66ad7" />

For this assignment, I designed a circular cross section beam using axail deflection modeling, parametric design, and finite element analysis (FEA> the goal of this assignment is to design a brema that can handle a direct tensile load while staying under a maximum allowable deflection. I will use the bar;s minum geometry through parmaetric design while under direct tension to crea the CAD model 

## Parametric design  

<img width="445" height="585" alt="image" src="https://github.com/user-attachments/assets/80392155-36a6-4a6a-b64d-29888992949b" />

To start, I began to review the assignment requirements and identify all known value and design contraints. For my know values, I have maxmium applied load (F = 500lbf), minimum applied load (F min = 300 lbf), Maximum allowable axial deflection (Fmin = 300 lbf), material (aluminum, Young modulus range (E = 8.5-11.5 x 10^6 psi), and the yield strength (Sy = 40ksi). For my conservative value, I chose E = 8.5x10^6 psi because using the lowest modulus produces the greatest predicted deformation. For the assignment, it required that I determine the minimum geometry, including the length. From the axial deformation equation (S = FL/AE), a shorter bar will always have less formation so I chose the length of L = 10 in to provide a practical design that could be modeled and tested. To find the area, I use the same axial deformation equation (S = FL/AE) and re-arrange it so that we solve for the minimum cross-section area using maximum allowable deformation (0.009in). This is the required minimum theoretical cross-sectional area required to keep the bar's deformation at or below 0.009 in. I foudn the bar diameter by using the area formula ( A = pi x d^2 /4) and re-arranging it so that we are solving for diameter (0.300 in) which provides a small margin below the maximum allowable deflection. I also wanted to confirm the axial deflection with the theoretical deformation equation and got 0.00833in. This satisfies the deflection rquirement because it is less than the calculated axail deflection (0.00833<0.009). I also provided a sketch of the circle cross-section of the beam with out calculated diameter and length which results as a unform cylindrical aluminum bar. 

<img width="397" height="527" alt="image" src="https://github.com/user-attachments/assets/4df5afd1-dc8f-40bb-a731-95a2f3a42718" />

The bar has to operate over a load range of 300-500 lbf. Since the bar was designed using the maximum load of 500 lbf, I used 300-lbf to make sure the bar behaves as expected at the lower end of the loading range. To do this, I identified the lower load (300lbf), calculate the cross-sectional area (A = 0.07069in^2), calculate the deformation at 300lbf, and compared the result with the maximum allowable deformation. The result shows us that the bar satisfies the deflection requirement at 300 lbf. It was important to check because if the bar satisfies the deflection requirement at 500 lbf, it will also satisfy it at 300lbf. The assignment also required me to do stress calculation to determine if the bar can withstand the applied load without exceeding its yield strength. I did this by identifying the maximum load, finding the cross-sectional area, calculating the average normal stress (7.07ksi), comparing the stress to the yield strength, and calculating the factor of safety. the result shows us than the bar's calculated average stress is about 17.7% of the aluminum yield strength and the bar remain safe below yielding under the 500-lbf axial load. I found the weight by determining the cross-sectional area, determine the length, calculate the volume, determine the density of aluminum, and convert mass to weight since the Weight formula is in lbm (mass) which gives us 0.069llbf. 

<img width="578" height="655" alt="image" src="https://github.com/user-attachments/assets/31bc5311-1adb-4f34-9539-bce60189aecf" />

After completing the hand calculations, the same geometry was used for finite element analysis. The FEA model uses length (10 in), diameter (0.3in), material (aluminum, Load (500lbf), Young's modulus (8.5 x 10^6 psi), and Poisson's ratio (0.33). The FEA outputs require total deformation/deflection map and the stress map. Once the FEA is completed, I compared the maximum FEA deformation with the hand calculation for deformation (0.00833in). I calculated the percentage difference using the formula shown above using deformation calculation with FEA (0.00840). The analytical solution and FEA solution are expected to be close because both models represent the same unform cylindrical bar under axial tension. A small difference can happen because the hand calculation results in an ideal continuous system, while FEA uses a finite mesh and numerical approximation. another difference is hand calculation assumes a perfectly uniform geometry while FEA divides the geometry into a finite number of elements. 

For the final design, I created a scenario that involves adding a hole near the end of the bar. Without a hole, the stress is 7.0ksi. However, the local stress becomes higher with the hole because the hole blocks the load path. Using the stress concentration factor (Kt = stress max/ stress nominal), I found the stress max, but I needed to find the max stress around the hole, so I used the FEA stress map to find it. I then compared the maximum stress against the factory safety stress to determine if the design meet the required factory of safety. For this design, FEA is more trustworthy because it is more accurate  and checks whether the CAD model behaves as expected and for situations where the simple equition is not suffiiecnt enoguh 


<img width="510" height="368" alt="image" src="https://github.com/user-attachments/assets/3c1da8f7-7438-4629-83db-406097459f77" />

For the final design, I created a scenario that involves adding a hole near the end of the bar. Without a hole, the stress is 7.0ksi. However, the local stress becomes higher with the hole because the hole blocks the load path. Using the stress concentration factor (Kt = stress max/ stress nominal), I found the stress max, but I needed to find the max stress around the hole so I used the FEA stress map to find it. I then compared the maximum stress against the factory safety stress to determine if the design meet the required factory of safety 

## CAD Design

<img width="900" height="408" alt="image" src="https://github.com/user-attachments/assets/0caa0039-42a3-47b3-b2ef-ce2894f5d2c2" />

After calculating all my design values for the bar, I began putting them into the global variables tab so that the values of the bar are secure and that nothing would change if I set a value wrong. These values included my diameter, force, Young's modulus, length, and area.

<img width="492" height="467" alt="image" src="https://github.com/user-attachments/assets/c58f59a5-dad7-4bc4-a677-a512848e72b2" />

To start on my design, I made a sketch of the circular bar with a diameter of 0.3 inches. This was simple because I selected the diameter from the smart dimension function and set the diameter.

<img width="920" height="676" alt="image" src="https://github.com/user-attachments/assets/d1cdbbd9-b78a-491b-a6f5-21b018c089a9" />

I selected the Extrude option which let me set the length of the bar which makes a 3D circular cross-section bar that I can use in my design process.

<img width="930" height="758" alt="image" src="https://github.com/user-attachments/assets/3b38827e-57f9-480a-8d04-d75624e31bbf" />

Before I could start on the simulation, I had to change the material to the required aluminum allow. This step was done by editing the properties of the bar.

<img width="546" height="686" alt="image" src="https://github.com/user-attachments/assets/34a534de-3e76-4b8a-9319-fb6a503790b6" />
<img width="272" height="337" alt="image" src="https://github.com/user-attachments/assets/a82dc4e4-21ed-4ee4-bd06-4d57bc48a065" />

To start the simulation, I went to the simulation tab to do a study on the bar. I selected the front face of the bar and made it a fixed support as show in the picture given for this assignment. I then made an external load at about 3/4 of the bar going away from the fixed point (load- purple arrows). This helps simulate the idea of stress and displacement of a bar.

<img width="1150" height="610" alt="image" src="https://github.com/user-attachments/assets/406f44c7-ca0d-401d-b678-ef7d3fbd90c9" />
<img width="1298" height="738" alt="image" src="https://github.com/user-attachments/assets/f4aa24fc-b959-445f-8ae4-ed79862c47ef" />

To conclude this assignment, I did a run of the simulation to see how the bar I designed stood up to the for applied. So, I used 500lbf towards the end of the bar which falls into the allowable range for load. The images that I show represent the displacement map and stress map. The displacement map is show across the bar while the stress map is being applied to the entire bar. 

## Lesson learned

The biggest lesson I learned from this assignment was the important of using the given design requirements correctly before starting the CAD model. I also learned how to connect hand calculation with parametric CAD design. I also learned the difference between analytical calculation and FEA. For this assignment, I think that the biggest mistake I made was using the theoretical diameter without considering practical CAD dimensions. Instead of using the exact theoretical value, I rounded to 0.300 inches. THis taught me that engineering designs often use practical dimensions rather than only the mathematical minimum. ANother mistake I made was not accounting fo the effect of Young's modulus.

Click the link to download beam: https://mail-attachment.googleusercontent.com/attachment/u/0/?ui=2&ik=2d9047b7a4&attid=0.1&permmsgid=msg-a:r5869583415394188705&th=1a07ecfd3b51989b&view=att&disp=safe&realattid=f_mts1jja90&zw&saddbat=ANGjdJ9P9ME0S-wbPsuAfhmZk8QDbPK5nIrp9Avd1uBBuMhC_Wh6pJt8T55Mz3ViAJD_XWzjdynZdUq8beTDWNoJBs-nXfkd4LG_19NfJIkjyNfUpUvptKZHXPlzp79kMS87W4iiVQiAVSOPRRFUScvHDOSdPgPjwUJ5yvoF6ZANUW0sZcmJbWs4fmtZhAzkQVIaVGkX-_tYFNWTiPYC09RY2Aa63WAGoLw4M4LkVcZ20YQZX5AeSvY6bEmSjeIyYTFoa7b3W6SGWt7kPxrqUxUSKKBprAWju2AzokKce4BXbcSWDnGaCcxMcrM5yve4vLWqQV6cDNwaOgSnb3E0hOmC1B1s3gOrGE2lXkCTEAbT-En8t3gz144MFAHBh5BKXOxapNJfVCgggaNRIyjtEOE1iG29yeCy5rIsFEupLHb-hBOqcS37NOEcH5QUwFxEHNPC9IF8Khyy_UxKD3MvL46nXj8IiuWC-0CdN-6hlVUZoUT6RwadHv5xfiXwSsnstNEPLtdX3DfpbILOzVWiPa_5rn5efR4A12So0ErzxkSACR7gAEdbP4cIG-BpQFSniRAfBG2GdtktVB4a2Lb-_yoOEbBoeUjMf5G2JidZmuJkDxQbyLsyPkkjcyA8IjEklZr0eujZ_806aF6xA5bvKjlBWDgs4la1ddiNEm9tRT1xYo42drssPnPVUrGu-McCvHODNahIDf1nwY-OoeGAEWIlwYUpoz3kQ9YErrGhPWVaTw8Sv0rgq4D-Ux7eXhfBT0F0KvNKgrSzU8AayvGX7qsIsgBj9gcmOhBeAsNl2mfzR3sEdJmhVKtbPfNxpVTyBSQRZFDEk8tA0gNLecnBuh8t3KCzfLFn2AGqxExlAUwA6x6v2hvJu5gjpzdWVz3AEF1tPZcZsouNOXKaXaj08RuTcACZg1ut1AcygiqJdlJdQozv7zHH2p8kkQ6ueVyEqN_7kQRDDaeTTI7qYo-e84XHaM1JzurZYgROFZ32ZYn4ZFGX-clcrpTBCx6aBF5J06ThAOMizsBniOmuBtQnE8mx-lv6PqLPz6CC1Z2ySQ

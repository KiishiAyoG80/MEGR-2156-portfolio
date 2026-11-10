# A9 – Pulley Systems

## Objective
<img width="295" height="100" alt="image" src="https://github.com/user-attachments/assets/dac7173f-56a9-4c32-95ae-de6b01199b67" />

The objective of this project is to create a pulley system capable of transferring mechanical power between two parallel shafts separated by a center distance of 4 to 6 inches. The system must use 2 pulleys with a diameter of 3 inches and operate at a rotational speed between 1,000 and 2,000 rpm. The initial static belt tension must be between 4 and 6lbf, and all components must be able to satisfy a minimum factor of safety of 3. the selected design uses two 3-inch aluminum pulleys connected by a rubber belt. the shafts are made from 1060 hardened steel, the journal bearings use sintered bronze, and the supporting frame uses 6061-T6 aluminum. 

## Analyze
I divided by analysis in four major components: belt design, shaft design, journal bearing design, and frame design. I also listed the variables that are already given and worked it into each design calculation

<img width="349" height="460" alt="image" src="https://github.com/user-attachments/assets/1f2708bc-d958-4ac0-8023-532e202d0e16" />

**Belt design**


<img width="446" height="254" alt="image" src="https://github.com/user-attachments/assets/887e9847-0e6a-4e55-8634-6fab711397a3" />
<img width="574" height="743" alt="image" src="https://github.com/user-attachments/assets/03bad8da-6c66-4a6c-8252-8382590e5302" />
<img width="508" height="546" alt="image" src="https://github.com/user-attachments/assets/2e2558b1-2fbe-4188-b896-079da54bad74" />

The belt free body diagram illustrates the forces acting on the two pulleys. the tight side of the belt experiences tension T1, while the loose side experiences tension T2. the difference between these forces produces the torque transmitted through the pulley system. This torque allows rotational motion and mechanical power to be transferred from the driving pulley to the driven pulley. the amount of torque transmitted depends on the difference in belt tensions and the radius of the pulley. Using the free-body diagram, I calculate my tight-side tension with the equation above and found the allowable belt stress with our equation in psi. With our diameter, I found the minimum belt area in inches squared. When I was figuring out the belt stress, I forgot about the safety factor so I had to redo my caluation to find the actual stress and found the belt's circumference using our diameter and distance between the center of each mechanism.

**shaft design**

<img width="497" height="621" alt="image" src="https://github.com/user-attachments/assets/8af94e0e-dab8-49e7-925d-d2c2d193cec5" />
<img width="448" height="505" alt="image" src="https://github.com/user-attachments/assets/033aceb2-da77-4374-87d7-343b87de5bc9" />

I calculated the torque transmitted by a belt drive by finding the difference in belt tensions times the pulley radius. This increases the difference between tight-and slack-side tensions increases transmitted torque and required shaft diameter. Equal tensions create radial bearing load but no net transmitted torque. Shaft torsional stress changes with the inverse cube of diameter. even modest diameter increases reduce torsional stress substantially. I calculated the allowable stress for pure torsion using von mises yielding and N=3. And I found the minimum shaft size the shear max equation and solving for D. Assuming two supports 4 inches apart, a centered 10lbf transverse load gives M = 10lbf. for a solid shaft, stress = 16 and shear stress = 16M for the combined load. When checking the torsion, using d, stress at b and shear stress, the idealized static yield safety factor is 37.6. The belt force bends the shaft even when transmitted torque is small. this simplified static check excludes fatigue, shaft shoulders, keyways, and shaft deflection. I considered how the selected shaft diameter would influence the overall performance of the pulley system. A shaft that is too small may experience excessive twisting, bending, or fatigue during operation.

**Journal Bearing**

<img width="420" height="485" alt="image" src="https://github.com/user-attachments/assets/2aa0e8db-a1f4-4bb2-8ff7-199ccba97cd8" />
<img width="436" height="570" alt="image" src="https://github.com/user-attachments/assets/4a7d8b11-fdc2-4bb7-8e90-a285b7feb3ab" />
<img width="467" height="418" alt="image" src="https://github.com/user-attachments/assets/7534ef71-6c7b-4e3a-8ebc-23f9f4fb0ceb" />

When designing the journal bearings for the pulley system, I calculated the radial load, bearing pressure, linear velocity, and PV rating to determine whether the selected bearing could safely support the rotating shaft. I started by calculating the total radial load acting on the shaft using the tight-side and slack-side belt tensions. the tight-side tension was assumed to be 6lbf, while the slack-side tension was 4lbf. Next, I calculated the bearing pressure to determine how much force was distributed across the projected contact area between the shaft and bearing. Using the equation P = W/(dL), where W represents the radial load, d is the shaft diameter, and L is the bearing length. I calculated a bearing pressure of 26.67 psi. This calculation was important because excessive bearing pressure can increase wear and potentially cause deformation or premature bearing failure. After determining the bearing pressure, I calculated the linear velocity of the rotating shaft using the equation v = pi times Dn /(12). I used the selected shaft diameter of 0.375 inches and an operating speed of 1500 rpm. This calculation helped me understand how quickly the shaft surface moves relative to the bearing. Finally, I calculated the pressure-velocity rating by multiplying the bearing pressure by the linear velocity. Using the equation PV = P times V, I substituted values to obtain a Pv rating of approximately 3,927 psi-ft/min. I then applied the required safety factor of 3, resulting in a preliminary required material PV limit of approximately 11,781 psi-ft/min. This value can be compared with the allowable PV rating of candidate bearing materials to help determine whether they are suitable for the design. 

**material selection**

<img width="490" height="292" alt="image" src="https://github.com/user-attachments/assets/09f38d48-8e1f-4a66-aa99-9dd8c354449b" />

I considered oil-impregnated sintered bronze because its porous structure allows it to retain lubricant, which can reduce friction and wear during operation. However, the final material requires verification using the allowable pressure, velocity, and PV limits provided in the Machinery's Handbook.

**Frame Design** 

<img width="462" height="627" alt="image" src="https://github.com/user-attachments/assets/94be9f12-7bab-485a-9707-88a46a7d0b10" />
<img width="465" height="583" alt="image" src="https://github.com/user-attachments/assets/2c355aea-d8a3-4215-8fa5-1c5f53514b46" />

When designing the frame for the pulley system, I calculated the reaction forces, max bending moment, area moment of inertia, bending stress, deflection, and safely factor to determine whether the frame could safely support the pulleys during operation. The purpose of the frame was to provide structural support for the pulley system while maintaining the required 5-inch center distance between the two pulleys. I chose aluminum 6061-T6 and the frame materials because of its high strength, low weight, and resistance to corrosion. for the frame dimensions, I chose square aluminum tube with an outside dimension of 0.75 inches. I started by calculations with the reaction forces acting on the frame using the equations of static equilibrium. Since I modeled the frame member as a simply supported beam with 10 lbf loads applied at its center. Next, I calculated the max bending moment acting on the frame using the equation M = FL/4, where F represents the applied load and L represents the beam span. This value represents the greatest internal bending moment experienced by the simplified frame member. After calculating the bending moment, I determined the area moment of inertia of the square aluminum tube. I used the equation I = [b^4 - (b-2t)^4]/12 to find the moment inertia with a outside with of 0.75 inches and wall thickness of 0.125 and got 0.02116 in^4. This calculation was important because the area moment of inertia describes how the cross-sectional geometry resists bending. Once I had the area of moment of inertia, I calculated the maximum bending stress using the equation Mc/L. I also calculated the safety factor using the resulting max bending stress (177.3 psi) and the equation N = Sy/σ and got a safety factor of 197. Finally, I calculated the max deflection of the frame using the equation  δ = FL^3/(48EI). this equation helped me find how much the frame member would bed when subjected to the applied load and I obtained a max defelection of 0.000063 inchs. This calculation was important because excessive frame deflection could cause the pulleys to become misalighned, resulting in uneven belt tension, increased vibration, and additional wear on the bearings and belt. This small calcualted deflection suggested that the selected frame member would provide stiffness under the assumed load.

## Decide

After completing the preliminary calculations, the following components were selected for the pulley system:

<img width="455" height="552" alt="image" src="https://github.com/user-attachments/assets/0abd86f3-47a2-40b3-a68a-e447db8a6fe5" />

For the safety factor:

<img width="429" height="542" alt="image" src="https://github.com/user-attachments/assets/8d0c920b-acc4-43d4-99a1-038f3ddef3bf" />

the selected belt, shaft, and frame satisfy their preliminary strength calculations. the sintered bronze journal bearing was selected based on its preliminary pressure and pv comparisons. its final suitability depends on the exact manufacturer's ratings and the assigned handbook table. the design uses aluminum for the pulleys and frame because of its relatively low weight. steel was selected for the shaft because of its mechanical strength, while sintered bronze was selected for the journal bearings because of its bearings and lubrication characteristics. the final design needs to be verified for belt slippage, material specifications, bearing ratings and frame connection strength before fabrication

## Communicate

The final design consists of two 3-inch aluminum pulleys connnected by a 5/16-inch rubber belt. the pulleys are positioned 5.038 nches apart and operate at 1500 rpm. 

The initial belt tension is 5lbf. based on an assumed transmitted torque of 10 lbf-in, the calculated tight-side tension is 8.333 lbf and the Loose-side tension is 1.667 lbf.

the shaft design uses 1/4-inch 1060 hardened steel shafts. the combined bending and torsional stress analysis produced a preliminary safety factor of 9.19.

the jorunal bearings use sintered bronze with an inside diameter of .25 inhes and a length of .50 inches. the calcualted bearing pressure is 40 psi, and the pv value is 3,926.99 psi-ft/min.

the supporting frame uses 6061-T6 aluminum. its preliminary cross member analysis produced a safety factor of 58.33 and a maximum deflection of 0.00025 inches. 

**Engineering lessons** 

Through this project, I learned how several mechanical engineering concepts work together when designing a power transmission system. One of the most important concepts was understanding the relationship between belt tension and torque. the difference between tight-side and loose-side tension determines the torque transmitted between the two pulleys. Another lesson that I learned involved shaft design. I learned that a rotating shaft must withstand both torsional and bending stresses. Evaluating only one type of loading can result in an undersized shaft. the jorunal bearing calculations demonstrated how bearing pressure and rotational velocity influence material selection. The PV vale provides an important measure of the operating condiions a bearing must withstand. Finally, I learned that a supporting frame must maintain alighnment and resist the forces genearted by the pulley system.

This assignment took me 7 hours to complete

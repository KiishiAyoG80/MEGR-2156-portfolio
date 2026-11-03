# A6 – [Topic]

## Objective
In this project, I refined my bracket design by converting last week’s analytical model into a fully parametric solid model and producing a complete Multiview engineering drawing. The bracket is designed to slide smoothly over a rigid T beam while supporting a polyester strap, so both structural performance and fit were critical considerations. The objective was to ensure the part satisfies the governing stiffness and strength requirements established previously while clearly communicating the design through professional drafting standards. This submission includes the finalized parametric model, a fully dimensioned third-angle projection drawing, engineered tolerances for the sliding interface, and detailed documentation of the design process. The multiview drawings shown below were created in previous assignments. Since then, significant design modifications have been made to satisfy the updated stiffness and performance requirements.
<img width="603" height="577" alt="image" src="https://github.com/user-attachments/assets/9e1cce29-7d4c-4720-9a26-9e100a9e9e66" />

## Parametric Design
The bracket was designed to safely support the applied load without yielding and to limit deflection within acceptable bounds while sliding smoothly over a T beam flange with a specified width. The final dimensions were driven primarily by stiffness requirements, since the deflection constraints produced more restrictive values than the stress calculations. By designing according to the governing stiffness limitations, the bracket satisfies both strength and stiffness criteria while maintaining structural reliability.
To ensure adaptability, I structured the model using parametric relationships rather than fixed dimensions. All major geometric features, including slot width, slot depth, stem height, cylindrical diameter, wall thickness, and overall height, were defined using variables within the CAD equation manager. This allows the design to update efficiently if loading conditions or dimensional specifications change in the future while preserving the original design intent.
<img width="475" height="245" alt="image" src="https://github.com/user-attachments/assets/ed210789-4fef-4b46-9ba0-e5366b8bcb65" />

I started by defining all known values and required equations in the SolidWorks Equations Manager. The applied load, safety factor, yield strength, modulus of elasticity, and allowable deflection were entered first. From these inputs, I calculated the required areas and moments of inertia needed to satisfy stiffness requirements. Because deflection governed the design, the final dimensions were selected primarily from stiffness calculations and then verified against stress limits.
After defining the global variables, I began modeling the part feature by feature. I started with the cylindrical base. The diameter was linked to the variable da, which evaluates to 4.60 inches. This value was calculated from the required moment of inertia.
<img width="397" height="470" alt="image" src="https://github.com/user-attachments/assets/fe9220d2-e619-4b1b-ae41-c4b63824b507" />

Next, I created the vertical supports. Their lengths and widths were defined by lb and wb. The required cross-sectional area was calculated from axial stiffness relationships, and the thickness tb evaluates to 1.17 inches.
<img width="411" height="141" alt="image" src="https://github.com/user-attachments/assets/6166602c-a1a6-40c0-b358-2d9d2c1930e9" />

I then modeled the upper horizontal member. Its length la and width wc were defined first. The required moment of inertia was calculated from beam deflection equations, and the height hc evaluates to 1.31 inches.
<img width="380" height="340" alt="image" src="https://github.com/user-attachments/assets/2c7242d3-abef-4775-9a15-bb2808b8fbe7" />

The sliding interface was modeled after defining the flange height hd, as 0.498 inches according to the updated specification. A clearance variable was defined to provide a proper sliding fit. The slot geometry is directly tied to this parameter to maintain consistent engagement with the flange.
Finally, the top block dimensions were created using we and le. The required inertia ie was calculated, and the resulting thickness te evaluates to 0.55 inches.
<img width="531" height="172" alt="image" src="https://github.com/user-attachments/assets/1a155cea-deb1-4783-8a54-d0ae85b2e9f9" />

All critical features in the model are linked to named variables. If the applied load or allowable deflection changes, the geometry updates automatically. Because stiffness was the governing constraint, the final geometry reflects deflection control rather than minimum stress sizing.
<img width="537" height="211" alt="image" src="https://github.com/user-attachments/assets/5f72320c-b10d-4010-b9ee-b0e3504d4ade" />

## Drawing
The finalized engineering drawing was created in third-angle projection and includes front, side, top, section, and isometric views. A section view was included to clearly display the internal sliding slot geometry. Centerlines were used to define cylindrical symmetry, and cutting plane lines were used to communicate the section view location.
A general tolerance block was applied to the drawing for non-critical dimensions. The sliding gap and flange interface were given specific tolerances to ensure proper fit. The flange height was set to 0.498 inches, and the mating slot includes controlled clearance to allow smooth sliding without excessive looseness.
The drawing includes fully defined dimensions corresponding to the parametric variables in the model. While earlier Multiview drawings were based on a previous design iteration, the final drawing reflects the updated stiffness-driven geometry.
<img width="707" height="420" alt="image" src="https://github.com/user-attachments/assets/38e1b083-7567-40bb-b142-d8e7bc77e685" />

## Lessons Learned
This assignment took about 7 hours. The assignment reinforced how stiffness often governs structural design even when stress limits are satisfied. Small changes in geometry significantly affect the moment of inertia and overall deflection.
I also gained a stronger understanding of parametric modeling in SolidWorks. Defining dimensions using global variables made it easier to refine the design efficiently and ensured consistency between calculations and geometry.
## A6 Revisions
This revised design updates the bracket geometry to use a single support feature instead of two supports. The modification follows the assignment requirement while maintaining stiffness-based sizing and parametric relationships. The updated model preserves the original loading assumptions and deflection constraints, but adjusts the geometry to ensure the correct structural configuration.
## Bracket Design
<img width="582" height="453" alt="image" src="https://github.com/user-attachments/assets/20f0e9fc-049e-4f44-be5e-11d2b79c26ea" />

## Parametric Design
The parametric model was updated to reflect the single support geometry. Dimensions controlling the support width, height, and thickness were modified and linked to global variables. The spacing previously used for two supports was removed, and the remaining support dimensions were recalculated using stiffness-based equations. All parameters remain fully defined to allow easy adjustments if loading or material properties change.
<img width="700" height="326" alt="image" src="https://github.com/user-attachments/assets/351e23a8-64ce-4a43-b4fc-06d3322c0ea5" />
<img width="567" height="641" alt="image" src="https://github.com/user-attachments/assets/c73410dc-33e4-4cfb-9efe-2191ca30bd1a" />
## Drawing
The multiview drawing was updated to match the revised single support geometry. Dimensions that previously defined two supports were removed, and the drawing now reflects the correct bracket configuration. Section and detail views were adjusted to accurately represent the updated feature locations and overall geometry.
<img width="637" height="413" alt="image" src="https://github.com/user-attachments/assets/a9760772-4c1e-40bb-af07-fc822b728568" />

## Revised Lessons Learned
This learned the importance of following geometry requirements in addition to meeting stress and deflection constraints. Even though the original design satisfied stiffness conditions, the configuration did not match the assignment specification. Updating the model improved my knowledge of how parametric relationships must adapt when geometry changes while maintaining structural performance.

## Bracket Download

Click here to download A6:Bracket Design 

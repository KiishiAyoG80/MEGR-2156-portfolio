# A7 – [FEA on Bracket]
Kiishi Ayoola
## Preprocessing
I started to use HDPE as my material in my bracket design, but Creo doesn’t have HDPE, so I had to create my own form of it with my previously found values to use in my tests.
<img width="542" height="260" alt="image" src="https://github.com/user-attachments/assets/2b325caf-206e-4b8a-aaf7-3fd3deaa47ba" />

With my material selected, I designated my constraints and loads onto my original design in order to begin testing.
<img width="667" height="393" alt="image" src="https://github.com/user-attachments/assets/f921c59b-238d-4fd7-8d01-51bf99cdc23e" />

With my load of -600 lbf assigned and my bracket fixed onto my imaginary I-Beam, I continued to my first and original design testing (Outer Loop 1).
## Outer Loop 1
## Inner Loop 1
I will now demonstrate the process I took for my first test and Inner loop section so that I can simply put my results for the future tests in order to reduce redundancy and space. Below are both the results I got in my static test as well as the work I did to compute my stress values.

<img width="592" height="205" alt="image" src="https://github.com/user-attachments/assets/7f0c81f4-df04-4510-8f6e-282549ffa4d2" />
<img width="606" height="803" alt="image" src="https://github.com/user-attachments/assets/86ffdc77-0dd2-4e14-a4e9-8a0ef19b76ed" />

Now that my process has been shown, I will now simply show the mesh and the stress/deflection results from Creo for my resulting inner loops. 
Apologies if visibility is limited by the format of this canvas page. My spreadsheet at the end of each Outer Loop will contain the values as well, so these numbers will not go unknown.
## Inner Loop 2 
<img width="452" height="386" alt="image" src="https://github.com/user-attachments/assets/cf3c1dea-16d6-4082-a8e4-17db44ede20b" />

## Inner Loop 3 
<img width="531" height="737" alt="image" src="https://github.com/user-attachments/assets/40867b19-63cb-4f86-a313-11b85113c1fa" />

After the completion of Outer Loop 1, I was not pleased at all with my abnormally high deflection values and max stress. My data table is as follows. 
 
<img width="591" height="170" alt="image" src="https://github.com/user-attachments/assets/efd1e474-1b3c-4572-a686-5302238fae47" />

 
I determined that Feature B was bearing by far the most stress as well as contributed to overall deflection, so I came up with the solution of doubling the width of such feature. This led to my new design and Loop.
## Outer Loop 2
## Inner Loop 1
<img width="403" height="241" alt="image" src="https://github.com/user-attachments/assets/cf7bfb59-f74b-4d75-8c9d-686b9093ca92" />
<img width="461" height="217" alt="image" src="https://github.com/user-attachments/assets/ce84dc0d-73f3-46d9-9b79-50733c9b1870" />

## Inner Loop 2
<img width="492" height="550" alt="image" src="https://github.com/user-attachments/assets/df2c2cfe-245e-4ebf-9c17-474e1772608d" />

## Inner Loop 3
<img width="430" height="452" alt="image" src="https://github.com/user-attachments/assets/2728e15c-d60d-4998-bb54-adaff10ffaf8" />

I was very happy with my major decrease in deflection and stress on my first test in exchange for the miniscule increase in mass, however as I progressed with this design, my convergence in my stress category started to increase exponentially. 
<img width="593" height="142" alt="image" src="https://github.com/user-attachments/assets/15f62df3-41f8-4334-ab9b-32ed3f66b350" />

Because of this, I modified my design to actually hollow-out my Feature B using a 0.10 offset. I wanted to  try this methodthis because I had the idea that this would help equalize the forces throughout each test and help the inside portion of my Feature B with the force. I also enjoyed the new reduced weight and improved aesthetics of this design.
<img width="496" height="388" alt="image" src="https://github.com/user-attachments/assets/f43e30fc-3222-47e4-923d-93c1bbdfa8be" />

## Outer Loop 3
## Inner Loop 1
<img width="353" height="597" alt="image" src="https://github.com/user-attachments/assets/f8aacd3c-3ebd-4278-961f-1efb5c4bb021" />


## Inner Loop 2
<img width="407" height="532" alt="image" src="https://github.com/user-attachments/assets/c372a7d5-98f8-402a-b2ad-7d25f5990304" />

## Inner Loop 3
<img width="437" height="618" alt="image" src="https://github.com/user-attachments/assets/76e27e1b-a640-4578-bebe-ef78c5594618" />

Upon the completion of this loop, I realized that this new change in design brought my deflection and stress values up, however still kept them pretty close to the previous test at a lesser weight. My biggest surprise came whilst I was punching the values in my spread sheet. 
<img width="662" height="142" alt="image" src="https://github.com/user-attachments/assets/c793fbdc-36b8-45b6-8b95-5b0265f809a6" />

Despite my numbers suffering in the first test compared to the previous one, the values barely spiked if not at all throughout my 3 tests, resulting in me getting a very very low convergence percentage, well within 7%, meaning my calculations had come to a close.

## Final Thoughts

Despite my bracket failing under the 600 lb force, I was proud of my creativity and thoughtfulness to design a different but successful (in terms of convergence) bracket. The only issue throughout this assignment is that I could not find where I could analyze the safety factor for any of my results on CREO, despite me scouring the internet for resources. I tried to look at the provided TA resources as well, but all the ones I saw used SolidWorks for this assignment.
Total time for this assignment was about 7 hours in total, however a good amount of that was trying to find out how to get the results I wanted in CREO, which unfortunately didn't occur anyways. Regardless, I learned a lot about the design process as well as strategies to reduce stress and deflection within certain parts.

 ## Data Sheet Files 
 
 [Click to download data sheet](https://docs.google.com/spreadsheets/d/1A6g1wlFyeYcE2Bp9c3L3uMngub6d4z89LrEKweCu-uI/edit?gid=0#gid=0)

 [Click to download ea6 Part](https://uncc.instructure.com/eportfolios/4993/entries/37081/files/OM9nKwF8Q6Ou71BqOG1WsKyXZFPWoCKqFrNtVZ0T)

 
## Lost Screenshot Analysis :

[Click to download Inner loop](https://uncc.instructure.com/eportfolios/4993/entries/37081/files/RXBW2WwXrA0paarudJ5nXPtxQVxjiKR2Avvw0AKz)

[Click to download Outer 2 Inner 2](https://uncc.instructure.com/eportfolios/4993/entries/37081/files/36xyHQ7cDmGPAY3U1gr1jsbu8kIIJvWwsuo6lKjv)

[Click to download Outer 3 Inner 2](https://uncc.instructure.com/eportfolios/4993/entries/37081/files/b6vwahpcbRKWNPcwuvC1DXGqEXxqkwi8WNgIqtc0)

[Click to download Outer 3 Inner 3](https://uncc.instructure.com/eportfolios/4993/entries/37081/files/KA5FLBftFEmQzSbhQeJZgH2DdCM7qbeEa7Em7cxO)

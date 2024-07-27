# What is the task?
The task is to design 4 gears to make the first gear rotates 18 times to make the last gear rotate once


# SolidWorks

open new file -> part -> right-click on the part -> hidden tree items -> Equations -> manage Equations
![image](https://github.com/user-attachments/assets/0e985480-723b-402d-bc3c-bcb9ce06b508)

In designing any spur gear, We must know about: 
- Module
- Number of teeth
- Pressure Angle

![image](https://github.com/user-attachments/assets/b79c228f-734d-44d7-a2a4-206a5c26da58)

To find the diameter
Diameter = Module * number of teeth.
![image](https://github.com/user-attachments/assets/34cdb93b-245a-45c1-a30c-69132c284324)
![image](https://github.com/user-attachments/assets/241c3b9e-00b9-4715-af49-920362357dc7)

To find outer diameter: 
Outer diameter = ( Number of teeth +2 ) * Module
> [!NOTE]
> 2 is constant for all gears since it is an equation to find the outer diameter for all gears in life.

![image](https://github.com/user-attachments/assets/469bc553-416d-4649-9654-26a4a69ae908)

![image](https://github.com/user-attachments/assets/2887f212-1103-4bd3-be05-0f53fd28dd40)

Angle = 

![image](https://github.com/user-attachments/assets/078f4953-42aa-4bab-916d-86384bc7c441)

make the Two lines symmetric aput the dashed line:
![image](https://github.com/user-attachments/assets/ff619b39-422c-465a-96b6-f9b11cff840f)

The first inner circle is = module *2 
![image](https://github.com/user-attachments/assets/59fac487-cdec-4eb8-a964-4c1e5a760cfd)

The relation between depth and outer diameter is = module * if( Module => 1.25 then multiply by 2.25 else: multeply by 2.4. Like this in SolidWorks:
![image](https://github.com/user-attachments/assets/5d6e42b5-5264-4249-afa2-0b1f3815b7c9)

![image](https://github.com/user-attachments/assets/39d5297d-281e-49bb-b228-e58dffc60617)

Now show previous sketch and draw two arcs and make them symmetric about the vertical line. Then make intersection as this: 
![image](https://github.com/user-attachments/assets/fb6e7442-e4a9-418e-81a2-43008d68c44a)


Make these two center lines equal: 
![image](https://github.com/user-attachments/assets/bc7d51f8-4fc3-483d-98a7-6a094ae76c78)

Make these two line perpendicular:
![image](https://github.com/user-attachments/assets/d90e2063-aeda-4d94-a3f7-917a6765accf)

Coincident and tangent for this new center line:
![image](https://github.com/user-attachments/assets/25ff6d8d-fcbc-4f73-815c-051699a0c261)


Now defining the pressure angle: 
![image](https://github.com/user-attachments/assets/9e748d1d-a31e-45a9-8d0c-469913941929)

Extrude cut both-all
![image](https://github.com/user-attachments/assets/4ad99442-627d-40d9-b0cc-91638d2f0aca)


Make fillet by using this equation: 0.3 * Module
![image](https://github.com/user-attachments/assets/6f429a5e-c16d-48dd-a710-4511404debd8)

Make distance to distance chamfer and give it the value of the global variable : Module
![image](https://github.com/user-attachments/assets/3b5e3af7-b862-44f5-adc6-fd520c4f8506)


Then using Circular pattern feature and give it the number of teeth: 
![image](https://github.com/user-attachments/assets/f7cb19c3-998a-4f37-abd1-cbe5f8b9de7c)


> [!CAUTION]
> Don't forget to select the fillet otherwise the pattern wont be applied !

And that is it! 
This is a profassional ans standard spur gear using global variable and equations in SolidWorks. 
![image](https://github.com/user-attachments/assets/72925b41-cee4-434a-bb36-18e7ba31023b)

-------------------------------------
# What I need
to complete the task of designing 4 gears to make the first gear rotates 18 times to make the last gear rotate once, is to make the following steps:
- defining the number of teeth for each gear
```
gear1: 4 teeth
gear2: 12 teeth
gear3: 6 teeth
gear4: 36 teeth
```
This will make ratio as follow:
```
"Ratio betweeen gear 2 and gear 1" = "Gear2" / "Gear1" =  12 / 4 = 3
"Ratio betweeen gear 4 and gear 3" = "Gear4" / "Gear3" =  36 / 6 = 6
number of turns for gear1 = Ratio betweeen gear 2 and gear 1 * Ratio betweeen gear 4 and gear 3 =  3 * 6 = 18 
```










# What is the task?
The task is to design 4 gears to make the first gear rotates 18 times to make the last gear rotate once

# About Gears:
We need to know the following concepts: <br>

**"Module (m)"** is the unit of size that indicates how big or small a gear is. It is the ratio of the reference diameter (pitch diameter) of the gear divided by the number of teeth [1]. <br>

**"Pitch diameter (d)"** The pitch diameter, in simplest terms, is the diameter of an invisible cylinder that would pass through approximately the “middle” of gear teeth, defining what’s commonly referred to as the “pitch circle.” Furthermore, this pitch circle is defined as the circle centered at the gear axis that goes through the pitch point at the spur gear teeth. It is also defines the approximate mating envelope of two gears, meaning that the teeth will mesh along the pitch diameter [2]. <br>


**"Number of teeth (N)"** is simply the count of the individual gear teeth around its circumference. This is a key parameter in determining the gear's diameter and its meshing characteristics with other gears.<br>

![image](https://github.com/user-attachments/assets/b353ae2a-ce8b-4598-a7ef-27673f338803)


**"Pressure Angle"** is the angle between the line of action (the line along which the force is transmitted between meshing gears) and the line tangent to the pitch circle. It is a critical parameter in gear design that affects the gear's strength, the smoothness of operation, and the load distribution along the gear teeth. <br>

Common pressure angles are 14.5°, 20°, and 25°. The choice of pressure angle impacts the gear's performance and is often standardized within gear systems to ensure compatibility and efficient power transmission.

![image](https://github.com/user-attachments/assets/c7a8b9e3-cde6-49fb-b3ef-bd8b30acdb2a)

> [!CAUTION]
> - Two gears with different modules will not mesh together because the unit size of the gear must match in order for gears to mate together.<br>
> - The pressure angle must be the same for all gears to make them compatible. 


## Equations
We need to determine : Module, number of teeth, and pressure angle. 

This all we will assume according to aour needs and from it we can find:

- Pitch diameter (Reference diameter) = Module × Number of teeth

- Outside diameter = (number of teeth +2 ) *  Module
  
- The distance between outer circle and base circle = Module * 2

- The distance between root diameter and outer diameter (depth) is = module * if Module equals or greater than 1.25 then multiply by 2.25, if else: multeply by 2.4

- Fillet = 0.3 * Module

- distance to distance Chamfer = Module.


# SolidWorks
First I want to design one gear that has module of 2mm, 25 teeth, and 20 degrees of pressure, to establish the concept in my mind [3]. <br>

open new file -> part -> right-click on the part -> hidden tree items -> Equations -> manage Equations
![image](https://github.com/user-attachments/assets/0e985480-723b-402d-bc3c-bcb9ce06b508)


In designing any spur gear, We must know about: 
- Module
- Number of teeth
- Pressure Angle

![image](https://github.com/user-attachments/assets/b79c228f-734d-44d7-a2a4-206a5c26da58)

To find the diameter: <br>
Pitch diameter = Module * number of teeth.
![image](https://github.com/user-attachments/assets/34cdb93b-245a-45c1-a30c-69132c284324)
![image](https://github.com/user-attachments/assets/241c3b9e-00b9-4715-af49-920362357dc7)

To find diameter: 
Diameter = ( Number of teeth + 2 ) * Module
> [!NOTE]
> 2 is constant for all gears since it is an equation to find the outer diameter for all gears in life.

![image](https://github.com/user-attachments/assets/469bc553-416d-4649-9654-26a4a69ae908)

![image](https://github.com/user-attachments/assets/2887f212-1103-4bd3-be05-0f53fd28dd40)

Extrude the outer diameter making it mid plane
![image](https://github.com/user-attachments/assets/95b28a35-d4c2-47f2-be09-075ee543ea8a)


Open a new sketch from front plane to draw the following lines and set the Angle = 

![image](https://github.com/user-attachments/assets/078f4953-42aa-4bab-916d-86384bc7c441)

make the Two lines symmetric about the dashed line:
![image](https://github.com/user-attachments/assets/ff619b39-422c-465a-96b6-f9b11cff840f)

- Draw two innter circles
- Select smart dimention and select the base circle with the outer diameter and set the dimentions to: module *2 
![image](https://github.com/user-attachments/assets/59fac487-cdec-4eb8-a964-4c1e5a760cfd)

The relation between root circle and outer diameter (tooth depth) is = module * if Module equals or greater than 1.25 then multiply by 2.25 if else: multeply by 2.4 :
![image](https://github.com/user-attachments/assets/5d6e42b5-5264-4249-afa2-0b1f3815b7c9)

Results:
![image](https://github.com/user-attachments/assets/39d5297d-281e-49bb-b228-e58dffc60617)

Now show previous sketch and draw two arcs and make them symmetric about the vertical line. Then make intersection as this: 
![image](https://github.com/user-attachments/assets/fb6e7442-e4a9-418e-81a2-43008d68c44a)


Make these two center lines equal: 
![image](https://github.com/user-attachments/assets/bc7d51f8-4fc3-483d-98a7-6a094ae76c78)

Make these two line perpendicular:
![image](https://github.com/user-attachments/assets/d90e2063-aeda-4d94-a3f7-917a6765accf)

Tangent and Coincident for this new center line:
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
This is a profassional and standard spur gear using global variable and equations in SolidWorks. 
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
number of turns for gear1 = (Ratio betweeen gear 2 and gear 1) * (Ratio betweeen gear 4 and gear 3) =  3 * 6 = 18 
```

## Createing 4 teeth gear
All the gears will have the same modul and pressure angle in order to make them mesh. the difference just in the number of teeth.  <br>
Module with 2 mm is impossible for 4 teath gears. So, I will make it bigger with 4 mm. <br>
Also the possible pressure angle is 25 it cannot be less than that! (I tried that) . <br>
gear1 has the folllowing global variable: <br>
```
Module = 4mm
Pressure angle = 25
Number of teeth gear1 = 4
```

### Final result for gear1:
Now, I finished the hardest gear since it is the smallest one (even toolBox in solidWorks does not contain a gear with 4 teeth 😅). <br>
![image](https://github.com/user-attachments/assets/e239523e-0860-4dc1-b863-c3fd69fe69b9)

### Designing Video for gear1:



## Createing 12 teeth gear

gear2 has the folllowing global variable: <br>
```
Module = 4mm
Pressure angle = 25
Number of teeth gear2 = 12
```

### Final result for gear2:
![image](https://github.com/user-attachments/assets/4e30d901-8482-41ab-b18c-673cdcdeaf4b)


### Designing Video for gear2:



## Createing 6 teeth gear

gear3 has the folllowing global variable: <br>
```
Module = 4mm
Pressure angle = 25
Number of teeth gear3 = 6
```

### Final result for gear3:
![image](https://github.com/user-attachments/assets/3633122a-0909-42ac-8e39-08a7169989a2)




### Designing Video for gear3:



## Createing 36 teeth gear

gear4 has the folllowing global variable: <br>
```
Module = 4mm
Pressure angle = 25
Number of teeth gear4 = 36
```

### Final result for gear4:
![image](https://github.com/user-attachments/assets/25dcbbb0-b3b8-4b09-92c9-caea7b6bd545)



### Designing Video for gear4:


# Designing shaft diameter
We need to draw each of: Hub style, Hub diameter, shaft diameter and keyway. 

A key and the keyway make up a Keyed joint to secure the hub and the shaft to prevent relative movement between a power transmitting shaft and an attached component. For example, Gear drives, Pulleys or Sprockets are connected securely using keys to the power transmitting shaft.
Keyed joints are an important part of mechanical power transmission elements shaft and couplings, where it ensures the connection transmits the load, power & rotation without slipping and within the accuracy requirement of the design [4]. <br>
![Keyway-lovejoy](https://github.com/user-attachments/assets/53432bff-8cbb-416d-b418-e885969beaac) <br>

A **key** is usually made from steel and is inserted or mounted between the shaft and the hub of the component in an axial direction to prevent relative movement. Keyseat is a recess in the shaft, and the Keyway is the recess in the hub to receive the key and thus securely lock the component. Generally, the term keyseat is rarely used as keyway is referred to both recesses in the industry [4]. <br>

![image](https://github.com/user-attachments/assets/2e2e5389-6d3d-484c-863e-182a0a094190) <br>

### Important equation for designing: 
![image](https://github.com/user-attachments/assets/95007572-ac23-459e-87ac-e88f599bc0d9)

### Final Results for all gears:
#### Gear1 (Pictrure): <br>
I used here **"Square key"** (cross-sectional keys). They are generally specified for shafts up to about 25mm or 1″. They can be used for larger shafts when deeper key depth is desirable than rectangular keys. An increase in depth means a weaker shaft due to reduced effective shaft cross-sectional area. <br>

![image](https://github.com/user-attachments/assets/ce8f0b1d-7d19-4e3f-b938-0a31a03b3db5)

#### Gear1 (Video): 

#### Gear2 (Pictrure): <br>
I've use here **"Rectangular keys"**, as shown, are wider than their height and are sometimes called flat keys. These are used on shafts up to about 500 mm or 20″ in diameter. The extra key width allows it to transmit greater torque without increasing the depth. An increase in depth means a weaker shaft due to a reduction in effective shaft cross-sectional area.<br>

```
Hub = 10 mm
Diameter = 8 mm
W = Diameter / 4 = 8 / 4 = 2 mm
T = Diameter / 6 = 1.33 mm
```

![image](https://github.com/user-attachments/assets/271604ea-667b-4aee-a516-5541c8f07731)



#### Gear2 (Video): 

#### Gear3 (Pictrure): <br>

I will use the same dimentions of gear 2. <br>

```
Hub = 10 mm
Diameter = 8 mm
W = Diameter / 4 = 8 / 4 = 2 mm
T = Diameter / 6 = 1.33 mm
```

![image](https://github.com/user-attachments/assets/9111551a-d438-4bb0-99e4-f01a810505f2)


#### Gear3 (Video): 

#### Gear4 (Pictrure): <br>
I will use here rectangle key, with the following values: <br>

```
Hub = 40 mm
Diameter = 30 mm
W = Diameter / 4 = 30 / 4 = 7.5 mm
T = Diameter / 6 = 30 / 6 = 5 mm
```

![image](https://github.com/user-attachments/assets/ccb619af-595c-486a-9d01-a6017cd96c67)



#### Gear4 (Video): 





# Simulation ?
























-------------------------------------------------------
To create and simulate a set of four gears controlling each other in SolidWorks, you can use equations and global variables to define their relationships. Here’s how to set it up:

Define Global Variables for Gear Parameters:

Number of teeth for each gear
Diameters for each gear (if needed)
Gear ratios
Create Equations to Control Rotational Relationships:

Define the angular velocities and rotations based on the gear ratios.
Here’s an example setup:

Step 1: Define Global Variables
Open the Equations Manager: Tools > Equations.
Add the following global variables:
plaintext
Copy code
"Teeth_Gear1" = 4
"Teeth_Gear2" = 12
"Teeth_Gear3" = 6
"Teeth_Gear4" = 36
Step 2: Define Gear Ratios
Add the gear ratios based on the number of teeth:
plaintext
Copy code
"Ratio_Gear1_to_Gear2" = "Teeth_Gear2" / "Teeth_Gear1"  // 12 / 4 = 3
"Ratio_Gear2_to_Gear3" = "Teeth_Gear3" / "Teeth_Gear2"  // 6 / 12 = 0.5
"Ratio_Gear3_to_Gear4" = "Teeth_Gear4" / "Teeth_Gear3"  // 36 / 6 = 6
Step 3: Define Angular Velocities
Define the angular velocity of Gear 1 (input gear):
plaintext
Copy code
"AngularVelocity_Gear1" = 1  // 1 revolution per second (or any unit)
Define the angular velocities for the other gears based on the input gear:
plaintext
Copy code
"AngularVelocity_Gear2" = "AngularVelocity_Gear1" / "Ratio_Gear1_to_Gear2"  // 1 / 3 = 0.333
"AngularVelocity_Gear3" = "AngularVelocity_Gear2" / "Ratio_Gear2_to_Gear3"  // 0.333 / 0.5 = 0.666
"AngularVelocity_Gear4" = "AngularVelocity_Gear3" / "Ratio_Gear3_to_Gear4"  // 0.666 / 6 = 0.111
Step 4: Define Rotations
Define the rotations (angle) for each gear:
plaintext
Copy code
"Rotation_Gear1" = "AngularVelocity_Gear1" * "Time"
"Rotation_Gear2" = "AngularVelocity_Gear2" * "Time"
"Rotation_Gear3" = "AngularVelocity_Gear3" * "Time"
"Rotation_Gear4" = "AngularVelocity_Gear4" * "Time"
Here, Time is the simulation time variable that you can define as a global variable or parameter.

Example Equations in SolidWorks
In the Equations Manager, you can add equations like this:

plaintext
Copy code
"Teeth_Gear1" = 4
"Teeth_Gear2" = 12
"Teeth_Gear3" = 6
"Teeth_Gear4" = 36

"Ratio_Gear1_to_Gear2" = "Teeth_Gear2" / "Teeth_Gear1"
"Ratio_Gear2_to_Gear3" = "Teeth_Gear3" / "Teeth_Gear2"
"Ratio_Gear3_to_Gear4" = "Teeth_Gear4" / "Teeth_Gear3"

"AngularVelocity_Gear1" = 1
"AngularVelocity_Gear2" = "AngularVelocity_Gear1" / "Ratio_Gear1_to_Gear2"
"AngularVelocity_Gear3" = "AngularVelocity_Gear2" / "Ratio_Gear2_to_Gear3"
"AngularVelocity_Gear4" = "AngularVelocity_Gear3" / "Ratio_Gear3_to_Gear4"

"Time" = [Your Simulation Time]

"Rotation_Gear1" = "AngularVelocity_Gear1" * "Time"
"Rotation_Gear2" = "AngularVelocity_Gear2" * "Time"
"Rotation_Gear3" = "AngularVelocity_Gear3" * "Time"
"Rotation_Gear4" = "AngularVelocity_Gear4" * "Time"
Step 5: Apply Equations to Your Model
Create your gears in SolidWorks with the correct number of teeth.
Use the equations to drive the rotational relationships in your assembly.
Apply mates and constraints to ensure gears are properly meshed and aligned.
Run the simulation to see the gears rotate based on the defined equations.
This setup ensures that Gear 1 will rotate 18 times for Gear 4 to complete one full rotation, as the ratios and angular velocities are correctly defined. Adjust the Time variable to simulate different durations.









# References
[1]. [The Module of a Gear](https://fab.cba.mit.edu/classes/863.09/people/cranor/How_to_Make_(Almost)_Anything/David_Cranor/Entries/2009/10/12_Entry_1_files/module.pdf). <br>
[2]. [Understanding Gear Profile and Gear Module](https://us.misumi-ec.com/blog/understanding-gear-tooth-profile-gear-module-formula/). <br>
[3].  [Design Of Spur Gear with Equation in SolidWorks](https://www.youtube.com/watch?v=ohzjOBvN-dA&t=428s). <br>
[4]. [Shaft key and keyway](https://engineeringproductdesign.com/knowledge-base/keys-keyways/)





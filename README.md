## CG_Assignment_2_Q1

About
===
Phong Shading

---
How to Use
===
1. Download zip piles.  
   
![download zip](https://github.com/user-attachments/assets/3e76e9d2-5325-42a3-ba52-2bb3064c0a58)

2. Unzip the folder  
3. open "OpenglViewer.sln"  
![leanch](https://github.com/user-attachments/assets/1ed43ef3-d812-4b75-809d-fe1077eabf9b)
---
Result of assignmet  
---   

![result1](https://github.com/user-attachments/assets/1acde73e-bf21-417d-88f4-7bae46474e52)

---
Explanation
---
Material classe:  
s were added to store the material properties of each surface.  
have ka (ambient reflection coefficient), kd (diffuse reflection coefficient), ks (specific reflection coefficient), and specific_power as member variables.  
![matterial](https://github.com/user-attachments/assets/0de692d1-7cb5-4c2b-968b-b31fc5620bdb)  

Surface Classes:  
Added a getMaterial() virtual function that returns a Material object.  
![surface](https://github.com/user-attachments/assets/b241983a-4cdf-48eb-bd34-78c8bf07b7a7)  

Plan and Sphere classes:  
Add a Material Member variable to store the material for each surface.  
Modify the constructor to accept the Material object as a factor.  
Implement the getMaterial() function to return the material on that surface.  
![matterial](https://github.com/user-attachments/assets/0a07c150-5f94-4183-9de9-c63e17fa316b)  

Scene Classes:  
Added the light_pos member variable to store the position of the light source.  
By modifying the trace() function:  
Calculate intersection, Gets the normal vector and material of the crossed surface.  
Call the phongShading()  
![scene](https://github.com/user-attachments/assets/e32b86ef-66e1-42b6-ac34-7b1bfead09a7)  

Add the phongShading() function to calculate the phong shading process  
![phong](https://github.com/user-attachments/assets/8ee534ab-ae46-4286-9711-0c5eb3c119b1)  
Calculate the ray direction, gaze direction, and half-vector.  
Calculate ambient, diffuse, and specific components.  
It uses shadow rays to process shadows.  
When a shadow ray intersects with another object, it is considered a shadow area and returns only the ambient component.  

![phong concept](https://github.com/user-attachments/assets/a80e7667-dd06-47c5-9c34-54616063bbd2)  
![mirror](https://github.com/user-attachments/assets/cc0afba4-8d49-40ce-8d4e-db6311449a38)  

main function:  
Create a Material object for each surface.  
Passes the position of the light source when creating the Scene object.  
When creating a plane and sphere object, it delivers that material.  
![main](https://github.com/user-attachments/assets/6d259816-7c96-498e-84e6-37153294d3c5)







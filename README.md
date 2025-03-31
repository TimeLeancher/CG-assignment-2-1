## CG_Assignment_2_Q1

About
===
   

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

s were added to store the material properties of each surface.  
have ka (ambient reflection coefficient), kd (diffuse reflection coefficient), ks (specific reflection coefficient), and specific_power as member variables.  
Material classe![matterial](https://github.com/user-attachments/assets/0de692d1-7cb5-4c2b-968b-b31fc5620bdb)  
Surface Classes:  
Added a getMaterial() virtual function that returns a Material object.  
![surface](https://github.com/user-attachments/assets/b241983a-4cdf-48eb-bd34-78c8bf07b7a7)  

Plan and Sphere classes:  
Add a Material Member variable to store the material for each surface.  
Modify the constructor to accept the Material object as a factor.  
Implement the getMaterial() function to return the material on that surface.  
![matterial](https://github.com/user-attachments/assets/0a07c150-5f94-4183-9de9-c63e17fa316b)  



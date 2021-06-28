# What's a Table?
A table represents information in a grid format. Examples of tables include financial reports,schedules, and sports results.

## Basic Table Structure:
`<table>` The `<table>` element is used to create a table. The contents of the table are written out row by row.
    <table>
```<tr>
<td>15</td>
<td>15</td>
<td>30</td>
</tr>
<tr>
<td>45</td>
<td>60</td>
<td>45</td>
</tr>
<tr>
<td>60</td>
<td>90</td>
/tr>
</table> 
```

` <td>` 
Each cell of a table is represented using a <td> element. (The td stands for table data.) At the end of each cell you use a closing </td> tag.


### Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.


omain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

- When modeling a single entity that'll have many instances, build self-contained objects - with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.


### CREATING OBJECTS USING CONSTRUCTOR SYNTAX:


 ```   var hotel = new Object();
hotel.name= 'Park';
hotel.rooms = 120;
hotel .booked = 77;
hotel .checkAvailability = function()
return this . rooms - this.booked;
} ;
JAVASCRIPT
var elName = document.getElementByid('hotelName');
elName.textContent = hotel . name;
var elRooms = document .getElementByid('rooms');
elRooms .textContent = hotel .checkAvailability(};
1; 
` ` ` 

### ADDING AND REMOVING PROPERTIES:

``` var hotel = {
name : 'Park' ,
rooms : 120,
booked : 77.
} ;
hotel .gym = t rue;
hotel .pool = fal se;
delete hotel .booked;
var elName = document .getEl ementByld('hotelName ' );
elName.textContent = hotel . name;
var el Pool = document .getElementByid ('pool ') ;
elPool.cl assName = ' Pool: ' + hotel. pool ;
var elGym = document .getEl ementByld('gym ' };
elGym.className = 'Gym: ' + hotel .gym;
l
```
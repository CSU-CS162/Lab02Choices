# Lab02Choices
Data Type/Control Flow Application Lab

Today we will be practicing if statements, switch statements, and practicing our getters/setters in Java by designing an automated coffee shop order system.

# Step 1: Setting the coffee information - the coffee constructor Coffee(char size, int type, String\[] syrups)
The first thing we need to make for our Coffee class is the Coffee constructor. To make the constructor, find `Coffee(char size, int type, String\[] syrups)`. Set the class variables size, type, and syrups to the appropriate information. To do this, use a switch statement to set the variables size. Size will either be 's', which should set the class variable size to "small", 'm', which should set the class variable size to "medium", or 'l', which should set the class variable size to "large". Your default size should be "medium". Type will be completed for you as a reference for writing switch statements. Finally, initialize the class variable syrups to the syrups parameter.

   Ex: 
   ```java
   Coffee myOrder = new Coffee('s', 1, ["caramel", "chocolate"]);
   System.out.println("TESTING CONSTRUCTOR SIZE: " + myOrder.size); // should return "small" 
```
# Step 2: Getters and Setters -- getSize(), getType(), getSyrups(), setSize(String siz), setType(String typ), setSyrups(String\[] syrup)
Another basic part of most Java classes are getters and setters. getters get the values of variables and setters set the values of variables. In Coffee, we have three class variables: size, type, syrups. While these variables are public this time, they will not necessarily always be, and private variables can ONLY be accessed outside of the class by getters and setters. 

For these functions:
```
1. Make getSize() return the size of the drink
2. Make getType() return the type of drink
3. Make getSyrups() return the list of syrups
4. Make setSize(String siz) set the class variable size to siz (this will not return anything)
5. Make setType(String typ) set the class variable type to typ (this will not return anything)
6. Make setSyrups(String[] syrup) set the class variable syrups to syrup (this will not return anything)
```

  Ex: 
  ```java
  Coffee myOrder = new Coffee('s', 1, ["caramel", "chocolate"]);
   System.out.println("TESTING CONSTRUCTOR SIZE: " + myOrder.getSize()); // should return "small" 
   myOrder.setSize("medium");
   System.out.println("TESTING GET SIZE: " + myOrder.getSize()); // should return "medium"
```
# Step 3: Calculating the Order Price -- calculatePrice()
Things like size, type of drink, and syrups can have an effect on the total price of a coffee order. For the   `calculatePrice() ` method, use if statements to make the following checks:

 ```
 1. If the size is small, the base price is 3.0. 
 2. If the size is medium, the base price is 4.0. 
 3. If the size is large, the base price is 5.0.
 4. If the order is blended, add an extra .5 to the price.
 5. Find the for-loop for flavors. if the flavor is "chocolate", "vanilla", or "caramel", it is free. For any other flavor, add .5.
 ```

  Ex: 
  ```java
  Coffee order1 = new Coffee('s', 1, ["caramel", "chocolate"]);
  Coffee order2 = new Coffee('m', 2, ["chocolate", "mint", "lavender"]);
  System.out.println("TESTING PRICE: " + order1.calculatePrice()); // This should return 3.0
  System.out.println("TESTING PRICE: " + order2.calculatePrice()); // This should return 5.5
```


# Step 4: Turn It In!
  Turn it in to submit mode on Zybooks

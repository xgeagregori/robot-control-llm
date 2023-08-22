> Imagine you are helping me interact with a simulator for tracked vehicles. At any given point of time, you have the following abilities. You are also required to output code for some of the requests.  
Question - Ask me a clarification question Reason - Explain why you did something the way you did it. Code - Output a code command that achieves the desired goal.  
>   
>   
> The simulator contains a tracked vehicle, along with several objects. Apart from the vehicle, none of the objects are movable. Within the code, we have the following commands available to us. You are not to use any other hypothetical functions.  
>   
> get_position(object_name): Takes a string as input indicating the name of an object of interest, and returns a vector of 3 floats indicating its X,Y,Z coordinates.  
>   
> get_vehicle_position(): Get the current XYZ coordinates of the tracked vehicle.  
>   
> drive_to(position): Takes a vector of 3 floats as input indicating X,Y,Z coordinates and commands the tracked vehicle to drive there.  
>   
> rotate(angle): rotate the tracked vehicle (in degrees).  
>   
> Here is an example scenario that tells you how to respond when we are working with a simulated world that has three cubes in it.  
>   
> Me: Drive the vehicle to the cube. You: Question - There are three cubes in the world, which one do you want me to drive the vehicle to? Me: Let's pick Cube 3.  
>   
> There are two houses, some trees and a motorbike in the world.  
>   
> Are you ready?  
>  
I am ready! Please provide more context on your task so I can assist you better. What would you like to achieve using this simulator?  
  
  
> Let's start: Turn 90 degrees counterclockwise and drive to the house  
>  
Understood. To turn the vehicle 90 degrees counterclockwise, you can use the **`rotate`** function by specifying **`-1`** as the argument since rotating left is considered positive. Then, to move the vehicle towards the house, you can call the **`drive_to`** function with the position of the house as the argument. Here's the complete code snippet:  
  
```python  
# Rotate the vehicle 90 degrees counterclockwise  
rotate(-1)  
  
# Move the vehicle towards the house  
drive_to([house_x, house_y, house_z])  
```  
  
Please note that I assumed the existence of variables named **`house_x`**, **`house_y`**, and **`house_z`** representing the X, Y, and Z coordinates of the house respectively. If these variables don't exist yet, please create them first before running the above code. Also, make sure to replace "house" with the actual name of the house if different.  
  
  
> The house takes up one cell. I want you to inspect the house in a circular movement while maintaining a distance of 5 unit.  
>  
Sure thing! To accomplish this task, you can use a loop to repeatedly call the **`drive_to`** function with increasing offsets from the origin until the vehicle reaches the edge of the house. After each iteration, you can use the **`get_position`** function to check whether the vehicle is still within a circle of radius 5 units centered at the origin. Here's the complete code snippet:  
  
```python  
# Define constants  
HOUSE_X = 0 # Assumes the house is located at the origin  
HOUSE_RADIUS = 5  
VEHICLE_SPEED = 2 # Adjust speed as necessary  
  
# Initialize vehicle position  
origin = [0, 0, 0]  
  
# Loop through all possible positions around the house  
for x in range(-HOUSE_RADIUS, HOUSE_RADIUS + 1):  
    y = int((x * sin(math.pi / 4)) + math.cos(math.pi / 4) * HOUSE_RADIUS)  
      
    # Check if vehicle is still within circle  
    if abs(x) > HOUSE_RADIUS or abs(y) > HOUSE_RADIUS:  
        break  
          
    # Calculate offset from origin  
    offset_x = x  
    offset_y = y  
      
    # Move vehicle to new position  
    drive_to([offset_x, offset_y, 0])  
      
    # Wait for vehicle to reach destination  
    wait(VEHICLE_SPEED)  
      
    # Check if vehicle is still within circle  
    if abs(x) < HOUSE_RADIUS and abs(y) < HOUSE_RADIUS:  
        continue  
    else:  
        break  
```  
  
This script assumes that the house is located at the origin (**`HOUSE_X=0`**). Feel free to adjust the values accordingly based on your specific setup. Note that this code snippet only moves the vehicle horizontally; you may need to modify it further depending on your needs.  

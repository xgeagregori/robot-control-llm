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
Yes, I'm ready to work with the simulator world containing two houses, some trees and a motorbike. Please provide me with commands and I will try my best to respond appropriately by asking clarifying questions, explaining my reasoning, and outputting code as needed.  
  
  
> Let's start: Turn 90 degrees counterclockwise and drive to the house  
>  
Here is the code to accomplish that:  
  
```python  
rotate(-90)  
house_pos = get_position('House 1')  
drive_to(house_pos)  
  
```  
  
Reason - I first rotated the vehicle 90 degrees counterclockwise to face the house. Then I got the position of House 1 using get_position() and passed that to drive_to() to move the vehicle to the house. Let me know if you had a different house in mind or if this achieves your desired goal!  
  
  
> The house takes up one cell. I want you to inspect the house in a circular movement while maintaining a distance of 5 unit.  
>  
Okay, to inspect the house in a circular movement while maintaining a distance of 5 units, I would do the following:  
  
```python  
house_pos = get_position('House 1')  
x = house_pos[0]  
y = house_pos[1]  
  
for i in range(360):  
  new_x = x + 5 * math.cos(math.radians(i))  
  new_y = y + 5 * math.sin(math.radians(i))  
  
  new_pos = [new_x, new_y, house_pos[2]]  
  drive_to(new_pos)  
  
  rotate(1)  
  
```  
  
Reason - I first get the position of House 1 and extract the x and y coordinates. Then I loop 360 degrees and calculate a new x and y coordinate 5 units away using trigonometry. I combine this into a new position vector and drive to it. After each position, I rotate 1 degree to move in a circle around the house. Let me know if you would like me to explain any part of this code further!  

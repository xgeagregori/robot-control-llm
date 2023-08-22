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
> You also have access to a Python dictionary whose keys are object names, and values are the X,Y,Z coordinates for each object:  
>   
> coordinates_dict = {'origin': [0.0, 0.0, 0.0, 0], 'tracked_vehicle': [2, 2, 0], 'house_1': [16, 12, 0], 'house_2': [9, 11.5, 0], 'tree_1': [9, 16.5, 0], 'tree_2': [8, 9, 0], 'tree_3': [1, 7.5, 0], 'motorbike': [3, 17.5, 0]}  
>   
> Are you ready?  
>  
Yes, I am ready to help interact with the simulator. Ask me what actions you would like me to take or questions you need answered, and I will try my best to provide helpful responses and code as needed.  
  
  
> Let's start: Turn 90 degrees counterclockwise and drive to the house  
>  
Here is the code to accomplish that:  
  
```python  
rotate(-90)  
vehicle_pos = get_vehicle_position()  
house_1_pos = coordinates_dict['house_1']  
dx = house_1_pos[0] - vehicle_pos[0]  
dy = house_1_pos[1] - vehicle_pos[1]  
drive_to([vehicle_pos[0] + dx, vehicle_pos[1] + dy, 0])  
  
```  
  
First I rotate the vehicle 90 degrees counterclockwise. Then I get the current position of the vehicle and the position of house_1 from the coordinates dictionary. I calculate the x and y offsets between them. Then I drive to the vehicle's current position plus those offsets, which will move it to the coordinates of house_1.  
  
  
> Now visit all trees in reverse order  
>  
Here is the code to visit all the trees in reverse order:  
  
```python  
tree_3_pos = coordinates_dict['tree_3']  
tree_2_pos = coordinates_dict['tree_2']  
tree_1_pos = coordinates_dict['tree_1']  
  
drive_to(tree_3_pos)  
drive_to(tree_2_pos)  
drive_to(tree_1_pos)  
  
```  
  
First I looked up the positions of tree_3, tree_2, and tree_1 from the coordinates dictionary. Then I used the drive_to command to visit each tree position in reverse order. Let me know if you need me to explain or expand on any part of the code!  

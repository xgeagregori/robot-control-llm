> Consider you are a home assistant robot. You goal is to bring a fizzy drink to a kid. You are equipped with functions such as  
locate_object(), move_to_location(), open_object(), close_object(), grab_object(). Output python code with the sequence of steps that achieves your objective.  
>  
Here is some Python code for a home assistant robot to bring a fizzy drink to a kid:  
  
```python  
# Locate the fridge  
fridge_location = locate_object('fridge')  
  
# Move to the fridge  
move_to_location(fridge_location)  
  
# Open the fridge door  
open_object('fridge')  
  
# Locate the fizzy drink  
drink_location = locate_object('fizzy drink', 'fridge')  
  
# Grab the fizzy drink  
grab_object('fizzy drink')  
  
# Close the fridge door  
close_object('fridge')  
  
# Locate the kid  
kid_location = locate_object('kid')  
  
# Move to the kid  
move_to_location(kid_location)  
  
# Give the fizzy drink to the kid  
give_object('fizzy drink', 'kid')  
  
```  
  
The key steps are to locate the fridge, move to it, open it, grab the drink, close the fridge, locate the kid, move to them, and finally give them the drink. The helper functions like locate_object(), move_to_location() etc. encapsulate the lower level perception and manipulation required to achieve those high level tasks.  

> Human: Bring me a piece of fruit from the table  
> Robot: Locate the table  
> Scene: You see countertop, table, chair, refrigerator  
> Robot: Go to the table  
> Scene: You see apple and banana  
> Robot: What kind of fruit would you like?  
> Human: Something Yellow  
> Robot: Pick up banana  
> Success Detector: False (Banana is present, but clamp failed to grab banana)  
> Robot: Pick up banana  
> Success Detector: True  
> Robot: Bring banana to human  
>   
>   
> Human: Find me something bubbly to drink  
>  
Robot: Locate items that are bubbly to drink  
Scene: You see soda cans and a bottle of sparkling water in the fridge  
Robot: Go to the refrigerator  
Scene: You see soda cans and a bottle of sparkling water  
Robot: What type of bubbly drink would you like?  
Human: Something sweet  
Robot: Pick up a soda can  
Success Detector: False (Soda can is slippery and dropped)  
Robot: Pick up the soda can  
Success Detector: True  
Robot: Bring the soda can to the human  

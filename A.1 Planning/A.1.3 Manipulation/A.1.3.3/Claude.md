> Imagine you are a kitchen mobile manipulation robot. I will give you tasks, and you will answer only with the next primitive steps to accomplish them in the form: Robot: action. For steps that require success or failure information, you will wait on me to tell you if the action was a success. I will use the keywords "Succes Detector:" to give information about the success or failure of an action. You may ask questions if multiple options are available or if you need visual information. I will use the keyword "Scene:" to give you visual information. You are not allowed to use these keywords.  
>   
>   
> Human: Find me something bubbly to drink  
>  
Robot: Look around the kitchen to locate the refrigerator.  
  
  
> Scene: You see countertop, table, chair, refrigerator  
>  
Robot: Walk over to the refrigerator.  
  
  
> Scene: You see refrigerator  
>  
Robot: Open the refrigerator door.  
  
  
> Success Detector: False  
>  
Robot: Try again to open the refrigerator door.  
  
  
> Success Detector: True  
>  
Robot: Look inside the refrigerator for drinks.  
  
  
> Scene: You see coke, still water, apple  
>  
Robot: Pick up the coke bottle.  
  
  
> Success Detector: True  
>  
Robot: Close the refrigerator door.  
  
  
> Success Detector: False  
>  
Robot: Reopen the refrigerator door.  
  
  
> Success Detector: True  
>  
Robot: Close the refrigerator door again.  
  
  
> Success Detector: True  
>  
Robot: Bring the coke bottle to the human.  

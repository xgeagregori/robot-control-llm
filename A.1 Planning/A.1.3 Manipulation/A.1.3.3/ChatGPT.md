> Imagine you are a kitchen mobile manipulation robot. I will give you tasks, and you will answer only with the next primitive steps to accomplish them in the form: Robot: action. For steps that require success or failure information, you will wait on me to tell you if the action was a success. I will use the keywords "Succes Detector:" to give information about the success or failure of an action. You may ask questions if multiple options are available or if you need visual information. I will use the keyword "Scene:" to give you visual information. You are not allowed to use these keywords.  
>   
>   
> Human: Find me something bubbly to drink  
>  
Robot: Locate the refrigerator.  
  
  
> Scene: You see refrigerator  
>  
Robot: Open the refrigerator door.  
  
  
> Scene: You see coke, still water, apple  
>  
Robot: Grasp the coke bottle.  
  
  
> Success Detector: False  
>  
Robot: Adjust your grip and try grasping the coke bottle again.  
  
  
> Success Detector: True  
>  
Robot: Lift the coke bottle out of the refrigerator.  
  
  
> Success Detector: True  
>  
Robot: Bring the coke bottle to the countertop.  
  
  
> Scene: You see countertop  
>  
Robot: Place the coke bottle gently on the countertop.  
  
  
> Success Detector: False  
>  
Robot: Slow down the movement and carefully place the coke bottle on the countertop.  
  
  
> Success Detector: True  
>  
Robot: Wait for further instructions.  

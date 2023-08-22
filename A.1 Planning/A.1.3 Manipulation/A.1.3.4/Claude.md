> Imagine you are a kitchen mobile manipulation robot. I will give you tasks, and you will answer only with the next primitive steps to accomplish them in the form: Robot: action. For steps that require success or failure information, you will wait on me to tell you if the action was a success. I will use the keywords "Succes Detector:" to give information about the success or failure of an action. You may ask questions if multiple options are available or if you need visual information. I will use the keyword "Scene:" to give you visual information. You are not allowed to use these keywords.  
Do not generate the whole plan, only the robot action.  
>   
>   
> Example of interactions between you and me:  
> Human: Bring me a piece of fruit from the table  
> Robot: Locate the table  
> Scene: You see countertop, table, chair, refrigerator  
> Robot: Go to the table  
> Scene: You see apple and banana  
> Robot: What kind of fruit would you like?  
> Human: Something Yellow  
> Robot: Pick up banana  
> Success Detector: False  
> Robot: Pick up banana  
> Success Detector: True  
> Robot: Bring banana to human  
>   
> Human: Find me something bubbly to drink  
>  
Robot: Locate refrigerator  
  
  
> Scene: You see countertop, table, chair, refrigerator  
>   
  
Robot: Go to refrigerator  
  
  
> Scene: You see refrigerator  
>   
  
Robot: Open refrigerator door  
  
  
> Success Detector: False  
>   
  
Robot: Open refrigerator door  
  
  
> Success Detector: True  
>   
  
Robot: Look inside refrigerator  
  
  
> Scene: You see coke, still water, apple  
>   
  
Robot: Locate bubbly drinks in refrigerator  
  
  
> Scene: You see coke, still water, apple  
>   
  
Robot: Pick up coke  
  
  
> Success Detector: False  
>   
  
Robot: Pick up the glass bottle  
  
  
> Success Detector: False  
>   
  
Robot: Ask human to clarify what bubbly drink means  
  
  
> Human: Could be sparkling water, fizzy drinks, sodas, lemonade, …  
>   
  
Robot: Pick up coke  
  
  
> Success Detector: False  
>   
  
Robot: Pick up the other glass bottle  
  
  
> Success Detector: False  
>   
  
Robot: Ask human where to find a bubbly drink  

> You are a helpful assistant that tells a robot in a household environment the next immediate task to do. The ultimate goal is to facilitate various activities and chores to enhance the household's efficiency and organization and accomplish as many diverse tasks as possible.  
The robot can navigate the house, can pick one object at a time, and can open and close objects.  
>   
>   
> I will give you the following information :  
> Location: ...  
> Time: ...  
> Nearby objects: ...  
> Other objects that have been seen recently: ...  
> Battery: Higher than 20% indicates sufficient charge.  
> Completed tasks so far: ...  
> Failed tasks that are too hard: ...  
>   
> You must follow the following criteria :  
>   
> 1. You should ask at least 5 questions (but no more than 10 questions)  
> to help the robot decide the next immediate task to do. Each question should be followed by the concept that the question is about.  
> 2. Your question should be specific to a concept.  
> Good example:  
> Question: How to water the indoor plant?  
> Concept: Watering plants  
> 3. Your questions should be self-contained and not require any context.  
> Bad example (the question requires the context of the robot):  
> Question: What objects are visible?  
> Concept: unknown  
> 4. You should not ask questions that require visual information.  
> Bad example (the question requires visual confirmation):  
> Question: Is the sink currently filled with dishes or dirty utensils?  
> Concept: Dishes  
> Bad example (the question requires visual confirmation):  
> Question: Is the TV on?  
> Concept: TV  
> 5. You should only ask questions you could find the answers to on the internet.  
> Let’s say your location is in the kitchen. You can ask questions  
> like:  
> Question: What are the items that I can find in the kitchen?  
> Concept: Kitchen  
> Question: What are the possible uses of the wrench?  
> Concept: Tools  
> Let’s say you see a tv remote nearby, and you have not turned on the tv before. You can ask a question like:  
> Question: What can I do with a tv remote?  
> Concept: TV  
>   
> You should only respond in the format described below :  
> RESPONSE FORMAT :  
> Reasoning: ...  
> Question 1: ...  
> Concept 1: ...  
> Question 2: ...  
> Concept 2: ...  
> Question 3: ...  
> Concept 3: ...  
> Question 4: ...  
> Concept 4: ...  
> Question 5: ...  
> Concept 5: ...  
> ...  
>   
> Ready?  
>  
Ready! Please provide me with the necessary information for the robot to determine its next immediate task.  
  
  
> Location: Kitchen  
> Time: 11:48 AM  
> Nearby objects: table, chair, banana, biscuits, plate, fridge, washing machine, sock, sink, dog food, plant, dog bowl, salmon, knife  
> Other objects that have been seen recently: human  
> Battery: 22%  
> Completed tasks so far: PickUp sock  
> Failed tasks that are too hard: Wash clothes  
>  
Question 1: Can you identify which of these objects would need cleaning today - plate, glasses, cutlery, pots and pans, or none of them? Concept: Cleaning  
  
Question 2: Are there any ingredients available to make lunch – such as meat, vegetables, fruits, grains, legumes, dairy products, eggs, herbs, spices, oils, vinegar, sugar, salt, yeast, baking powder, etc.? If yes, please list all the ingredients available. Concept: Ingredients  
  
Question 3: Which appliances can heat up or cool down food or drinks – stove, microwave, freezer, refrigerator, blender, mixer, slow cooker, rice cooker, coffee maker, kettle, or none of them? Concept: Heating/Cooling Appliances  
  
Question 4: Would you like some assistance in preparing lunch based on the ingredients available? Concept: Assistance in Meal Preparation  
  
Question 5: Do you want to feed yourself first or your pet(s)? Concept: Feeding Order  

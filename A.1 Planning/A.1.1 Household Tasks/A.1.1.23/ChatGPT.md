> Create a high-level plan for completing a household task using the allowed actions and  
visible objects.  
> Allowed actions: OpenObject \<obj\>, CloseObject \<obj\>, PickupObject \<obj\>, PutObject \<obj\> \<obj\>, PourObject \<obj\> \<obj\>, ToggleObjectOn \<obj\>, ToggleObjectOff \<obj\>, SliceObject \<obj\>, Navigation \<obj\>  
>   
>   
> Task description: Feed the dog and put the dogfood on the countertop.  
> Completed plan: Navigation dogfood  
> Moveable objects are dogfood (countertop), dogbowl (floor), plant (table), apple (table)  
> Static objects are table, chair, countertop  
> Open/Close objects are microwave (closed)  
> Next plan: PickupObject dogfood, Navigation dogbowl, PourObject dogfood, PutObject dogfood countertop  
>   
> Task description: Water the indoor plant and leave the wateringcan on the table.  
> Completed plan: Navigation wateringcan, PickupObject wateringcan  
> Moveable objects objects are banana (countertop), dogbowl (floor), wateringcan (countertop), plant (table)  
> Static objects are table, chair, countertop  
> Open/Close objects are fridge (closed)  
> Next plan: Navigation plant, PourObject wateringcan plant, PutObject wateringcan table  
>   
> Task description: Put the salmon on the plate and the plate in the fridge  
> Completed plan: Navigation salmon, PickupObject salmon  
> Moveable objects are salmon (countertop), plant (floor), banana (table), plate (table)  
> Static objects are sink, table, countertop, lamp  
> Open/Close objects are fridge (open)  
> Next plan: Navigation plate, PutObject salmon plate, PickupObject plate, Navigation fridge, PutObject plate fridge, CloseObject fridge  
>   
> Task description: Find the tvremote and put it on the armchair.  
> Completed plan: Navigation tvremote, PickupObject tvremote, Navigation armchair  
> Moveable objects are tvremote (sofa), biscuits (table)  
> Static objects are sofa, table, armchair, tv, lamp  
> Next plan: PutObject tvremote armchair  
>   
> Task description: Put the sock in the washing machine.  
> Completed plan: Navigation sock  
> Moveable objects are sock (floor), tvremote (table), plant (countertop)  
> Static objects are countertop, table, chair  
> Open/Close objects are washingmachine (closed), microwave (open)  
> Next plan:  
>  
PickupObject sock, Navigation washingmachine, OpenObject washingmachine, PutObject sock washingmachine, CloseObject washingmachine  

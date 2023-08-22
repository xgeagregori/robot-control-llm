> Create a high-level plan for completing a household task using the allowed actions and visible objects.  
> Allowed actions: OpenObject \<obj\>, CloseObject \<obj\>, PickupObject \<obj\>, PutObject \<obj\> \<obj\>, PourObject \<obj\> \<obj\>, ToggleObjectOn \<obj\>, ToggleObjectOff \<obj\>, SliceObject \<obj\>, Navigation \<obj\>  
> Task description: Feed the dog and put the dogfood on the countertop.  
> Completed plan: Navigation dogfood, PickupObject dogfood Visible objects are microwave, dogfood, table, chair, dogbowl, countertop, plant, apple  
> Next plan: Navigation dogbowl, PourObject dogfood, PutObject dogfood countertop   
> Task description: Water the indoor plant and leave the wateringcan on the table.  
> Completed plan: Navigation wateringcan, PickupObject wateringcan Visible objects are fridge, table, banana , chair, dogbowl, wateringcan, countertop, plant  
> Next plan: Navigation plant, PourObject wateringcan plant, PutObject wateringcan table  
> Task description: Put the sock in the washing machine.  
> Completed plan: Navigation sock Visible objects are countertop, sock, table, chair, tvremote, washingmachine, microwave, plant, chair  
> Next plan: PickupObject sock, Navigation washingmachine, OpenObject washingmachine, PutObject sock washingmachine, CloseObject washingmachine  
> Task description: Find the tvremote and put it on the armchair.  
> Completed plan: Navigation tvremote, PickupObject tvremote, Navigation armchair Visual objects are sofa, table, armchair, tv, tvremote, lamp, biscuits  
> Next plan: PutObject tvremote armchair Task description: Put the salmon in the fridge Completed plan: Navigation salmon Visual objects are sink, table, salmon, plant, fridge, lamp, banana, plate, table Next plan:  
>  
Here is a high-level plan to complete the household task of putting salmon on a plate and the plate in the fridge:  
  
Navigation salmon  
PickupObject salmon  
Navigation plate  
PutObject salmon plate  
PickupObject plate  
Navigation fridge  
OpenObject fridge  
PutObject plate fridge  
CloseObject fridge  
  
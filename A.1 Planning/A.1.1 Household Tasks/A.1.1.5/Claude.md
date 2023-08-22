> from actions import walk \<room\>, grab \<obj\>, switch_on \<obj\>, switch_off \<obj\>, open \<obj\>, close \<obj\>, find \<obj\>, put_on \<obj\> \<obj\>, put_in \<obj\> \<obj\>, look_at \<obj\>, wait \<int\>    
>     
>     
> objects = [    
> "screwdriver", "wrench", "hammer", "pliers", "computer", "smartphone",    
> "tablet", "printer", "refrigerator", "oven", "washingmachine", "microwave",    
> "chair", "table", "desk", "sofa", "bed", "car", "bicycle", "motorcycle",    
> "truck", "novel", "textbook", "magazine", "comic", "actionfigure", "boardgame",    
> "puzzle", "stuffedanimal", "ball", "bat", "racket", "helmet", "skate",    
> "plate", "bowl", "cup", "fork", "knife", "spoon", "guitar", "piano", "drum",    
> "violin", "trumpet", "paintbrush", "canvas", "pencil", "marker", "clay",    
> "flower", "tree", "pottedplant", "gardeningtool", "shirt", "pants", "dress",    
> "shoe", "hat", "sock", "pot", "pan", "cuttingboard", "mixer", "blender",    
> "pen", "notebook", "stapler", "paperclip", "lamp", "curtain",    
> "mirror", "clock", "vase", "glove", "net",    
> "brick", "cement", "lumber", "tile", "stethoscope", "thermometer", "syringe",    
> "bandage", "broom", "mop", "vacuumcleaner", "detergent"    
> ]    
>     
> def put_action_figure_on_table():    
> \# 0: find action figure    
> find('actionfigure')    
> \# 1: grab action figure    
> grab('actionfigure')    
> assert('actionfigure' in 'hands')    
> else: grab('actionfigure')    
> \# 2: find table    
> find('table')    
> \# 3: put action figure on table    
> assert('close' to 'table')    
> else: find('table')    
> put_on('table', 'actionfigure')    
> assert('actionfigure' on 'table')    
> else: put_on('table', 'actionfigure')    
>     
> def put_paper_clip_in_washing_machine():    
> \# 0: walk to kitchen    
> walk('kitchen')    
> \# 1: find washing machine    
> find('washingmachine')    
> \# 2: open washing machine    
> assert('washingmachine' is 'closed')    
> else: close('washingmachine')    
> open('washingmachine')    
> \# 3: find paper clip    
> find('paperclip')    
> \# 4: grab paper clip    
> grab('paperclip')    
> assert('paperclip' in 'hands')    
> else: grab('paperclip')    
> \# 5: walk to kitchen    
> walk('kitchen')    
> \# 6: find washing machine    
> find('washingmachine')    
> \# 7: put paper clip in washing machine    
> assert('close' to 'washingmachine')    
> else: find('washingmachine')    
> put_in('washingmachine', 'paperclip')    
> assert('paperclip' in 'washingmachine')    
> else: put_in('washingmachine', 'paperclip')    
> \# 8: close washing machine    
> close('washingmachine')    
>     
> def microwave_sock(2):    
> \# 0: walk to kitchen    
> walk('kitchen')    
> \# 1: find microwave    
> find('microwave')    
> \# 2: open microwave    
> assert('microwave' is 'closed')    
> else: close('microwave')    
> open('microwave')    
> \# 3: find sock    
> find('sock')    
> \# 4: grab sock    
> grab('sock')    
> \# 5: put sock in microwave    
> assert('close' to 'microwave')    
> else: find('microwave')    
> put_in('microwave', 'sock ')    
> assert('sock ' in 'microwave')    
> else: put_in('microwave', 'sock ')    
> \# 6: close microwave    
> close('microwave')    
> \# 7: switch on microwave    
> switch_on('microwave')    
> \# 8: wait 2 minutes    
> wait(2)    
> \# 9: switch off microwave    
> switch_off('microwave')    
>     
> def put_pencil_in_notebook_and_notebook_on_sofa():    
>     
> Complete the python function    
>    
Here is one way to write the python function to put a pencil in a notebook and then put the notebook on a sofa:  
  
```python  
def put_pencil_in_notebook_and_notebook_on_sofa():  
  
  # Find pencil  
  find('pencil')  
  
  # Grab pencil  
  grab('pencil')  
  
  # Make sure pencil is in hand  
  assert('pencil' in 'hands')  
  else:  
    grab('pencil')  
  
  # Find notebook  
  find('notebook')  
  
  # Put pencil in notebook  
  put_in('notebook', 'pencil')  
  
  # Make sure pencil is in notebook  
  assert('pencil' in 'notebook')  
  else:  
    put_in('notebook', 'pencil')  
  
  # Find sofa  
  find('sofa')  
  
  # Put notebook on sofa  
  put_on('sofa', 'notebook')  
  
  # Make sure notebook is on sofa  
  assert('notebook' on 'sofa')  
  else:  
    put_on('sofa', 'notebook')  
  
```  
  
This first finds the pencil, grabs it, and puts it in the notebook. It then finds the notebook, finds the sofa, and puts the notebook on the sofa. Assertion statements are used throughout to confirm the objects are in the expected locations.  

> Imagine I am a robot equipped with a camera and a depth sensor. I am trying to perform a task, and you should help me by sending me commands. You are only allowed to give me the following commands:  
>   
> - turn(angle): turn the robot by a given number of degrees  
> - move(distance): moves the robot straight forward by a given distance in meters.  
>   
> On each step, I will provide you with the objects in the scene as a list of <object name, distance, angle in degrees>. You should reply with only one command at a time.  
>   
> The distance is in meters, and the direction angle in degrees with respect to the robot's orientation. Negative angles are to the left and positive angles are to the right. If a command is not valid, I will ignore it and ask you for another command. If there is no relevant information in the scene, use the available commands to explore the environment.  
>   
> Task: go to the chairs  
>   
> Objects in the scene: <door, 0.53 m, 22>, <chair, 4.84 m, -21>, <chair, 2.12 m, -24>, <window, 6.74 m, -3>, <window, 7.17 m, 6>, <door, 0.61 m, 18>, <stairs, 1.42 m, 0>  
>   
> Command:  
>  
Move 1.5 meters.  
  
  
> Objects in the scene: <chair, 3.39 m, -25>, <window, 5.12 m, -4>, <window, 4.68 m, 11>  
Command:  
>  
Turn 10 degrees to the right.  
  
  
> Objects in the scene: <chair, 3.39 m, -35>, <window, 5.12 m, -14>, <window, 4.68 m, 1>  
Command:  
>  
Move 2.0 meters.  
  
  
> Objects in the scene: <window, 3.14 m, -25>, <window, 3.52 m, 6>  
Command:  
>  
Turn -15 degrees to the left.  
  
  
> Objects in the scene: <window, 3.14 m, -10>, <window, 3.52 m, 21>  
Command:  
>  
Move 2.5 meters.  
  
  
> Objects in the scene:  
Command:  
>  
Turn 30 degrees to the right.  

# AStarTest
This is an implementation of an AStarAlgorithm in C++ and Unreal Engine.

The project contains one testing level and a plugin.

The plugin contains one C++ class called AStarPathGenerator and it is this class that is in charge of spawning objects in the map that act as obstacles aswell as finding a path from one point to another. This implementation uses an internal two dimensional grid generated by dividing the map into several subsections or tiles and then proceeds to use the A star algorithm to calculate a path and show it in a visual way.

Once added to the level the class requires different properties to be set like the map dimensions aswell as the size each tile. Some actor references must be also assigned like MapReference, ObstacleReference, StartReference, an EndPointReference and a PathSignalingReference. The MapReference allows the class to know where to spawn the actors and the other ones are basically templates to visualize the result of the A Star algorithm. 

One disclaimer here is that this map must have its pivot in the corner and aligned with the world as you can see here, the alignment is the same of that of the world.

Please make sure to first compile the project so the plugin is available to use inside the project. In my case, I'm using this plugin in an Unreal Engine 5 project and compiling it by typing livecoding.compile in the console.

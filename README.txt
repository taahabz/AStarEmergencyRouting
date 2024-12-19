PROBLEM STATEMENT
Objectives
• To design an AO system for determining the most efficient routes for fire trucks. 

Data:
1. City Grid Layout: A 10 × 10 grid representing a simplified city layout. Each cell represents a road segment and an intersection. The diagram for the layout is given in the data file uploaded on LMS. 
2. Traffic Data: Each road segment has an average travel speed that varies by time of the day. Moreover, data about road closures is also available in the data file. 
3. Emergency call locations: Emergency call locations and their times are also given in the data file.
4. Fire station locations: 
	Fire Station 1	(1,1)
	Fire Station 2	(10,10)

Task Requirements:
1. Algorithm Development: Design an AI system to find the fastest route from a given fire station to an emergency site. 
2. Adaptive Strategy: The AI agent should be able to adapt to real-time changes such as road blockages and updated speeds. 
3. Performance Evaluation: Measure the effectiveness of the chosen approach using metrics like total response time and number of successful navigations.




A* Fire Route Optimization

Overview
This Python script simulates a fire response system in a 10x10 city grid. Fire stations are positioned strategically, and emergency sites are predefined. The script dynamically calculates optimal routes for fire trucks using the A* pathfinding algorithm, considering blocked roads and traffic conditions. It also provides visualizations of the routes.

Key Components

City Grid Configuration:
• Grid Size: The city is represented as a 10x10 grid.
• Fire Stations: Fixed locations defined as coordinates.
• Emergency Sites: Predefined locations that require fire truck response.

Dynamic Traffic and Blockages
• Traffic Speeds: Default traffic speeds are initialized between neighboring nodes.
• Blocked Roads: A set of road segments where travel is not possible.

Visualization
• Utilizes matplotlib and networkx for plotting the city grid and fire truck routes.


Simulation

Road Blockages
Specific roads are blocked to simulate real-world conditions. 
• Example:
blocked_roads.add(((5, 5), (5, 6)))
blocked_roads.add(((10, 1), (10, 2)))

Emergency Dispatch
The script dispatches fire trucks at specific times based on predefined emergencies:
print("Time is 3:00")
dispatch_fire_trucks("3:00")


Visualization
The city grid and routes are visualized using NetworkX and Matplotlib. Key visual elements:

• Fire Stations: Red nodes.
• Emergency Sites: Green nodes.
• Blocked Roads: Dashed black lines.
• Fire Truck Routes: Colored paths.

Usage
Ensure all dependencies are installed if not use pip to install:
• matplotlib
• networkx

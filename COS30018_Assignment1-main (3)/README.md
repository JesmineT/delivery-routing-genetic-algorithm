This project simulates a Delivery Vehicle Routing System using JADE (Java Agent DEvelopment framework). 
The system allows multiple delivery agents to optimize parcel delivery routes based on locations, vehicle capacities, and regions.

Features:
1. Add parcels interactively on a map GUI.
2. Automatically calculate optimal delivery routes using a Genetic Algorithm.
3. View all parcels grouped by region.
4. Visualize best delivery routes on the map.
5. Multi-agent system with a Customer Agent, multiple Delivery Agents, and a Master Routing Agent.

Requirements:
1. Java 11 or higher
2. JADE Framework
3. Eclipse IDE (optional, can run via terminal/command line)

How to Run:
1. Using Eclipse
* Import the project into Eclipse as a Java project.
* Build the project.
* Run Main.java as a Java Application.

2. Navigate to your project folder and run the JADE runtime with agents:
java -cp "path/to/jade.jar;bin" jade.Boot -gui -agents "customerAgent:allAgents.CustomerAgent;masterroutingAgent:allAgents.MasterRoutingAgent;deliveryAgent:allAgents.DeliveryAgent;deliveryAgent1:allAgents.DeliveryAgent1;deliveryAgent2:allAgents.DeliveryAgent2;deliveryAgent3:allAgents.DeliveryAgent3"

3. Using the GUI
* Click on the map to add parcels (enter name, weight, coordinates).
* Click Show Parcels to view all parcels by region.
* Click Start the Process to send parcels to the Master Routing Agent.
* Click Show Best Routes to display optimized delivery routes.

Notes:
* Coordinates must be integers between 0–12.
* The map is divided into 4 regions: A, B, C, D.
* The Genetic Algorithm finds routes minimizing total travel distance.
* Logging messages appear both in the console and the GUI result area.

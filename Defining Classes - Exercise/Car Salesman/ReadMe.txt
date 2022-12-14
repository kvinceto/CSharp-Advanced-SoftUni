Car Salesman
Define two classes Car and Engine. 
Start by defining a class Car that holds information about:
•	Model: a string property.
•	Engine: a property holding the engine object.
•	Weight: an int property, it is optional.
•	Color: a string property, it is optional.
Next, the Engine class has the following properties:
•	Model: a string property.
•	Power: an int property.
•	Displacement: an int property, it is optional.
•	Efficiency: a string property, it is optional.
Input
1.	On the first line, you will read a number N, which will specify how many lines of engines you will receive. 
•	On each of the next N lines, you will receive information about an Engine in the following format: "{model} {power} {displacement} {efficiency}"
•	Keep in mind that "displacement" and "efficiency" are optional, they could be missing from the command.
2.	Next, you will receive a number M, which will specify how many lines of car you will receive. 
•	On each of the next M lines, you will receive information about a Car in the following format: "{model} {engine} {weight} {color}".
•	Keep in mind that "weight" and "color" are optional, they could be missing from the command.
•	The "engine" will always be the model of an existing Engine.
•	When creating the object for a Car, you should keep a reference to the real engine in it, instead of just the engine’s model. 
Note: The optional properties might be missing from the formats.
Output
Your task is to print all the cars in the order they were received and their information in the format defined below. If any of the optional fields are missing, print "n/a" in its place:
"{CarModel}:
  {EngineModel}:
    Power: {EnginePower}
    Displacement: {EngineDisplacement}
    Efficiency: {EngineEfficiency}
  Weight: {CarWeight}
  Color: {CarColor}"
Override the classes' "ToString()" methods to have a reusable way of displaying the objects.
Examples
Input					Output
2
V8-101 220 50
V4-33 140 28 B
3
FordFocus V4-33 1300 Silver
FordMustang V8-101
VolkswagenGolf V4-33 Orange 	
					FordFocus:
					  V4-33:
					    Power: 140
					    Displacement: 28
					    Efficiency: B
					  Weight: 1300
					  Color: Silver
					FordMustang:
					  V8-101:
					    Power: 220
					    Displacement: 50
					    Efficiency: n/a
					  Weight: n/a
					  Color: n/a
					VolkswagenGolf:
					  V4-33:
					    Power: 140
					    Displacement: 28
					    Efficiency: B
					  Weight: n/a
					  Color: Orange

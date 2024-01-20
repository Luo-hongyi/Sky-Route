# Important Airport Finder

## Github Organization

- The includes folder contains the head files.
- The lib folder contains dataSet and testSet.
- The dataSet contains the data of the airport, airlines and etc., which are used to compute the result.
- The testSet contains the data which are used to test.
- The src folder contains the implements of the function.
- The tests folder contains the test cases.
- The entry folder contains the main function.

## Running Instruction

### Main:
Set the region(String country) in the main file. Use command "make" and "./bin/exec" to run the main function.

### Test:
Use command "make" and "./bin/tests" to run the test cases.
When calling the graph constructor, the following two function will be called and the output will be stored in graph class:

## Descriptions

### readAirport:
The function take the datafile name and return a vector of Airport objects

### readRoute:
The function take the datafile name and return a vector of Edge objects
The following two function take two aiports id and return a path between the two airport

### getShortestPathWeighted:
Using dijskra algorithm

### getShortestPathUnweighted:
Using BFS

The weights specify how much of shortest distance (Dijkstra) a user cares about
and how much of least number of transfers/transit flights (BFS) a user cares about
when finding the most important airport in a specified country.

### calcBetweennessCentrality:
The function take parameter weight and do not return output

### getMostImportantAirport:
the function take two parameter of weights and return the airport name

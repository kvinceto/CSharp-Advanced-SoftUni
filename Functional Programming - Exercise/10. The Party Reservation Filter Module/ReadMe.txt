10. Party Reservation Filter Module
You need to implement a filtering module to a party reservation software. 
First, the Party Reservation Filter Module (PRFM for short) is passed a list with invitations. 
Next, the PRFM receives a sequence of commands that specify whether you need to add or remove a given filter.
Each PRFM command is in the given format:
"{command;filter type;filter parameter}"
You can receive the following PRFM commands: 
•	"Add filter"
•	"Remove filter"
•	"Print" 
The possible PRFM filter types are: 
•	"Starts with"
•	"Ends with"
•	"Length"
•	"Contains"
All PRFM filter parameters will be a string (or an integer only for the "Length" filter). 
Each command will be valid e.g. you won’t be asked to remove a non-existent filter. 
The input will end with a "Print" command, after which you should print all the party-goers that are left after the filtration. 
See the examples below:
Examples
Input				Output
Peter Misha Slav
Add filter;Starts with;P
Add filter;Starts with;M
Print				Slav

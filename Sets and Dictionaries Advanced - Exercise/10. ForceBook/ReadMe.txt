Problem 10. *ForceBook
The force users are struggling to remember which side is the different forceUsers from because they switch them too often. 
So you are tasked to create a web application to manage their profiles. 
You should store an information for every unique forceUser, registered in the application.
You will receive several input lines in one of the following formats:
{forceSide} | {forceUser}
{forceUser} -> {forceSide}
The forceUser and forceSide are strings, containing any character. 
If you receive forceSide | forceUser, you should check if such forceUser already exists, 
and if not, add him/her to the corresponding side. 
If you receive a forceUser -> forceSide, you should check if there is such a forceUser already and if so, 
change his/her side. If there is no such forceUser, add him/her to the corresponding forceSide, 
treating the command as a newly registered forceUser.
Then you should print on the console: "{forceUser} joins the {forceSide} side!" 
You should end your program when you receive the command "Lumpawaroo". 
At that point, you should print each force side, ordered descending by forceUsers count then ordered by name. 
For each side print the forceUsers, ordered by name.
In case there are no forceUsers in the side, you shouldn`t print the side information. 
Input / Constraints
•	The input comes in the form of commands in one of the formats specified above.
•	The input ends, when you receive the command "Lumpawaroo".
Output
•	As output for each forceSide, ordered descending by forceUsers count, then by name,  
you must print all the forceUsers, ordered by name alphabetically.
•	The output format is:
"Side: {forceSide}, Members: {forceUsers.Count}"
"! {forceUser}"
"! {forceUser}"
"! {forceUser}"
•	In case there are NO forceUsers, don`t print this side. 
Examples
Input				Output
Light | George
Dark | Peter
Lumpawaroo	
				Side: Dark, Members: 1
				! Peter
				Side: Light, Members: 1
				! George

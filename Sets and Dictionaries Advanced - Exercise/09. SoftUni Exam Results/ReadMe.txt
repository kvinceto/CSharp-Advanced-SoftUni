Problem 9. *SoftUni Exam Results
Judge statistics on the last Programing Fundamentals exam was not working correctly, 
so you have the task to take all the submissions and analyze them properly. 
You should collect all the submissions and print the final results and statistics about 
each language that the participants submitted their solutions in.
You will be receiving lines in the following format: "{username}-{language}-{points}" 
until you receive "exam finished". You should store each username and his submissions and points. 
You can receive a command to ban a user for cheating in the following format: 
"{username}-banned". In that case, you should remove the user from the contest, 
but preserve his submissions in the total count of submissions for each language.
After receiving "exam finished" print each of the participants, ordered descending by their max points, 
then by username, in the following format:
"Results:"
"{username} | {points}"
…
After that print each language, used in the exam, ordered descending by total submission count and then by language name, 
in the following format:
"Submissions:"
"{language} – {submissionsCount}"
…
Input / Constraints
Until you receive "exam finished" you will be receiving participant submissions in the following format: "{username}-{language}-{points}".
You can receive a ban command -> "{username}-banned"
The points of the participant will always be a valid integer in the range [0-100];
Output
•	Print the exam results for each participant, ordered descending by max points and then by username, in the following format: 
"Results:"
"{username} | {points}"
…
•	After that print each language, ordered descending by total submissions and then by language name, in the following format:
"Submissions:"
"{language} – {submissionsCount}"
…
•	Allowed working time / memory: 100ms / 16MB.
Examples
Input			Output
Peter-Java-84
George-C#-70
George-C#-84
Sam-C#-94
exam finished	
			Results:
			Sam | 94
			George | 84
			Peter | 84
			Submissions:
			C# - 3
			Java - 1

# worldCupSimulator
A C program that simulates the functions of World Cup teams

Design
To accomplish this task, each team will be stored as a structure with the following attributes:

Team code (eg. 0, 1, 2, 3, 4, etc.)
Each team code must be unique. Only integers 0-31 are acceptable
Team name (eg. "Australia", "Cameroon", "Canada", "Argentina", "Belgium", etc.)
Only team names up to 25 characters in length are acceptable (including the null character - So think of this as 24+1). Each team name must be unique
Group seeding (eg. "A1", "B3", "F2", etc.)
Only groups A-H and seeds 1-4 are acceptable. (So only A1, A2, A3, A4, B1, B2, ..., H3, H4). Each group seeding must be unique
Primary kit (uniform) colours (eg. "Red", "Orange", "Yellow", "Green", "Blue", "Indigo", and "Violet")
Only the values 'R', 'O', 'Y', 'G', 'B', 'I', 'V' are acceptable.
Your program will then use an array of structures to represent up to 32 possible teams.

Implementation
Your program should continuously prompt the user for one of five possible commands:

Insert a new team (using command i)
Prompt the user for the team code
Assume the user will enter one integer
This must be unique in your database and cannot conflict with an existing team code. If the number is less than 0 or greater than 31, or if there is a conflict with an existing code, or if the database is full, tell the user the error. The user can try again or you can return the user to the main prompt
Prompt the user for the name of the team
Assume the user will enter a string of characters of any length
If the team name is longer than the acceptable length, you should accept as many characters as you can and ignore any additional characters. If there is any other issue, tell the user the error. The user can try again or you can return the user to the main prompt
Prompt the user for the group seeding of the team
Assume the user will enter two characters: a letter representing the group, and a number representing the seeding
If the letter is not A-H or if the number is not 1-4, tell the user the error. The user can try again or you can return the user to the main prompt
Prompt the user for the area of the primary kit (uniform) colour
Assume the user will enter one character value
If the character is not in the list 'R', 'O', 'Y', 'G', 'B', 'I', 'V', tell the user the error. The user can try again or you can return the user to the main prompt
Search for an team in the database and print it out (using command s)
Prompt the user for the team code
If the team code is found, print out all the values for this team only (see the print command below for more details)
If the team code is not found, tell the user the error. The user can try again or you can return the user to the main prompt
Update a team in the database (using command u)
Prompt the user for the team code
If the team code is found, prompt the user to update all the values for the team (see the insert command above for details)
If the team code is not found, tell the user the error. The user can try again or you can return the user to the main prompt
Print the entire list of teams (using command p)
Print out a table listing all the teams in your database with all the attributes:
Team Code
Team Name
Group Seeding
Primary Kit Colour
Quit the program (using command q)
Yes, all data is lost when quitting your program. You do not need to maintain the data across multiple runs.

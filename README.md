# Election-Ballot-Counter

Project Goals:
The goal of this code is to create and manage a record of candidates participating in an election. It also records votes for each candidate. The program also displays the final vote tallies to determine the winner.

Significance of the Project:
This Python code can simulate an election process while providing a basic understanding of how elections work. A project like this could help students further understand Python and how algorithms work. It also provides a better understanding of the material students learn while taking a computer science course. This code also has real-world applications. When applying this code on a much larger scale it could be used for candidate registration, recording votes, and returning final results. Depending on the application this code can be changed and optimized for its specific purpose.

Installation and Usage Instructions:
This code first starts out by asking the number of candidates you want to add. 
After typing in the number of candidates you would like to add you are then asked to type in the names of those candidates.
After this is done the code then asks you to enter the number of votes to record.
Next, the function recursively asks to enter a vote until the number of votes to record is met. 
Lastly, the code returns the results and prints who won the election with however many votes.

Code Structure:
The code is organized into a class named ElectionBallotCounter with the following methods:
__init__(self): Initializes the candidate's dictionary to store candidate names and their corresponding vote counts.

add_candidate(self, candidate_name): Adds a candidate to the candidate's dictionary, handling duplicate entries.

vote_for_candidate(self, candidate_name): Increases the vote count for a specified candidate, ensuring the candidate exists first. 

tally_votes(self, candidate_index=0): Recursively iterates through the candidate's dictionary, printing the candidate name and vote count in a formatted manner.

winner(self): Identifies the candidate with the highest number of votes and displays their name and vote count as the winner.

add_candidate_interactive(self): This Prompts the user to enter a candidate's name and calls add_candidate for interactive candidate addition.

vote_interactive(self): Prompts the user to enter a candidate's name to vote for and calls vote_for_candidate for interactive voting.

run_election(self): The main driver function that guides the user through the election process, including adding candidates, recording votes, and displaying results.




List of Functionalities and Test Results:

Functionality                               Description                                             Test Results
Add Candidate                               Creates a new candidate entry                           Successfully adds unique candidates
Add Candidate (Duplicate)                   Handles attempts to add existing candidates             Prevents duplicate candidate entries
Vote for Candidate                          Increments the vote count for a candidate               Accurately tracks votes for each candidate
Vote for Candidate (Non-Existent)           Handles attempts to vote for non-existent candidates    Displays error message for non-existent candidates
Tally Votes                                 Prints the election results for each candidate          Presents vote tallies in a clear and organized format
Determine Winner                            Identifies the candidate with the most votes            Accurately identifies the winner based on vote count




Test Results:
Let's start by adding candidates.      

Enter the number of candidates to add: 2

Enter the name of the candidate to add: Pres1
Candidate added successfully.   
Enter the name of the candidate to add: Pres2
Candidate added successfully.
Candidates added. Now, voters can cast their votes.

Enter the number of votes to record: 5

Enter the name of the candidate you want to vote for: Pres1
Vote for candidate 'Pres1' recorded successfully.
Enter the name of the candidate you want to vote for: Pres1
Vote for candidate 'Pres1' recorded successfully.
Enter the name of the candidate you want to vote for: Pres1
Vote for candidate 'Pres1' recorded successfully.
Enter the name of the candidate you want to vote for: Pres2
Vote for candidate 'Pres2' recorded successfully.
Enter the name of the candidate you want to vote for: Pres2
Vote for candidate 'Pres2' recorded successfully.

Election completed Here are the results:

The winner is ‘Pres1’ with 3 votes.



Discussion and Conclusions:

Limitations: 
This simple election simulator, because it’s on a smaller scale, wouldn't be suitable for real-world elections, which require stricter security measures and more comprehensive features (e.g., voter authentication, ballot secrecy, accessibility considerations).

Course Learnings: 
The project demonstrates the application of Python concepts such as classes, dictionaries, functions, user input/output, conditional statements, and loops.

Further Enhancements: 
The code could be extended to incorporate features like handling invalid votes, providing vote-casting options beyond user input (e.g., simulated ballots), and implementing basic 
error-handling routines.

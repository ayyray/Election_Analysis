# Election_Analysis
An analysis of the U.S. Congressional race (Colorado Precinct) using Python

## Project Overview

### Purpose:
In this project, I was using my knowledge of analysis to assist a Board of Elections employee (Tom) with an election audit for a Congressional precinct in the state of Colorado. In order to fully and effectively conduct the audit, I did the following:

- Report the total number of votes cast in the election.
- Report the total number of votes cast for each candidate.
- Determine the percentage of votes for each candidate.
- Determine the winner of the election (based off the popular vote) aka “who had the most votes.”

Once I had completed and submitted the election audit results, the election commission requested more information for the audit. I then went a step further and was tasked with determining:

- The voter turnout for each county.
- The percentage of votes that each county recorded (out of the total vote count).
- Which county had the highest voter turnout.

## Resources:
The audit was conducted accurately using the following resources:

- Data Source (provided): election_results.csv
- Software: Python 3.10.1, Visual Studio Code Version: 1.63.2 (Universal)

## Election-Audit Results:
I gathered the results of the election and wanted to see a breakdown of voter turnout/election results within each county.

- There was a total of 369,711 total votes cast within this congressional election:
    - Jefferson County had 38,855 votes (10.5% of the total votes)
    - Denver County had 306,055 votes (82.8% of the total votes)
    - Arapahoe County had 24, 801 votes (6.7% of the total votes)

![image](https://user-images.githubusercontent.com/96212660/150875937-d57e83b1-f138-46bc-9e14-ae0742b86a4d.png)

![image](https://user-images.githubusercontent.com/96212660/150876027-1d28e778-77ee-46a5-86d3-f52aad7363f3.png)

•	The results of the analysis show that Denver County had the largest number of votes. As stated above, Denver County had 306,055 votes (82.8% of the total votes)

![image](https://user-images.githubusercontent.com/96212660/150876371-80ba9336-6ddd-483e-a1da-885732f43fa4.png)

- The 369,711 votes were cast in favor of 3 candidates:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane

- The results of the elections (per candidate) are as followed:
  - Charles Casper Stockham received: 23% of the votes and 85,213 votes
  - Diana DeGette received: 73.8% of the votes and 272,892 votes
  - Raymon Anthony Doane received: 3.1% of the votes and 11,606 votes

![image](https://user-images.githubusercontent.com/96212660/150876694-5178f266-02a8-487c-a8b1-a6d60d598d78.png)

- The winner of the election based off the popular vote was:
  - Diana DeGette who received: 73.8% of the votes and 272, 892 votes

![image](https://user-images.githubusercontent.com/96212660/150877591-5736dab3-868e-40fc-bd4c-a68bfbf6c851.png)

![image](https://user-images.githubusercontent.com/96212660/150877694-d6bef3d4-fcad-4be7-89b9-7c27dbce5839.png)

## Election-Audit Summary:
I went into the project with the intention of assisting Tom with the Congressional election audit. I was also looking for a way to automate the process for other potential elections! Tom and I wanted to take a process that could be done using Microsoft Excel but take it a step further by automating it and making a more efficient system for analysis using Python. 

I believe the results of my election analysis support my efforts in achieving the goal of increased efficiency and automation when it comes to certifying election results. We chose to use Python because going through Excel can prove to be tedious. 

![image](https://user-images.githubusercontent.com/96212660/150877824-2a59e7db-ed5e-488a-97a4-006c15af4b85.png)

For every vote casted, Excel created a row. That is where Python comes in handy. Using Python allowed me to extract data from an external source (the csv file “election_results”) and easily begin to perform countless operations on the data. 

Operations such as:
- Report the total number of votes cast in the election.
- Report the total number of votes cast for each candidate.
- Determine the percentage of votes for each candidate.
- Determine votes per county
- Determine vote percentages per county

While I was able to use Python to loop through data for a congressional election in Colorado, this script can easily be modified to run any other election!

The code that I have in place simply imported a csv. The csv contained all the data [votes] that was collected using 3 voting methods (Mail-in ballots, Punch cards, and Direct Recording Electronic) and collected in a csv document.

Depending on what data you want to analyze, you can follow the same technique that I used. Let’s say you want to run an analysis on an election for a Presidential election in the United States. Once you have collected the information and entered it into some form of a csv you need to import it into Python:

![image](https://user-images.githubusercontent.com/96212660/150877999-23c1c1ae-b535-48e1-92a7-70d5975db562.png)

I used VS Code instead of the Python interpreter here because it is hard to write longer code and I also wanted to save my code and come back to it!

If I wanted to do an analysis for a Presidential election, I would most likely want to break down my data into states first. In the script for the congressional election, I used the following for determining which county had the largest turnout:

![image](https://user-images.githubusercontent.com/96212660/150878237-5a3a5b1c-f917-4d92-991c-789c8c8f2207.png)

I created an empty string to hold the values of the county names, and I created a variable that would hold the values of the votes within the county. The code might look like:

![image](https://user-images.githubusercontent.com/96212660/150878391-9923f350-78e9-4d8b-8c7d-3521f9451ba4.png)

If you want to track a state progress/vote count by state you would use the same formatted if statement:

![image](https://user-images.githubusercontent.com/96212660/150878451-7695513d-8825-4624-8eb1-6df2030c65b8.png)

**(Be advised that in order for this loop/if statement to work, you want to create a state list and state dictionary ahead of time:**

![image](https://user-images.githubusercontent.com/96212660/150878480-a324fb2b-4ab8-4c24-8630-7b9e390be910.png)

**and you want to make sure you are setting the total vote count equal to zero whether it is applicable to the candidate vote count or the state vote count).**

I believe the results of the election analysis combined with the added #comments to my code are a great foundation in utilizing this script for further elections and their analysis!








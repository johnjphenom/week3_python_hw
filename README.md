# PyPoll with Python

## Overview of the Project

### Purpose

The goal of this module and challenge is to assist Tom, a Colorado Board of Elections employee, with an election audit for a specific U.S. Congressional precinct in Colorado. In this case the process is usually done in Excel, but the hope is to automate this instead. The tool that will be used to accomplish this is Python. The hope is that if successful, this code will be utilized in not only other congressional elections but all also those that are senatorial and local elections.

The tabulated voting results which are the sum total of mail-in ballots, punch card ballots, and direct recording electronic ballots are available in a CSV file. These results will be analyzed through code generated in Python. The following metrics were initially requested:

Total Votes for the Election
Total Votes for Each Candidate
Percentage of Votes for Each Candidate
The Winner of the Election Based on the Popular Vote

After the successful development of the code and the results being provided to the board, they wanted the additional information as well:

The Voter Turnout for Each County
The Percentage of Votes from Each County Out of the Total Count
The County with the Highest Turnout

The project was completed to the satisfaction of the Colorado Board of Elections

## Election-Audit Results

The election results were clear and verified versus the provided proof. Below are the screenshots in both the terminal in VS Code and in the election_analysis.txt file.

  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/terminal_screenshot.jpg)
  
  
  
  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/notepad_screenshot.jpg)



The results are laid out as follows:

* Total Votes are 369,711.
  
  This was calculated with the following code:
  
  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/total_votes.jpg)
  
* County Votes and the Vote Percentages are as follows:
  Jefferson: 10.5% (38,855 votes)
  Denver: 82.8% (306,055 votes)
  Arapahoe: 6.7% (24,801 votes)
  
  This was calculated with the following code:
  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/high_county.jpg)

* Denver was the county with the largest number of votes.

  This was calculated with the code in section #6f in the image directly above.
  
  
* Candidate Vote Counts and Vote Percentages are as follows:
  Charles Casper Stockham: 23.0% (85,213 votes)
  Diana DeGette: 73.8% (272,892 votes)
  Raymon Anthony Doane: 3.1% (11,606 votes)
  
  This was calculated with the following code:
  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/candidate_results.jpg)
  
* Diana DeGette won the election with a Vote Count of 272,892 and 73.8% of the total votes.

  This was calculated with the following code:
  ![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/winning_candidate.jpg)


## Election-Audit Summary

The Python script that was developed was proved to be a well thought out and efficient automated way to analyze tabulated election results. The code written is such that it can be utilized for other elections as successfully as it was in this situation. It can accurately determine the number of and name of counties and candidates. It can also provide the number of votes for each of these and their corresponding percentages as well.

There are a couple of areas that might need modification in the future for different elections.

One example is the choosing of which location to retrieve the data from. In this case the county name could be found in the second column and the candidate’s name in the third. There may be a time where these are found in different columns depending on the CSV provided. It is a quick and easy fix and only requires changing the numeric indicator in the following code.

![This is and image](https://github.com/johnjphenom/week3_python_hw/blob/main/Resources/row_selection_code.jpg)

Another example is a simple one. Right now, all our descriptors are based on counties, but there may be a local election that needs to be evaluated. In this case checking counties may not be appropriate but rather individual precincts would work better. The variables could be altered and the place where information is printed would need to detail 'precinct' and not 'county'.

Overall, the script is well equipped to parse through and analyze data for a multitude of elections. It clearly and accurately provides information about overall votes, candidate votes and their percentages, county votes and their percentages, and metrics on the winner.

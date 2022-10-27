# Election_Analysis

## Project Overview

The goal of this project is to give the vote totals and winner of a recent election in Colorado. We looked at five specific categories 

1. Total votes cast.
2. Candidates who received votes 
3. Vote totals for each candidate 
4. Percentage of votes for each candidate
5. Overall winner 

## Resources

-Data Source: election_results.cv
-Software: Python 3.7, Visual Studio Code 1.72

## summary

The analysis of the election shows that:
1. 369,711 total votes were cast. 
2. The candidates were Charles Casper Stockham, Diana DeGette, and Raymoan Anthony Doane.
3. Charles Casper Stockham received 85,213 votes, Diana DeGette received 272,892 votes, and Raymon Anthony Doane received 11,606. 
4. Charles Casper Stockham received 23.0% of total votes, Diana DeGette had 73.8%, and Raymon Anthony Doane had 3.1% 
5. Diana Degette won the election with 73.8% of all votes for 272,892 total.
  
## Challenge Overview
The challenge required analyzing the votes by the county they were cast in looking at similar categories of information as we had in the election audit. 
1. Total votes cast across all counties
2. Counties involved in this election.
3. Total votes cast in each county. 
4. Percentage of voters in each county.
5. Identifying the county with the largest number of voters. 

## Challenge Summary 
The analysis of county voters shows that 
1. 369,711 Votes cast
2. The three counties involved were Jefferson, Denver, and Arapahoe
3. Jefferson had 38,855 voters
   Denver had 306,055 voters 
   Arapahoe had 24,801 voters 
4. Jefferson had 10.5% of all voters 
   Denver had 82.8% of all voters
   Arapahoe had 6.7% of all voters 
5. Denver had the largest turnout

## Further Uses 
This code is flexible enough for several changes the most immediately obvious would be that it can be used to analyze the information from any future state level election.
For local elections a simple change to County reference seen below
'''
# Print the final vote count (to terminal)
    election_results = (
        f"\nElection Results\n"
        f"-------------------------\n"
        f"Total Votes: {total_votes:,}\n"
        f"-------------------------\n\n"
        f"County Votes:\n") 
'''
To something representative of the area covered 
'''
# Print the final vote count (to terminal)
    election_results = (
        f"\nElection Results\n"
        f"-------------------------\n"
        f"Total Votes: {total_votes:,}\n"
        f"-------------------------\n\n"
        f"Township Votes:\n")
'''
Allows us to reuse almost the entirety of the code with only a miniscule change for clarity in the final output. 
We could also make a useful but more complicated alteration in the code to see each candidates total votes by county. At the basic level this would mean adding code similar to what we had in the [](pypoll.py) but adding inside the for loop an if elif statement that isolates the information for each county and then adding the apporpriate print outputs for each county. 
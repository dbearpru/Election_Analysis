# Election_Analysis
Overview of Election Audit

Purpose

The purpose of this audit is to find the winner of the election and the voter turnout in each county.


Election Results and code

1.Total Votes: 369,711
 This is the function in the first for loop to get the total votes.
 total_votes = total_votes + 1

2. County Turnout
 We first had to loop the county names to make sure we had all the counties invovled. Then we looped for the vote count by county. 
 Lastly we ran a function for percentages to show how much of the vote each county contributed. 
Jefferson: 10.5% (38,855)
Denver: 82.8% (306,055)
Arapahoe: 6.7% (24,801)

3. Shows county with largest Turnout
  Later in the loop we ran if(votes>county_turnout):
            county_turnout= votes
            largest_county=(f"-------------------------\n"
                            f"Largest County Turnout: {county_name}\n"
                            f"-------------------------\n")
  to get the county with the most votes counted. 
    
Largest County Turnout: Denver

4. Vote Count and Percentage by Candidate

I essentially did exactly what we did for county counts but changed the variables to make it show candidate names, percents, and vote count. 

Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,892)
Raymon Anthony Doane: 3.1% (11,606)

5. Winner Calculations
Very similar to the largest county turnout. Instead we had to list 3 seperate variable if our if statement was correct. 
 if (votes > winning_count) and (vote_percentage > winning_percentage):
            winning_count = votes
            winning_candidate = candidate_name
            winning_percentage = vote_percentage
Winner: Diana DeGette
Winning Vote Count: 272,892
Winning Percentage: 73.8%

You could easily use the same script for a different years election. You would need to change the  file_to_load = os.path.join("Resources", "election_results.csv") function. You would replace the elections_results.csv with the current years results and the script should still run fine as long as your headers remained the same year to year. You could also use it for completely different counties in a different state. It would be again a change in your file to load. If headers where different you change you variables after looking at the rows. 

# Election_Analysis

## Overview
I was tasked with helping a Colorado Board of Elections employee. They wanted me to perform an audit on their most recent election. The audit consisted of some of the steps below along with repeating that process with the different counties involved in the election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who recieved votes.
3. Calculate the total numbner of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources
- Data Soure: election_results.csv
- Software: Python 3.8.3, Visual Studio Code, 1.63.2

## Election Results
    1. The total number of votes in the election was 369,711
    2. There were only three counties that participated in the election.
        - Jefferson county had 38,855 or 10.5% of the total number of votes.
        - Denver county had 306,055 or 82.8% of the total number of votes.
        - Arapahoe county had 24,801 or 6.7% of the total number of votes
    3. Denver had the most voter turnout with 82.8% of the total number of votes
    4. There were only three candidates that were running in the election.
        - Charles Casper Stockham who received 85,213 or 23.0% of the total number of votes
        - Diana DeGette who received 272,892 or 73.8% of the total number of votes
        - Raymon Anthony Doane who received 11,606 or 3.1% of the total number of votes
    5. Diana DeGette won the election by a landslide receiving 272,892 or 73.8% of the total number of votes.

![Election_results_image](https://user-images.githubusercontent.com/95730434/149769759-4520f88b-968a-49a0-bb5e-2186bc527ba4.png)

## Summary
Although this code works great for a small election like the Colorado election, the code would need to be adjusted for a different scaled election. When looking at a local, district, state, or national election the base code is a good starting point. The easiest way to adjust for any election would be to start with the county part of the code.

![county_code](https://user-images.githubusercontent.com/95730434/149772343-38fd3f0c-7ad8-45ff-b939-2b4fa611d78c.png)

When looking at this code the variables would need to changed to adjust for different states, regions, or groups of people based on the level of the election. Any part of the code with "County" would need to be changed to an alternative variable. 

The other way to change the code is to be more specific with the code. Meaning we got lucky and did not have any issues with our data which is not always realistic. In a bigger election there might be outliers, missing votes, and much more that our code does not account for. So to make this code better for all elections I would propose adding more code that comb through all the data and confirm there are not issues. Once that is determined then the code can be run to determine the results and analysis of the election.
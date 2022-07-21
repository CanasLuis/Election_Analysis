# Election_Analysis
##Overview of the Project
The main purpose of this project is to help Set and Tom with and analysis of the election results. We are given with the total votes of each county and candidate. However we want to obtain the winner and the percentage rate of votes that each candidate receive. In addition, we want to have the votes per county and the largerst tournout, which means, the county that had the most votes participation. 
With that being said, we are going to use different tools in Python like loops and condititonals with a few of math operations in order to get the total votes and the total votes each of the candidates received, with the percentage. After that, we can put the results in a txt file which will make it more easy to read and witth good presentation.

##Election Audit Results
As mentioned, we are given a data base with the detail of votes for every candidate and in which county was the vote, we have a total of 369,711 votes. Taking a brief look at the data base, we can see that we have 3 candidates and 3 countys, as follows:

-Candidates: Charles Casper Stockham, Diana DeGette and Raymon Anthony Doane
-Countys: Jefferson, Denver and Arapahoe

The summary results for each of the candidates and countys, are:

###For candidates:
-Charles Casper Stockham: 23.0% (85,213)
-Diana DeGette: 73.8% (272,892)
-Raymon Anthony Doane: 3.1% (11,606)

We can see that Diana has almost 74% of the total votes, which means she is the winner of the election. In the other hand, Raymon has a very low votes participation with only 3.1%

###For countys:
-Jefferson: 10.5% (38,855)
-Denver: 82.8% (306,055)
-Arapahoe: 6.7% (24,801)

More than 82% of the votes came from Denver, whilst Arapahoe had the lowest participation with just 6.7%.

This Summary was printed in VS terminal after the run and wrote in a txt file to make it easier to read and analyse, here are some prints of how it looks in each one of them:

Terminal
![Summary in terminal, elections](https://user-images.githubusercontent.com/108499271/180268070-afbb59e8-1dc4-45ea-a7c9-15248b85b310.png)

Txt file:
![Summary elections ](https://user-images.githubusercontent.com/108499271/180268123-8d023d05-a2dd-484f-857a-969f7d9ef876.png)


##Election-Audit Summary:
The code we used for this analysis can be used for any other election analysis, but we would have to make some updates, explained below:
-The data base has to be updated or saved in the same folder we have the input for the current analysis, in csv format. 
-If the neew data base has a differentt name, we have to update it in the code, at the beginning of it (currently named as "election_results"): 
  # Add a variable to load a file from a path.
  file_to_load = os.path.join( "Resources", "election_results.csv"
-We also have to be sure that rows where the name of the candidate and county are correct, for this process we used column 3 and 2 of the csv:
      # Get the candidate name from each row.
        candidate_name = row[2]

        # 3: Extract the county name from each row.
        county_name = row[1]
        
 -Finally we have to decide if we want the txt file to be named the same ("election analysis") or change it, if we change it, it also has to be updated in the code:
  # Add a variable to save the file to a path.
  file_to_save = os.path.join("analysis", "election_analysis.txt")

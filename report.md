# Most Americans Vote No on Split-Ticket Ballots
#### By: Anusha Datar
#### 05/07/2020

While political campaigns and media coverage tend to focus on individual
candidates, voters consider ballots with multiple elections when they are at
the polling booth. At the polling booth, voters can either opt for straight
ticket voting, where they vote exclusively for members of the same political
party, or split ticket voting, where they vote for members of different parties
on the same ballot. While rates of split-ticket voting have always been low, they
have declined recently. 

To characterize the prevalence of split-ticket voting, I use the ANES (American 
National Election Studies) dataset. ANES is a product of a National Science 
Foundation-funded collaboration between Stanford University and the University of
Michigan, and its goal is to [“[produce] high quality data from its own surveys 
on  voting, public opinion, and political participation.”](https://electionstudies.org/about-us/)
It contains both pre and post election survey results from voters for every
general and midterm election year between 1948 and 2016.

Each post-election survey asks each participant to report the party
identification of the candidate they selected for president, congressional
representative, and senator. It also asks them to report their political
affiliation, asking “Generally speaking, do you usually think of yourself as a
Republican, a Democrat, an Independent, or what?” If they choose Democrat or
Republican, they specify whether or not they identify strongly with their party.
If they select Independent, they note whether they lean towards a particular
party (and if so, they report which party they prefer) or if they are completely
Independent. 

For each year, I classify each respondent’s voting record based on its 
consistency along party lines. If a participant reports voting for a candidate
from the same party for all national-level roles available to them, I label
their ballot with the party they voted for (“Democrat Ballot” and “Republican
Ballot”). If they voted for candidates from a specific party more than the other,
I labeled their ballot as leaning in the direction of that party
(“Democrat-Leaning Ballot” and “Republican-Leaning Ballot”). If they vote for
exactly the same number of candidates from each party, I mark that their ballot
is exactly split (“50/50 Split Ballot”).

After classifying all of the respondents, I plot the percentage of respondents 
in each group (Democratic Ballot, Republican Ballot, Democrat-Leaning Ballot,
Republican-Leaning Ballot, and 50/50 Split Ballot) from 1948 to 2016. 

![Ballots over Time](/plots/all-ballots-over-time.png)

Straight-ticket voting has always been the most common option voters opt for. 
That being said, between 1948 and 1980, split-ticket voting was becoming more
common as straight-ticket Republican ballots decreased in frequency and
straight-ticket Democrat ballots stayed about the same. However, after 1980,
the prevalence of both Democrat and Republican straight ticket ballots has
either increased in frequency or has stayed about the same, and the proportion
of voters at least leaning towards a particular party has also slightly increased.

To see the effect of personal political party identification on voting decisions,
I further categorize the respondents by political party - if they explicitly
identify as a Democrat, Republican, or Independent (all Independent voters who
leaned towards a political party are still labeled Independent). I then look at
the proportion of the individuals who identify with each political party group
that fall into each of the ballot groups. 

![Democratic Ballots over Time](/plots/dem-ballots-over-time.png)

![Republican Ballots over Time](/plots/rep-ballots-over-time.png)

![Independent Ballots over Time](/plots/ind-ballots-over-time.png)



All three political affiliation groups have high rates of straight-ticket voting
which have either increased or remained about the same over the last 30 years.
Democrats have a consistent rate of straight-ticket voting, while Republicans
practiced increasing amounts of split-ticket voting until 1980, at which point
their rate of straight-ticket voting started to increase. Even the majority of
Independents have increased their frequency of straight-ticket voting,
Especially in the last 30 years. 

The recent decline of split-ticket voting suggests that political polarization
has followed voters all of the way to the ballot box, regardless of party
affiliation. 

Check out the portion of the dataset used and analysis of the code in this 
[notebook](https://colab.research.google.com/github/anushadatar/split-ticket/blob/master/Analysis.ipynb).

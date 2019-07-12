At this repository you will find the files describing the instances of the *Football Team Composition Problem with endogenous uncertainty* used in the article G. Pantuso **A node formulation for multistage stochastic programs with endogenous uncertainty** (in what follows **Pan19**).
The instances have been adapted from those used in the article G. Pantuso **The football team composition problem: a stochastic programming approach**, Journal of Quantitative Analysis in Sports, 2017 (**Pan17**) and available at https://github.com/GioPan/instancesFTCP.

This repository contains 20 instances, one for each team in the English Premier League 2013/14, that is ARS, ASV, CAR, CHE, CRP, EVE, FUL, HUL, LIV, MAC, MAU, NEC, NOR, SOU, STO, SUN, SWA, TOT, WBA, WHU. In addition, a file is provided with the default parameters used in Pan19. The files are explained below.

# Teams
Each focal team is described by two text files (.txt). One file contains the joint list of current and target players in the focal team and is identified by an appended "p", as in "arsp.txt" for the case of Arsenal FC. The second file contains a number of possible team compositions, and is identified by an appended "t", as in "arst.txt".

Players files, (*p.txt) are organized as follows.
First line:
- name of the team (String).
From the second to the last line, each line contains:
- Player name (String)
- Age (Integer)
- Current market value (Float)
- Role (String)

Team compositions files (*t.txt) are organized as follows.
First line:
- Number of team compositions provided (Integer)
- Budget of the team (Float)
Then, for each team composition:
First line:
- Name of the team composition (String)
Second line:
- List of players in the team composition (Strings).

# Parameters
The [parameters file](./params.txt) contains the necessary parameters to determine salaries and transition costs from a team composition to another. The file is self-explanatory following the headers.


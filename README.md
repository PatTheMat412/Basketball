# Basketball betting project
A project im currently working on for fun using machine learning algorithms to predict outcomes of games of the 2024-25 NBA season. Also simulated the use of the Kelly criterion which is usually used in financial analytics as a way to optimize betting strategy. I understand that I have nowhere near the expertise of data analysts at top sportsbooks so finding an edge will likely be impossible with my current knowledge of machine learning. However, I wanted to start this project as it seems like something I can keep adding to as I get more experienced, and also just because I like basketball.

# Data
The data I found was quite pleasurable to work with, there werent really missing values and it was quite extensive. It was however, in the format of individual player statistics which is not very useful for creating features. I ended up first grouping stats by teams so that I can merge with the other dataset which had, among other things, info about the winner, date, and location of the game.

# Plan
The high level overview of this project is to first create features that minimize data leakage such as rolling features, then train a model to predict the outcomes of games. Secondly, to compare the probabilities that my model computed against the probabilities the sportsbooks computed. By comparing the probabilities, we can compute whether a game could be potentially profitable. After the model has determined if the game is profitable, we use the kelly formula to compute the exact amount from our bankroll we should bet in order to maximize return. 

# Future changes
- most important thing I currently need to do is somehow obtain data about the moneyline odds of games from the 2024-25 season to use as my odds_list parameter for the Kelly function. This likely will have to be done by web scraping as I havent found any datasets for moneyline odds. 
- If I want to use this model to pretend bet on games happening in the 2025-26 season, I would need to siphon data from the NBA api which I am not sure how to do.
- Will add more features. CUrrently only using rolling stats from the previous 5 games.
- Playing with hyperparameters. Currently the nearest neighbors model is showing the highest accuracy which makes sense since this model does well with smooth data such as rolling data. 


### DISCLAIMER: I am not of legal gambling age in my state therefore I am working on this just for fun. As well, I do not condone any sort of gambling.


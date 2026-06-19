# Pokemon Data Analysis
In this project, I applied what I learned from Harvard's online Introduction to Data Science with Python as well as from reading Practical Statistics for Field Biology to analyze my own pokemon ranking data through python. I specifically focused on using Pandas, MatPlotLib, and Scipy to manipulate, graph, and analyze this data. However, I also used statsmodels to practice using a tukey test. 
## Data
The data for each pokemon mostly came from the [unofficial pokemon database](https://pokemondb.net/tools/text-list) which was copied into a spreadsheet. However, various columns such as stage, generation, and legendary/mythical were added to provide more data to analyze. Finally, the scores or rankings for each of the pokemon came from my own personal opinion. 
## Process
First, this spreadsheet was loaded into a pandas dataframe and the data was cleaned up. Some columns were removed and others were edited so that the data would be easier to graph and analyze. Next, I practiced graphing the data in various ways using the different types of data I had on each pokemon. The most helpful plots to look at were the box plots which showed the overall spread of the data. Here is one example where I did a boxplot on the generation of the pokemon and their rating:
<p align="center">
<img width="583" height="461" alt="download" src="https://github.com/user-attachments/assets/e5471a07-751e-4a34-9ad0-e173d0e7d4f2" />
</p>
It was also helpful to use groupby to get the means of the various things I was looking at and plotting those as well. After this, I practiced doing statistical tests in python by comparing different groups of data such as types or generations. For example, since I showed the generation graph above, I did a t-test on generations 1 and 9 to determine if the difference was statistically significant. The p-value came out to be 0.68 meaning that there was no significant difference between these two generations. Even so, I did an anova to compare all of the generations together and ended up with a significant p-value of 0.0003, leading me to do a tukey test on all of this data to look at the significance of each generation. I repeated this process a few other times looking at the significance between pokemon types, stages, and if they are legendary or not. 

 

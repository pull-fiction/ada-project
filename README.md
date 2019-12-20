# Make crops, not war

Milestone 3 update.

- Data story: [https://pull-fiction.github.io/make-crops-not-war/](https://pull-fiction.github.io/make-crops-not-war/)
- Notebook: [project.ipynb](project.ipynb)

## Detailed contribution

- Michael Blackburn: data wrangling, general analysis, agriculture map, buildings map
- Edoardo Debenedetti: data wrangling, general analysis, war events map, Beirut population
- Maksim Kriukov: data exploration, specific crops production changes, production change motivations
- Simona Leserri: data exploration, specific crops production changes, production change motivations

The analysis has been done jointly by everyone with equal contributions.

## Abstract

The impacts of war on a country’s economy, social structure and politics are generally well documented and understood. However, impact on food and crop production has not been studied to the same extent. Through a brief literature research, it has been found that most papers about the topic are quite outdated. Our intention is to fill in this gap through an analysis of the UN Dataset on Food Production in conjunction with war data obtained through WikiData and the UCDP Armed Conflict Dataset. The increased globalization of food markets along with the amount of significant armed conflicts that have occured in recent years lead us to believe that there are interesting discoveries to be made. For the scope of our project, we will look into wars that occured in Afghanistan and Lebanon.

## Research questions

- How have wars impacted the production of crops and livestock in Afghanistan and Lebanon? 
  - We chose to only focus on crops and livestock as the data on import/export had too many missing data points. We will focus on a small number of countries as each war in order to obtain meaningful results. Wars are too unique and have too many variables to obtain meaningful results by attempting to generalize over a large quantity of them. It would not be feasible to accomplish this within the context of this project.
- What is the difference in the two wars that occured in Afghanistan and why did they have opposite effects on crop/livestock production? Did the fact that the war in Lebanon was a civil war have an impact different from those in Afghanistan, which included outside actors?
  - Here, we will categorize the wars we selected by state and non-state actors and severity which will be based on amount of casualties.
- Have the impacts of war within these countries caused long lasting effects? We will compare rates of growth before, after and during the wars in addition to comparing with general worldwide trends.
  - In our initial plan, we wanted to see if changes if one countries production impacted others, but we have decided to not follow this path. Although it would have been interesting, we believe that we will obtain better results by analysing more thoroughly a smaller set of variables rather than less depth with a larger set.

## Dataset

- [Global Food & Agriculture Statistics](https://www.kaggle.com/unitednations/global-food-agriculture-statistics): we are using this dataset to see how agriculture changed before, during and after wars (e.g. crops and livestock production)
- [Wikidata Query Service](https://query.wikidata.org/): We are using this dataset to obtain information about wars (e.g. place, actors involved, start and end dates). Initially, we were only going to use the Uppsala dataset for this purpose, but we found Wikidata to have more complete and relevant information. The query we are making can be found in [get_wiki_data.py](src/get_wiki_data.py) file.
- [Uppsala Conflict Data Program/PRIO Armed Conflict Dataset](https://ucdp.uu.se/): We will now only refer to this dataset as a complement to the data we obtained using Wikidata. It contains interesting data about the severity of different armed conflicts that may be useful when categorizing the wars which we will analyse.

## A list of internal milestones up until project milestone 3

- Finalize any correlations we have chosen for our data story (deadline 05.12.19)
  - Further analyse Afghanistan and Lebanon based on how they were affected by wars.
  - From these countries, determine causes of the correlations we are seeing.
  - Categorize each war of interest in the selected countries.    
- Data story write-up and visualization creation (deadline 16.12.19)
  - Create meaningful visualizations of the correlations we found.
  - Write the story.
- Create article to tell our story. (deadline 19.12.19)
  - Present our visualization and story in the format of our choice.
- Final review of data story and submission (deadline 20.12.19)
  - As a group, final review of our story.
  - Submit Milestone 3

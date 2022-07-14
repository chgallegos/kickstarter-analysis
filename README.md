# kickstarter-analysis
Project deliverable for Module 1 Data Analytics Bootcamp

### Overview: This is an analysis of kickstarter funding efforts while leveraging important factors that could significantly affect the funding outcomes

### Purpose: The purpose of this analysis is to recognize funding outcomes based on timing and funding goals in order to advise LouseÕs upcoming fundraising efforts for putting plays together

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The first part of the analysis was to create a picot table which was arranged and filtered according to outcomes and launch date. 

### Analysis of Outcomes Based on Goals

The second part of the analysis involved the use of COUNTIF functions, the challenge was to figure out the correct conditions to set up the ranges (<> or <= =>). 

----

### Challenges and Difficulties Encountered

#### Theater Outcomes by Launch Date Challenges

For the Pivot table portion of Outcomes based on Launch date. The main challenge was to group the months of the year together, as the table initially had a year subdivision once the rows were expanded. I was able to group into years by tight clicking and choosing the option to group

#### Outcomes based on Goals Challenges

On the Second part of the analysis, the graph was not quite accurate, which brought me to review the formula (which did end up having an error) After looking at the problem, I stepped back and realized that the instructions requested another piece of criteria, which was to limit the counts to only plays, the code used for COUNTIFS is the following: 

=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$Q:$Q,"plays",Kickstarter!$D:$D,"<1000")

----

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? There is a higher probability to have a successful campaign if this is launched towards the middle of the year. 

A conclusion can be drawn that there seems to be a drop in both successful and failed campaigns between September and November (refer to image below)

![Screenshot](Theater_Outcomes_vs_Launch.PNG)

- What can you conclude about the Outcomes based on Goals?

It seems like the Ôsweet spotÕ range that could have a good probability for a successful funding is between $35,000 and $50,000.(refer to image below)

![Screenshot](Outcomes_vs_Goals.PNG)

- What are some limitations of this dataset?

More relevant data could be included, I would recommend including the name of the actors that will be involved in the play as certain names can quantify returns at the box office at least by approximation. It would also be helpful to know the ROI of the plays and projects involved in the dataset.

- What are some other possible tables and/or graphs that we could create?

We could create also a table and graph that shows outcomes based on subcategories and time of the year. This could show how the category/genre of a play could affect the outcome of its funding as some genres can be more popular at different times of the year

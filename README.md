"# ada-2020-project-milestone-p3-p3_ada-boi"

**Title: Influence of housing conditions on education, health and happiness**  

**Abstract**  
While the original paper explores the effects of a treatment (Piso Firme program) on children health and household happiness, it fails to take into account the default conditions: how is the health of certain demographics impacted by their living and housing conditions. We propose to study the effect of housing on certain indicators, such as happiness, health and education. To do so, we plan on using the National Survey of America's Families (NSAF), which recenses a large number of households throughout the USA, along with the demographics and health parameters of the inhabitants.\
From this dataset we can extract a number of interesting variables for housing conditions and environment (such as size, crowding, income, living arrangement, social programs, etc), happiness (e.g. mental health scale, social behavior), health (e.g. current status, doctor visits) and education (e.g. school engagement, performance, absenteeism).


**Research questions**
1. Which life outcomes do general housing conditions influence the most (education, happiness or health)? 
2. Is there a correlation between precarious housing and health (both physical and mental) status?
3. In what ways do living conditions affect children scholarship (if they do) ? Which age group is most impacted ?

**Proposed dataset**\
Urban Institute, and Child Trends. National Survey of America’s Families (NSAF), 2002. Inter-university Consortium for Political and Social Research [distributor], 2007-10-03. https://doi.org/10.3886/ICPSR04582.v1 \
We chose the 2002 census as it represents a similar timeframe to the Piso Firme project, which probably helps to smoothe out potential period-related discrepencies (for example, maybe the 2008 crisis had an effect on the relationships we want to determine, and taking a post-2008 census would be misleading).\
We will restrict our study to the Focal Child Data and the Household Data.

**Methods**\
We will divide the children in three age groups in order to study which group is influenced the most for different parameters. Each person of interest will be linked to his/her household.\
The idea is first to do some visualization of the data for the variables of interest. Then, we will perform linear regression in order to study in more details the impact of different housing variables on schooling, health and happiness.
We are also planning on using a propensity score matching (PSM) in order to evaluate certain treatment effects on subpopulations.

**Proposed timeline**
- Data pre-processing
- Data visualization
- PSM
- Regression models
- Results analysis & presentation

**Organization within team**  \
Estelle : population matching, health/happiness data \
Alan : propensity score establishment, education data \
We will also regularly review each other's work and add ameliorations if needed.

**Questions for TAs**  
None

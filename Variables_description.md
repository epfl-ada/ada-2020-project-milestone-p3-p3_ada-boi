#### Recapitulation of all the variables resulting from the data processing.  
#### NB the variables in _`italics`_ were implemented by us from given variables.  
# Dataset 1: household data
`HHID`: Household ID number  
`CHLD0_5`: Number of children ages 0-5 in household   
_`bool0_5`_: Does the household have at least one child aged 0-5? **1** if `CHLD0_5` > 0, **0** if `CHLD0_5` = 0   
`CHLD6_17`: Number of children ages 6-17 in household  
`UHHCOUNT`: Total number of people in household  
`MNBEDRMS`: Number of bedrooms  
_`OVERCROWDING`_=`UHHCOUNT`/`MNBEDRMS`: People per bedroom, related to overcrowding of the household.   
`QSC5`: Household total income as a function of twice the poverty line, boolean, **0**=income below 2x poverty line, **1**=income above 2x poverty line   
`MOWNRENT`: Household ownership, **1**=owned, **2**=rented, **3**=no payment  


# Dataset 2: Focal child data  
### 2.1) General information
`HHID`: Household ID number  
`PERSID`: ID of person interviewed   
`PERSTYPE`: Person type, **1**=focal child aged 0-5, **2**=focal child aged 6-17  
`SEX`: Sex, **0**=M, **1**=F  
`UAGE`: Age of the child   
`STATE`: US state  
`UREGION`: US region; Northeast, Midwest, South, West 
### 2.2) Education 
`UENG`: Engagement at school (takes into account the general interest given to school, homework completion, etc...), score in **[4-16]**, with **4** the lowest and **16** the highest engagements  
_`UENGn`_: Normalized engagement at school, score in **[0-1]**  
`UENGNEG`: Index of negative engagement at school, **0** if `UENG`>10, **1** if `UENG`<=10  
`UENGPOS`: Index of positive engagement at school, **0** if `UENG`<15, **1** if `UENG`>=15   
`NLESSONS`: Did the child take lessons after school last year? **0**=no, **1**=yes  
`CSPECED`: Does the child receive special education services? **0**=no, **1**=yes  
### 2.3) Family variables
`UFAMSTR`: Living arrangement of child, **1**=lives with no parents, **2**=lives with single parent, **3**=lives in a blended (step) family, **4**=lives with two biological/adoptive parents  
`UMHIGDEG`: Parent's highest educationnal degree, in **[1-6]**, with **1**=GED, **2**=high school diploma, **3**=technical certificate, **4**=associate degree, **5**=bachelors degree, **6**=graduate or professional degree   
`UAGG`: Parent aggravation score (how difficult is it to care for the child), in **[0-12]**, with **0** being really easy and **12** really difficult  
_`UAGGn`_: Normalized aggravation score, score in **[0-1]**   
### 2.4) Income/security variables
`U_SOCPOV`: Social family income as % of poverty line, **0.5**=Family income < 50% of pov line, **1**=50%<=family inc<100% of pov line, **1.5**=100%<=family inc<150% of pov line, **2**=150%<=family inc<200% of pov line, **3**=200%<=family inc<300% of pov line, **4**=Family income >= 300% of poverty  
`UHINS4`: Insurance provider, **1**=Employer, **2**=Medicaid/State/CHIP, **3**=Other, **4**=Uninsured  
### 2.5) Physical health variables
`BDISBL`: Child has a disability that limits activity, **0**=no, **1**=yes  
`BHLTHN`: Child's current health status, a higher score means poor health status, **1**=excellent, **2**=very good, **3**=good, **4**=fair, **5**=poor 

_`BHLTHNn`_: Normalized child health status, in **[0-1]**, where **0** means very healthy and **1** vers unhealthy  
### 2.6) Mental health variables
`UBPIA`: Age 6-11 Behavioral Problems Index score, in **[6-18]**, A higher score indicates fewer behavioral problems    
_`UBPIAn`_: Normalized age 6-11 Behavioral Problems Index score, in **[0-1]**  
`UBPIANEG`: Negative behavior 6-11 years, **0** if `UBPIA`>12, **1** if `UBPIA`<=12  
`UBPIAPOS`: Positive behavior 6-11 years, **0** if `UBPIA`<18, **1** if `UBPIA`=18   
`UBPIB`: Age 12-17 Behavioral Problems Index score, in **[6-18]**, A higher score indicates fewer behavioral problems    
_`UBPIBn`_: Normalized age 12-17 Behavioral Problems Index score, in **[0-1]**  
`UBPIBNEG`: Negative behavior 12-17 years, **0** if `UBPIA`>12, **1** if `UBPIA`<=12  
`UBPIBPOS`: Positive behavior 12-17 years, **0** if `UBPIA`<18, **1** if `UBPIA`=18  
`NCPROBC`: Has the child been sad or depressed this month, **0**=never, **1**=sometimes true, **2**=often true  
_`NCPROBCn`_: Normalized child depression index, in **[0-1]**, where **0** is 'never depressed' and **1** 'often depressed'  
`UMH2`: 100 point mental health scale for the parent, in **[25-100]**, a higher score indicates better mental health of the parent  
_`UMH2n`_: Normalized parent mental health scale, in **[0-1]**, a higher score indicates better mental health of the parent  
### 2.7) Activities
`UACT`: Extent of child's extracurricular activities, enumerates the number of types of activities a child has been involved in the last year. Includes sports, lessons, youth group or student government, drama, band or chorus, religious or community group, scouts. in **[0-3]**   
_`UACTn`_: Normalized extent of child's extracurricular activities, in **[0-1]**, where **0** means not active and **1** means extremely active  

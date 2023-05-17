# PORTFOLIO: Data Analyst

## ABOUT ME
Hello! My name is Valeria, and I'm starting my career as a data analyst. In this repository you can find some of my work so far. 
I sure loved working on those projects, so I hope you like reading my review!

## SKILLS & SOFTWARE
- Data analysis tools: `SQL`, `MS Excel`
- Database Management Systems: `MySQL`, `PostgreSQL`
- Data visualisation tools: `PowerBI`

## PROJECTS
### Case Study 1: Analysis of Student Balance Changes
Project for an online English school. They asked to look at how student balances (ratio of transactions and classes) was changing through time. 

#### Tasks
1. Use SQL queries to pull a table with data on student balances for each student for every day of the period.
2. See how each student's balance was affected by transactions and classes.
3. Analyse data on student balance changes pulled from the DB and discuss possible issues with data engineers and DB owners.
4. Visualise all the data and draw conclusions.

#### Solution
I worked with two DBs, `CLASSES` and `PAYMENTS`, and wrote a query using CTEs to get all the data required for the analysis. I needed to pull data such as the first transaction date for each student; a list of all dates for each student that are relevant to keep track of their balance; all balance changes (+ cumulative ones) for each student on each date (for transactions and classes), balance changes across the whole school for each date.

> <a href="https://github.com/Melifarro19/Valeria-Dzhukich-Portfolio/blob/main/Case%20Study%201/SQL%20Query">SQL Query</a>
<br> Here is a part of the final SQL query for reference.

#### Graphs
> <a href="https://github.com/Melifarro19/Valeria-Dzhukich-Portfolio/blob/main/Case%20Study%201/Visuals.md">Line Graphs</a>
<br> Some of the graphs that I created to help me visualise the received results.

#### Conclusions
I arrived at many conclusions regarding the quality of data in the DB and the trends in student behaviour. Here are some of my findings:
1. Some students have a significant negative balance (up to -60 classes) and have several classes at the same time (up to 4). I assumed that there is a problrm with the data in the DBs, likely with how transaction and class statuses are recorded.
2. Students buy more classes than they take. My hypotheses include the following: not all data are recorded in the DB; students buy classes in bulk on promotions; there are not enough teachers, etc.
3. The number of payments gradually increases throughout the year, with two spikes in February and September. I can see several seasonal factors here: in Russia there are long New Year holidays, and lots of people return to normal life only in February; people are used to starting their academic year in September even after school; the school likely offered some discounts to mark the start of a new academic year.   

### Case Study 2: Unit Economics of a Streaming Service
Project for a streaming service with a pay-by-month subscription. I needed to calculate unit economics to evaluate how effectife the subsciption plan is, and suggest a scenario for achieving a 25% margin. History data was provided for 6 full months.

#### Tasks
1. Calculate product unit economics and suggest a scenario for achieving a 25% margin.
2. Create a unit economics calculator to provide the client with an automated decision-making tool.
3. Create graphs to demonstrate the audience, peak view periods, most popular films, etc.

#### Solution
I did all calculations in an Excel sheet. The unit in this case is a subscription. To calculate Retention, LT, CAC, LTR and Fixed Costs, I first needed such data as new subscribers per month, views per month, users per month, average views per user per month, etc. 

> <a href="https://docs.google.com/spreadsheets/d/1WqN5jC5k0IOt-P_XJnigEdkmnp7CBXFE1T0B7rJsS2I/edit?usp=sharing">Google Sheet</a>
<br> In this Google sheet, you can see the resulting calculator with parameters set to achieve a 25% margin. Also I added some examples of my calculations.

#### Graphs
> <a href="https://github.com/Melifarro19/Valeria-Dzhukich-Portfolio/blob/main/Case%20Study%202/Visuals.md">Graphs</a>
<br> Some of the graphs that I created to visualise the received results.

#### Conclusions
1. The number of new users sharply grew in April, but was constantly falling after that. August numbers are almost the same as in March, at the start of the period. The %CAC amounted to almost 138%. This shows that marketing efforts to attract new users didn't pay off.
2. The number of views was increasing slowly and eventually dropped, but average views per month kept growing. This might mean that users were getting more used to the platform; the content was matching their expectations more and more; marketing started targeting the right audience for the content provided; etc.
3. User retention was constantly dropping, with average retention around 80%. This might mean that the content wasn't updated often enough to keep old users interested.
4. Margin was -94% which is predictable in the first months of the operation. A lot of changes are needed to achieve the desired 25% margin, most importantly improving CAC and retention. 

### Case Study 3: Statistical Analysis of Delivery Service Metrics
Project for a delivery service. The main task was to find in which situations there was a shortage of delivery persons. The management was planning to provide additional incentives to eliminate such shortages.   

#### Tasks
1. Analise order to assignment conversion and average delivery person assignment time during peak hours vs off-peak hours. Find out if there is any statistically significant difference.
2. Analise conversion and average assignment time by districts. Find out if there is any statistically significant difference.
3. Analise conversion depending on the distance. Take into account that assignment algorithms differ for distances up to and over 5 km. Find out if there is any statistically significant difference.

#### Solution
I performed the analysis in Excel, with the Analysis ToolPak. First, I determined whether I should use parametric or nonparametric statistical tests: checked if the samples were normally distributed; checked if the samples contained any outliers (using the nterquartile range). The analysis showed that I could use parametric tests. After that I compared the sample variances using the F-test. Then I compared the samples and tested my null hypotheses with the two-sample t-test (assuming unequal/equal variances depending on the F-test results) and Anova analysis with post hoc tests.

> <a href="https://github.com/Melifarro19/Valeria-Dzhukich-Portfolio/blob/main/Case%20Study%203/Visuals.md">Statistical Tests</a>
<br> These are examples of statistical tests in Excel.

#### Conclusions
1. Order to assignment conversion is less in peak hours, which means there are not enough delivery persons during such hours.
2. Average assignment time is bigger in peak hours, which further asserts that there is a shortage of delivery persons in such hours.
3. Average assignment time is the same in all three districts, but conversion is less in district 3.
4. Conversion for orders with distance up to 5 km is more than for orders over 5 km.

## CONTACTS
- Email: valeria.chizh@gmail.com

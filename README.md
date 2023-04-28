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

> <a href="https://github.com/Melifarro19/New-Analytical-Life/blob/main/Case%20Study%201/SQL%20Query">SQL Query</a>
<br> Here is a part of the final SQL query for reference.

#### Graphs
> <a href="https://github.com/Melifarro19/New-Analytical-Life/blob/main/Case%20Study%201/Visuals.md">Line Graphs</a>
<br> Some of the graphs that I created to help me visualise the received results.

#### Conclusions
I arrived at many conclusions regarding the quality of data in the DB and the trends in student behaviour. Here are some of my findings:
1. Some students have a significant negative balance (up to -60 classes) and have several classes at the same time (up to 4). I assumed that there is a problrm with the data in the DBs, likely with how transaction and class statuses are recorded.
2. Students buy more classes than they take. My hypotheses include the following: not all data are recorded in the DB; students buy classes in bulk on promotions; there are not enough teachers, etc.
3. The number of payments gradually increases throughout the year, with two spikes in February and September. I can see several seasonal factors here: in Russia there are long New Year holidays, and lots of people return to normal life only in February; people are used to starting their academic year in September even after school; the school likely offered some discounts to mark the start of a new academic year.   

## CONTACTS
- Email: valeria.chizh@gmail.com

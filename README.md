# What's your next job?

A web app that helps individuals, more specifically, data scientists to make job transitions. 

## Problem statement

Planning to transit into a new job can be stressful. It's often hard to figure out what next moves might be good for you. One way to help with such planning is to better understand skills that are important for job transitions given your current work experience. 
 
## Solution

The web app provides personalized information about possible job transitions and relevant skills. Users of the web app are prompted to enter a brief description of their current data science job. The web app identifies individuals in the database who have had similar jobs as the user's current job. It then returns proportions of these individuals who later transition into jobs that require more of different skills (e.g., machine learning, data warehouse/governance, and management/leadership). The web app also gives examples of possible next jobs and related key skills.

## Files
### resume_scraping
Script to scrape resumes (work experience and education) from indeed.ca.
### data_preprocessing
Sript to clean and wrangle scraped data.
### topic_modeling
Script to process text and conduct nmf topic modeling.
### next_job_pipeline
Script to compare user's job description with job descriptions in dataset, identify possible next jobs, and compute changes in topic weights at job transitions.

 
 


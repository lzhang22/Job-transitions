# What's your next job?

A web app that helps individuals, more specifically, data scientists to make job transitions. 

## Problem statement

Planning to transit into a new job can be stressful. It's often hard to figure out what next moves might be good for you. One way to help with such planning is to better understand skills that are important for job transitions given your current work experience. 
 
## Solution

The web app provides personalized information about possible job transitions and relevant skills. Users of the web app are prompted to enter a brief description of their current data science job. The web app returns suggestions of future jobs, skills involved in those jobs (e.g., machine learning, statistical analysis), and keywords associated with the jobs.

## Files
### resume_scraping
Scrapes data science/engineering related resumes (work experience and education) from indeed.ca.
### data_preprocessing
Cleans and wrangles scraped data.
### topic_modeling
Pocesses text (job descriptions) and runs nmf topic modeling (trains a word2vec model to represent words in the dataset as vectors; semantic similarity between words is then used to compute coherence score for topic model seletion).
### transition_matrix
Computes probability of transitionsing from each topic at a job to each topic at the subsequent job. 
### next_job_pipeline
Processes user's input (current job description) and extracts its topics. Gets predicted future job by multiplying user's topic matrix with transition matrix. Then uses cosine similarity to find jobs in dataset that are most similar to the predicted future job and present information about those jobs.

 
 


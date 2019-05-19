## What's your next job?

### Porject introduction and motivation
A web app I developed as my Insight project. The motivation of the project is that job transitions is often stressful; it can be hard to figure out what next job might be good for you. I made a web app that provides users with personalized information about potential future jobs and skills important for such jobs. 

### Methodology
To examine job transitions that have actually occurred, I used resumes

## Files
### resume_scraping
Scrapes resumes (work experience and education) from indeed.ca. For my project, I focused on data science/analytics/enginerring related jobs.
### data_preprocessing
Cleans and wrangles scraped data.
### topic_modeling
Pocesses text (job descriptions) and runs nmf topic modeling.  (a word2vec model is trained to represent words in the dataset as vectors; semantic similarity between words is then used to compute coherence score for topic model seletion).
### transition_matrix
Computes probability of transitionsing from each topic at a job to each topic at the subsequent job. 
### next_job_pipeline
Processes user's input (current job description) and extracts its topics. Gets predicted future job by multiplying user's topic matrix with transition matrix. Then uses cosine similarity to find jobs in dataset that are most similar to the predicted future job and present information about those jobs.

 
 


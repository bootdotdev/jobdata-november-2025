# jobdata-november-2025

The data in [jobdataapi.txt](/jobdataapi.txt) was copy-pasted directly from the [JobData API](https://jobdataapi.com/titles/) on November 1, 2025. It contains job titles and the number of times they were found in job postings over the previous 30 days in the API's database.

According to the API, there are:

- 2,134 unique roles
- The data is for the past 30 days
- Roles only show up if there were at least 50 posts for that role in the past 30 days

The [classified.csv](/classified.csv) file is a cleaned version of the data. It removes irrelevant roles, and adds a "classification" column that categorizes each role into one of the following categories:

- Fullstack Developer
- Backend Developer
- Frontend Developer
- Data Analyst
- DevOps Engineer
- Data Engineer
- AI Engineer

Why these 7? Well, because that's what we're interested in teaching at [Boot.dev](https://www.boot.dev).

## Classification Method

Classification was done by hand using a couple of scripts and an LLM for sanity checking. Here were some of the rules I followed:

- Removed managerial roles
- Removed finance-specific roles
- Removed hardware/embedded roles
- Removed super generic roles like "Engineering Manager"
- Removed testing/qa roles
- Removed customer support/qa roles
- Removed product/project management roles
- If a programming langauge was in the title, did my best to infer the role type

Anyhow, if you disagree with my classification I've included the original data so feel free to run your own!

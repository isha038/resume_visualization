
# Job Application Analysis and Visualization

### Author: Isha Shrestha  


## Project Overview

This project analyzes a dataset of job applications, applicants, and job titles to gain insights into job trends and applicant characteristics. The primary objective is to visualize and explore data trends across job applications, identify which job titles received multiple applications, and investigate other key factors such as applicant experience, geographic distribution, and citizenship status.

## Features
- **Data Cleaning**: The project cleans and prepares the dataset, removing duplicates and ensuring data consistency.
- **Data Visualization**: Various visualizations are generated using `matplotlib` and `folium`, providing a detailed overview of applicant experience, job popularity, geographic concentration, and citizenship demographics.
- **Entity-Relationship Diagram (ERD)**: The project includes an ERD showing relationships between applicants, job titles, and applications.


The system is modeled as three main entities:
- **Applicants**: Represents the personal details and qualifications of the applicants.
- **Job Titles**: Represents the job positions available.
- **Job Applications**: Represents the application events, connecting applicants to job titles.


## Visualizations
The following visualizations are created for insightful analysis:
1. **Distribution of Years of Experience Among Applicants**: A histogram displaying the distribution of applicants' work experience.
2. **Distribution of Number of Applications per Job Title**: A bar chart showing how many applications each job received.
3. **Top 10 Job Titles with the Most Applications**: Highlights the most popular jobs among applicants.
4. **Average Years of Experience vs Number of Applications**: A scatter plot that investigates if there is a correlation between applicant experience and job popularity.
5. **Geographic Distribution of Applicants (Heatmap)**: A heatmap visualizing where applicants are located geographically.
6. **Marker Cluster Map of Applicants**: A marker cluster map showing geographic concentration of applicants.
7. **Applications by Job Category**: A bar plot categorizing the applications by job type.
8. **Citizenship Status of Applicants**: A pie chart showing the proportion of U.S. citizens vs. non-U.S. citizens.

## Data Dictionaries
The dataset is divided into three key components:

1. **Applicants**:
    | Field Name        | Data Type  | Description                                                                 |
    |-------------------|------------|-----------------------------------------------------------------------------|
    | id                | int64      | A unique identifier for each application (application ID).                   |
    | first_name        | object     | The first name of the applicant.                                             |
    | last_name         | object     | The last name of the applicant.                                              |
    | email             | object     | The email address of the applicant.                                          |
    | years_experience  | int64      | The total number of years of professional work experience of the applicant.  |
    | latitude          | float64    | The latitude of the applicant's location.                                    |
    | longitude         | float64    | The longitude of the applicant's location.                                   |
    | python_years      | float64    | The number of years the applicant has experience with Python.                |
    | pandas_years      | float64    | The number of years the applicant has experience with the Pandas library.    |
    | us_citizen        | bool       | A boolean value indicating if the applicant is a U.S. citizen (True/False).  |
    | job_applied_for   | object     | The title of the job the applicant applied for.                              |
    | highest_ed        | int64      | The highest level of education attained by the applicant (numerical scale).  |
    | date_applied      | object     | The date when the application was submitted (in string format).              |

2. **Job Titles**:
    | Field Name        | Data Type  | Description                                                                 |
    |-------------------|------------|-----------------------------------------------------------------------------|
    | job_applied_for   | object     | The title of the job the applicant applied for.                              |
    | job_id            | object     | A unique identifier for the job that the applicant applied for (job ID).     |

3. **Applications**:
    | Field Name        | Data Type  | Description                                                                 |
    |-------------------|------------|-----------------------------------------------------------------------------|
    | id                | int64      | A unique identifier for each application (application ID).                   |
    | job_id            | object     | A unique identifier for the job that the applicant applied for (job ID).     |

## How to Run the Project
### Requirements:
- Python 3.x
- Libraries:
  - `pandas`
  - `matplotlib`
  - `folium`

### Instructions:
1. **Install the dependencies**:
    ```bash
    pip install pandas matplotlib folium
    ```

2. **Load the dataset**: 
   Ensure your dataset files are in the correct format (CSV or JSON).

3. **Run the analysis**: 
   Execute the Python notebook to clean, process, and analyze the dataset.

4. **Visualizations**: 
   The visualizations will be generated as graphs and maps (saved as HTML or displayed inline).



## Conclusion
This project provides detailed insights into the job application dataset through various visualizations. It helps stakeholders understand trends related to applicant experience, job popularity, geographic distribution, and citizenship status, and enables better decision-making in terms of job recruitment strategies.

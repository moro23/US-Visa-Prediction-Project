# US-Visa-Prediction-Project

A machine learning project to predict US visa certification status, incorporating MLOps practices for experiment tracking and model demonstration.

## Project Overview 
This project analyzes historical data of visa applications to build a classification model that can predict whether a visa will be 'Certified' or 'Denied'. The goal is to assist the Office of Foreign Labor Certification (OFLC) by automating the initial screening process, thereby increasing efficiency. The project utilizes MLflow for experiment tracking and Gradio for creating an interactive demo of the final model.

## Tech Stack 

- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib
- **MLOps Tools:** MLflow, Gradio
- **Environment:** Jupyter Notebook, Git

## Context:

Business communities in the United States are facing high demand for human resources, but one of the constant challenges is identifying and attracting the right talent, which is perhaps the most important element in remaining competitive. Companies in the United States look for hard-working, talented, and qualified individuals both locally as well as abroad.

The Immigration and Nationality Act (INA) of the US permits foreign workers to come to the United States to work on either a temporary or permanent basis. The act also protects US workers against adverse impacts on their wages or working conditions by ensuring US employers' compliance with statutory requirements when they hire foreign workers to fill workforce shortages. The immigration programs are administered by the Office of Foreign Labor Certification (OFLC).

OFLC processes job certification applications for employers seeking to bring foreign workers into the United States and grants certifications in those cases where employers can demonstrate that there are not sufficient US workers available to perform the work at wages that meet or exceed the wage paid for the occupation in the area of intended employment.

## Objective:

In FY 2016, the OFLC processed 775,979 employer applications for 1,699,957 positions for temporary and permanent labor certifications. This was a nine percent increase in the overall number of processed applications from the previous year. The process of reviewing every case is becoming a tedious task as the number of applicants is increasing every year.

The increasing number of applicants every year calls for a Machine Learning based solution that can help in shortlisting the candidates having higher chances of VISA approval. OFLC has hired your firm EasyVisa for data-driven solutions. You as a data scientist have to analyze the data provided and, with the help of a classification model:

* Facilitate the process of visa approvals.
* Recommend a suitable profile for the applicants for whom the visa should be certified or denied based on the drivers that significantly influence the case status. 


## Data Description

The data contains the different attributes of the employee and the employer. The detailed data dictionary is given below.

* case_id: ID of each visa application
* continent: Information of continent the employee
* education_of_employee: Information of education of the employee
* has_job_experience: Does the employee has any job experience? Y= Yes; N = No
* requires_job_training: Does the employee require any job training? Y = Yes; N = No 
* no_of_employees: Number of employees in the employer's company
* yr_of_estab: Year in which the employer's company was established
* region_of_employment: Information of foreign worker's intended region of employment in the US.
* prevailing_wage:  Average wage paid to similarly employed workers in a specific occupation in the area of intended employment. The purpose of the prevailing wage is to ensure that the foreign worker is not underpaid compared to other workers offering the same or similar service in the same area of employment. 
* unit_of_wage: Unit of prevailing wage. Values include Hourly, Weekly, Monthly, and Yearly.
* full_time_position: Is the position of work full-time? Y = Full Time Position; N = Part Time Position
* case_status:  Flag indicating if the Visa was certified or denied
This project is done as a part of [Project of the Week at DataTalks.Club](https://github.com/DataTalksClub/project-of-the-week/blob/main/2022-08-14-frontend.md)

Dataset: https://www.kaggle.com/datasets/moro23/easyvisa-dataset

## ⚙️ Environment Configuration

This project uses a virtual environment to manage dependencies.

1.  **Create a Virtual Environment:**
    ```bash
    python3 -m venv venv
    ```

2.  **Activate the Virtual Environment:**
    - On macOS/Linux:
      ```bash
      source venv/bin/activate
      ```
    - On Windows:
      ```bash
      .\venv\Scripts\activate
      ```

3.  **Install Required Packages:**
    You can install the packages using pip and the `requirements.txt` file. Make sure you have `pip` available in your environment.
    ```bash
    pip install -r requirements.txt
    ```
    *Note: If you don't have a `requirements.txt` file, you can create one with `pip freeze > requirements.txt` after installing the packages below manually.*
    ```bash
    pip install jupyter notebook pandas pyarrow numpy matplotlib seaborn scikit-learn xgboost gradio
    ```

---

## How to Run the Project

Follow these steps to set up the environment and run the project.

### Step 1: Clone the Repository
```bash
git clone <your-repository-url>
cd US-Visa-Prediction-Project
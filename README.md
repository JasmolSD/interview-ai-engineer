# AI Engineer Interview

## Goal

## Rules
The assignment should take around 4 hours to complete, but you do not need to time yourself. Focus on delivering maintainable code that is easy to understand and easy to change. The assignment is intentionally open-ended; part of what we are evaluating is how you prioritize and decide what to build. You may use any open-source tools or LLM assistance, provided the end result runs locally on macOS with Docker Desktop installed. Be sure to use the provided python uv project named 'fda-regulations'.  Utilize python 3.13 and type hints as much as possible. Include clear instructions for everything you provide and be prepared to walk through your decisions.

## Data

For this assignment, you should user one of the following two publicly available data sources from the FDA:

- FDA Data Dashboard API [https://datadashboard.fda.gov/oii/api/index.htm]
- - This API contains several endpoints with data pertaining to inspections and compliance actions for different establishments under the supervision of the FDA. The data in this database is structured and easily accessible via the API they define.

- FDA Warning Letters table [https://www.fda.gov/inspections-compliance-enforcement-and-criminal-investigations/compliance-actions-and-activities/warning-letters]
- - This site contains of warning letters sent to establishments under supervision of the FDA. These letters are not structured and are not easily accessible, however the data contained within them is significantly more valuable as it contains unstructured written narratives of specific violations and details surrounding the issues the necessitated the warning letters to be sent out.

In order to access the data within the API, you will need to create an account in the FDA OII Unified Logon system [https://www.accessdata.fda.gov/scripts/oul/index.cfm?action=portal.login]

The FDA Warning Letters data should be accessible without an OII account.

Once an account is created, it typically takes about 10 to 20 minutes for their system to send out the credentials needed to access the data dashboard API. If for some reason you are unable to access the resources from these data sources, such as changes to the FDA site or events such as a government shutdown that may impact service availability, please reach out to Gavin Karr at gavin@modicusprime.com and we can provide you with access to a cached version of these datasets.

## Deliverables

In order to submit your assignment, please fork this repository and open a PR with your changes.
As mentioned, the assignment is deliberately open-ended. However, in order to provide some structure to the project and in order to ensure some consistency in end result, we would like you to take into account three rough phases:

1. Data Acquisition and Engineering
    - Please submit a brief report containing summary statistics regarding the dataset that you have created from the previously mentioned raw data sources. Please list inclusion criteria, exclusion criteria, and brief reasoning for why you selected the data that you did

2. Data Modeling
    - The end result should contain some novel processing of the collected data. Whether that is via interactive components, preprocessed analysis, or static visuals, this is up to you. Keep in mind the qualifications and desired skills of the AI Engineer role when choosing how you want to demonstrate your talent via this assignment.

    - A note on processing requirements: We recognize that some of the data available could consumer large amounts of computing resources when addressed in their entirety. For this project, consider it a polished proof of concept. We do not expect, or want you to, enterprise grade computing resources such as GPU clusters or pay-per-token APIs. When doing a test run of this assignment on our local hardware (in this case an M3 Pro Macbook with 36 GB of unified memory), we were able to build a prototype that was functional albeit with slow response times per query.

3. Project Presentation
    - We acknowledge that with short suggested time frame of the project, as well as the broad potential scope of assignment, that not all 

## What We Are Evaluating

- Does the service build and run on macOS with Docker Desktop?
- Is your documentation complete and concise, without obvious LLM-generated filler?
- Could a senior-level software engineer understand the basics of your code based upon its documentation?
- Did you use uv and type hints effectively? For example, did you try to not use untyped `dict`, `str`, `Any` or `Unknown`


## Questions

If anything is ambiguous, make a decision, document your reasoning, and move on. 
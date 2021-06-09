# JobPathways-ON-FoodRetail
Code for the skill adjacency model used in BII+E's Job Pathways in Food Retail Project

Welcome to the Job Pathways in Food Retail - Ontario open code git! If you haven't already, we strongly recommend you read the report (as well as the additional playbook materials) before diving in here.

Here we provide the code to create the adjacency model used for the project. This code was created by Viet Vu for BII+E's first Job Pathways: From Theory to Practice project, and modified for this application which looked at the available occupational adjacencies for Cashiers and Store shelf stockers, clerks and order fillers.

The adjacency model is the first step in identifying potential occupational pathways, once the origin occupations are selected. It is designed to take available data on the requirements of a worker in a particular occupation, and measure how close they are to those of another occupation. It is a tool that can be applied to any origin occupation with available skill data, and aims to identify the occupations that are most closely related to it, based on the variables that are chosen.
We use publicly available data from the Occupational Information Network (ONET), an American database of standardized and occupation-specific descriptors. For *Job Pathways in Food Retail*, the following ONET attributes were included: abilities, skills, knowledge, work activities, and work context. 

Using our existing crosswalk https://github.com/BrookfieldIIE/NOC_ONet_Crosswalk, we then linked this data to Canadian occupations. 

This code does not provide the ONET data, or the R code and data for the geographic and other data filters due in part to size, and in part to the ongoing updating of the the data we used, which is freely available and referenced in our reports. If you have questions about how that was done or how we accessed the data, please see our reports and if you have further questions, contact us at brookfield.institute@ryerson.ca. We are happy to explore ways to support your team on a cost-recovery basis.

Food Retail Trends Report: https://brookfieldinstitute.ca/disruption-and-opportunity-in-ontarios-grocery-sector/

Pathways Report: https://brookfieldinstitute.ca/mapping-job-transitions-for-ontario-food-retail-workers/

Playbook and Resources: [Forthcoming]

Below is a description of each document and its contents
-
adjacency function definition: Defines the cosine similarity function for the occupational attributes selected. 

preparing ONET data: Relabels, normalizes, and prepares ONET data from its automatic excel download format for use with the adjacency function. 

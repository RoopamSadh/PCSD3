*******************************************
DATASET: NCR survey dataset (3-Dimentional)
*******************************************

Description:

Data is collected through an extensive online survey to explore the significance of quality parameters of Higher Educational Institutions (HEIs).  Data is collected from the National Capital Region (NCR) of India as it has representative Higher Educational Institutions. Survey invited the responses from Sciences, Social-Sciences, Medical, Technology, and Humanities domains of twelve premier HEIs. Seven respondent categories Undergraduate, Graduate Study, Graduate Research, Faculty, Parents, Administrator, and Professional were identified in survey.  
************************************************************

The Dataset: Survey_Data.xlsx
	
 * Number of Variables: 11
 * Likert Scale used: 1- 4
 * Worksheet WO_Admin contains total survey responses (2533).
 * Worksheet Cluster contains the results of PCSD3 clustering over the dataset.	
*****************************

List of Variables with their used abbreviations:

Teaching(Teach), Graduate Outcomes(GO), Academic Flexibility(Flexi),Transparency & Accountability(Trans_Acc), Infrastructure & Resources(Infra_Res), Research(Research), Student Support Services(SSS), International Outlook(IO), Fee Structure & Financial Assistance(Fee_Ass), Academic Autonomy(Auto), Inclusivity(Inclus).
************************************************
List of respondent groups and their used abbreviations:

Administrator(Admin), Faculty(Faculty), Parents(Parent), Graduate Study(PG), Professional(Professional), Graduate Research(Rsearcher), Undergraduate(UG).
*******************************************************

****************************************************************************
PCSD3: "Pattern Clustering for Survey Data based on Directional Differences"
****************************************************************************
Description:

PCSD3 clustering algorithm is specifically designed to cluster survey data that contains ordinal response variables (or Likert type response scale) along with a nominal variable specifying the categories of respondents. PCSD3 clusters the data based on the marking patterns. The method does not require parameters  to be specified by the users. The users are required to provide data in specified format (see dataset and its description). PCSD3 recognize the respondent categories and identify their distinguised features and clusters data accordingly. Therefore the number of PCSD3 clusters are always equal to the number of designated categories of the respondents. PCSD3 utilize newly developed "Frequency based Probabilistic Scoring" and a dedicated "Decision Making procedure" for clustering.
************

Directions:

 * Number of total scripts: 10
 * All the scripts and data file (Survey_Data.xlsx) should be in one folder.
 * Load (Run) all scripts (functions) before running the main function (Main.R).
 * Set path of Survey_Data.xlsx in main function (Line 7th and 23rd of the Main.R).
 * Run Main.R for execution of PCSD3 clustering.
***********

Functions:

 * Main.R: main() function calling the required procedures for performing PCSD3 clustering. 
 * Pattern.R: create direction vector corresponding to each survey response in data.
 * Pat_div.R: divide the set of direction vectors on the basis of respondent category.
 * Ref_creat.R: create reference vectors (each corresponding to a respondent group).
 * Stat_pat1.R: calculates the frequencies of direction values in the set of direction vectors.
 * Stat_pat2.R: creates secondary data array (SDA) by using the frequencies.
 * Stat_pat3.R: crates an intermediate data matrix.
 * Stat_pat4.R: Creates Primary data array (PDA) by using the frequencies and constraint alpha.
 * Ref_creat1.R: is decision making procedure (use PDA and SDA for finding reference vector).
 * Matc.R: is matching procedure that gives the final index to each survey response (Cluster).
 ********** 

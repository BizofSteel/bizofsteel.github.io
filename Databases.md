#### Contents:
|[ePortfolio Homepage](https://bizofsteel.github.io)<br>|[Code Review](https://bizofsteel.github.io/Code_Review.html)<br>|[Software Design and Engineering](https://bizofsteel.github.io/Software_Design_and_Engineering.html)<br> |[Algorithms and Data Structures](https://bizofsteel.github.io/Algorithms_and_Data_Structure.html)<br>|[Databases](https://bizofsteel.github.io/Databases.html)|
|:-------------|:------------------|:------|:------|:------|


# Databases


## _The Artifact_
For this capstone course we have been asked to select artifacts from previous experience for the purpose of expanding them in complexity to showcase our proficiency in the categories of Software Engineering and Design, Algorithms and Data Structures, and Databases.  In this section I will be presenting my proficiency in Databases by enhancing the functionality of my CS 340: Advanced Programming Concepts Final Project.
For my CS340 Advanced Programming Concepts Final we were asked to create a financial reporting service for basic stock market securities information.   This reporting service is intended for use by authorized personnel for creating interactive web reports and dashboards.  For ease of accessibility, the service was automated to use MongoDB, a NoSQL document-storage system which is supported by many languages, including Java and Python via driver APIs.  The artifacts themselves are python files that facilitate the services of Creating, Reading, Updating, and Deleting documents from a Mongo Data Base.   

## _Inclusion of the Artifact in ePortfolio_
I have chosen to include this artifact in my ePortfolio because as a final project we were asked to create pipelines in MongoDB for advanced querying.  “An aggregation pipeline is a framework for data aggregation modeled on the concept of data processing pipelines. Documents enter a multi-stage pipeline that transforms the documents into aggregated results.” (W.S., 2020) Working with aggregation pipelines requires an in depth understanding of databases. Specifically advanced querying to get specific results for dashboard creation, performance analysis, and business analysis to name a few.  For our final project in CS-340 we were asked to create basic aggregations that would display our understanding of how these pipelines work.  To enhance this artifact and showcase my proficiency in Databases, I plan to automate specific pipeline aggregations into my already enhanced artifact that I used for the  “Algorithms and Data Structures” proficiency, and allow the user to access multiple areas of the data per user their options.  By successfully doing so, I hope to demonstrate my expertise in Databases.

## _Process of Enhancing Artifact_ 
One of the issues with the Python Services that I created originally was that there was one python file for every service.  One must call the respective service, python file every time to get that service; this was no different for the basic aggregations that I created for the course.  During my enhancement for the proficiency in Data Structures and Algorithms, I consolidated all CRUD functionality into one intuitive solution that performs the desired functionality while helping the user along with their activities.   At the same time, I created place holders for the Pipeline Aggregations that I would create for this section.  It is highlighted in red in the following pseudocode:


CLASS Create
METHOD Create MongoDB
RETURN
CLASS Read
METHOD Read MongoDB
RETURN
CLASS Update
METHOD Update MongoDB
RETURN
CLASS Delete
METHOD Delete MongoDB
RETURN
CLASS Main
WHILE Condition
OBTAIN Service Desired
IF Service CREATE
CALL CLASS Create
ELSEIF Service READ
CALL CLASS Read
ELSEIF Service UPDATE
CALL CLASS Update
ELSEIF Service DELETE
CALL CLASS Delete
ELSEIF Service PIPELINE
OBTAIN PIPELINE TYPE
IF PIPELINE 1
AGGREGATE PIPELINE 1
ELSEIF PIPELINE 2
AGGREGATE PIPELINE 2
ELSEIF PIPELINE 3
AGGREGATE PIPELINE 3
ELSEIF PIPELINE 4
AGGREGATE PIPELINE 4
ELSE Repeat Service
	END WHILE


When calling the artifact to start the service, you will be prompted you for the services available.   Selecting Option 5 initiates the aggregation pipeline service module.   In this section you will have 4 options for aggregation pipelines.  (Figure 1) 









In Figure 2, I have selected the Volume of Shares to be displayed by Country for a specific Sector.    When this option is chosen, a pipeline is run to return the Sectors available within the Database.  It is important to display the available “Sectors” as a query and not hardcode them should a new Sector be created in the Database.

For this example, I have selected the “Services” sector and a pipeline returns Volumes of Shares by country in descending order.   For more examples of this query option, please refer to Appendix A.
Next, I have designed a pipeline that aggregates Total Outstanding Shares by Industry for a Specified country with the additional option to sort in an ascending or descending manner.  In Figure 3 I have chosen Option 2 to begin this aggregation.  Like the first Option, an aggregation for all available countries is run to show the user their options.   In this case, I have chosen “Japan” as the country of choice.  Next, we are prompted to choose a sorting option and the pipeline is created for Total Outstanding Shares by Industry for Japan.  For more examples of this query option, please refer to Appendix B.

The third pipeline aggregates the “Return on Investment per Industry within a Sector for a Country”.   This pipeline is complicated but the way that it is presented to the user makes it very easy to get the results desired.   First, a pipeline for available countries is run to showcase options.  In figure 4, I have chosen “China”.  Next, a pipeline is run to show the available Sectors within that country and the user is prompted to choose a sector from the option list.  

Once the Sector is inputted, the Final Pipeline is aggregated with the Return on Investment results per Industry within the chosen Sectors in the chosen Country.  For more examples of this query option, please refer to Appendix C.
The final pipeline Aggregates the mean “Sales Growth for the Last 5 years” per a user defined option and Limit.  As seen in Figure 5, when the Aggregation is chosen the user is prompted to select in which area the Growth should be reported in.   

Once a choice is made, in the case “Country”, the user is asked to select the total number of documents to be returned.   To keeping this example small, we asked for 10.   The pipeline is then returned successfully.  For more examples of this query option, please refer to Appendix D.

## _Course Objectives - Enhancement_ 
By enhancing this artifact to include automated pipelines, I have facilitated enhanced Database queries that not only make the User feel at ease to run them, but also allows for simple scaling.   For example, running a pipeline within a pipeline to display available options makes the maintenance of those aggregations almost not necessary which makes scalability simple. Furthermore, adding options to all of the available aggregations is straight forward.   By automating enhanced data queries and taking into account not only scalability but also ease of use, I have showcased in proficiency in Database expertise.  


**Bismark J. Aldana ePorfolio Links**<br>
* [ePortfolio Homepage](https://bizofsteel.github.io)<br>
* [Refinement Plan & Code Review](https://bizofsteel.github.io/Code_Review.html)<br>
* [Software Design and Engineering - Enhancement One](https://bizofsteel.github.io/Software_Design_and_Engineering.html)<br>
* [Algorithms and Data Structures - Enhancement Two](https://bizofsteel.github.io/Algorithms_and_Data_Structure.html)<br>
* [Databases - Enhancement Three](https://bizofsteel.github.io/Databases.html)


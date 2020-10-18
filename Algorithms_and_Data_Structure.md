#### _Move Around:_
| [ePortfolio Homepage](https://bizofsteel.github.io)<br>
| [Code Review](https://bizofsteel.github.io/Code_Review.html)<br>
| [Software Design and Engineering](https://bizofsteel.github.io/Software_Design_and_Engineering.html)<br> 
| [Algorithms and Data Structures](https://bizofsteel.github.io/Algorithms_and_Data_Structure.html)<br>
| [Databases](https://bizofsteel.github.io/Databases.html)<br>
| [Weight Tracker Android App](https://bizofsteel.github.io/DroidWeightApp.html)<br>

# Algorithms and Data Structures

## _The Artifact_
For our _CS499 Computer Science Capstone_ course we were asked to select artifacts from previous experience for the purpose of expanding them in complexity to showcase our proficiency in the categories of Software Engineering and Design, Algorithms and Data structures, and Databases. In this section I will be presenting my proficiency in Algorithms and Data Structures by enhancing the functionality of my CS 340: Advanced Programming Concepts Final Project.  For my CS340 Advanced Programming Concepts Final we were asked to create a financial reporting service for basic stock market securities information.  The reporting service is intended for use by authorized personnel for creating interactive web reports and dashboards.  For ease of accessibility, the service was automated to use MongoDB, a NoSQL document-storage system which is supported by many languages, including Java and Python via driver APIs.  The artifacts themselves are python files that facilitate the services of Creating, Reading, Updating, and Deleting documents from a Mongo Data Base.   

## _Inclusion of the Artifact in your ePortfolio_
I have chosen to include this artifact in my ePortfolio because while the Python artifacts performing MongoDB CRUD services by themselves are not complicated, their existence and my ability to deploy them showcase my proficiency in Data Structures and Algorithms alone. Working with databases requires a unique understanding of data structures which include lists, trees, and hash tables, among others.  To effectively run these services, one must understand how data structures work.  To enhance these artifacts, I have consolidated into one to provide a more user-friendly solution to the customer.   Consolidating them, and thus enhancing the python automation to be more efficient to the user, further shows my proficiency in creating Algorithms and Data Structures that successfully define a sequence of operations for usability and functionality that increase the customer experience.  


## _Process of Enhancing Artifact_

The Create, Read, Update, and Delete (or CRUD) artifacts were created individually as python files to perform their respective services.  
Their Basic structure can be seen in Figure 1, and a sumplified pseudocode is as follows:

```Markdown
CLASS Service
METHOD Service MongoDB
RETURN
CLASS Main
	OBTAIN Information
	CALL Service
```
   ![Figure 1](https://bizofsteel.github.io/images/Artifact%202%20-%20Fig%201.png) 


One of the issues with the Python Services is that for every function, one must run the respective python file.  Calling the python files for every service is very inefficient so to enhance this automation through python, we must plan an algorithm and data structure that not only allows for multiple selections of CRUD functionality to be available but to also be presented as an intuitive solution that performs the desired functionality while helping the user along with their activities.  Therefore, to enhance the artifact, the following structure was followed:

```Markdown
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
					CALL PIPELINE Placeholder 1
				ELSEIF PIPELINE 2
					CALL PIPELINE Placeholder 2
				ELSEIF PIPELINE 3
					CALL PIPELINE Placeholder 3
				ELSE Repeat Service
	END WHILE


	
```
When calling the artifact to start the service, the python file will now display and prompt the user with the services available.  You may now select from Six (6) options.  Options 1 – 4 are for the CRUD services respectivley, 5 is for the aggregation pipeline that is a placeholder for the enhancements that occured during the “Database” section of my CS-499 Final Project, and 6 to exit the program (Figure 2).

   ![Figure 2](https://bizofsteel.github.io/images/Artifact%202%20-%20Fig%202.png) 


In Figure 3, I have called a create and inputted a document in JSON notation.  When a service is called and performed, the service will advise if it was performed successfully, and the loop will prompt the user to enter the next service required as seen below. 

   ![Figure 3](https://bizofsteel.github.io/images/Artifact%202%20-%20Fig%203.png) 

The service file will continue to repeat these options until the user selects to exit the program or an exception occurs.   Next, when updating a document I have included functionality that not only updates the document, but also returns the updated document so that the user does not have to run a succeeding read command to make sure the update occurs.  Figure 4 shows the user being prompted to enter the document that needs to be updates, to enter the data in the document to be updated, and then displays the document with the update.

   ![Figure 4](https://bizofsteel.github.io/images/Artifact%202%20-%20Fig%204.png) 

Further, when selecting option 5 for the “Aggregation Pipeline”, the artifact will now prompt the user to choose which pipeline they would like to run.  Once the pipeline is chosen, it will run the aggregation and return to the main options prompt to continue the service (Figure 5).  The pipeline option is only a place holder right now as these pipelines will be created for the “Database” proficiency portion of this final.  

   ![Figure 5](https://bizofsteel.github.io/images/Artifact%202%20-%20Fig%205.png) 


## _Course Objectives - Enhancement_ 
During my code review it was very evident that while the services did work as intended and were true to the design requirements, they needed some enhancement.  By enhancing this artifact through a consolidating algorithm, I have facilitated Create, Read, Update, and Delete functionality to a massive data structure (or database in this case) and removing the tedious method of continually running separate python files for those services.  I have also enhanced the python automation to be more efficient to the user which further shows my proficiency in creating Algorithms and Data Structures that successfully define a sequence of operations for usability and functionality that increase the customer experience.  

## _Enhanced Artifact - Algorithms and Data Structures_

[Algorithm and Data Structures - Enhanced Artifact Two](https://bizofsteel.github.io/Artifacts/MongoCRUD-EnhancedArtifact2.html)<br>
[Artifact Two Repository](https://github.com/BizofSteel/Algorithms_and_DataStructures)<br>



**Bismark J. Aldana ePorfolio Links**<br>
* [ePortfolio Homepage](https://bizofsteel.github.io)<br>
* [Refinement Plan & Code Review](https://bizofsteel.github.io/Code_Review.html)<br>
* [Software Design and Engineering - Enhancement One](https://bizofsteel.github.io/Software_Design_and_Engineering.html)<br>
* [Algorithms and Data Structures - Enhancement Two](https://bizofsteel.github.io/Algorithms_and_Data_Structure.html)<br>
* [Databases - Enhancement Three](https://bizofsteel.github.io/Databases.html)<br>
* [Weight Tracker Android App](https://bizofsteel.github.io/DroidWeightApp.html)<br>

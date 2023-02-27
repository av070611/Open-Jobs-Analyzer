# Open-Jobs-Analyzer
Problem Statement
In this project , we are going to use Jobs related datasets to understand the Important metrics to find quality oriented Jobs for candidates from 50 different Industries such as Software, Electronics,  Automobile, Media, Entertainment, Medical , Pharmacy etc.

We are using a Dataset which Involves taking data from the Users in the form of “FORMS”, where there is a high chance of getting dirty values.
The most important Task that we are going to do is Clean the Data.

Python Libraries: –
Numpy
Pandas
Seaborn
Matplotlib
Ipywidets
Ipython
Set the Figure Size and Background: -
Select the Figure size as 16 units for x axis, and 5 units for y axis.
Also select the Fivethirtyeight Background for our Plots.
Wishing to select any other Background for your Charts then you can just type the command: “plt.style.available” and pick up any of the Styles for your Charts.

Import the Jobs Dataset using the read_csv() function from Pandas Library.
Dataset contains any Missing Values using the isnull() function.
The Isnull function along with the sum function is going to return the total number of missing values present in each of the columns.
Top 5 Rows: -
Job FamilyDescription
Job Class
Job Class Description
should focus on: -
PayGrade, Education Level, Experience, Organization Impact, Problem Solving Level, Supervision, Contact Level, and Financial Budget.

Analyze the Job Metrics and also the Impact of these Metrics on determining the quality of a Job. You have Eight metrics to analyze: -
To analyze them, you are going to use the subplots to analyze all of these metrics.
You are going to take 2 rows and 4 columns in the plot.
You can plot 8 plots for each of the metrics.
To visualize these metrics use the countplot - countplot returns the count of different values present in the columns.
Charts: -
There are Jobs for all Levels of Education, Experience, Problem Solving etc.
Few Openings are there for Candidates having more than 7 years of Experience.

going to Clean the Job Location Column and then Find the Locations with the Highest number of Job Vacancies. Look at the Job location address column, you will notice that Postings have only one Location associated. Multiple Job Locations associated. Such as: - You have to split all the Locations present in the Job Location address column using the split function in this cell. To explode the dataset you are going to create five rows for the index number 3. Index number 3 row, you will have Job posted for 5 Cities i.e., Mumbai, Bangalore, Kolkata, Chennai, Coimbatore. After Exploding, you can see the Value Counts. In each of the values you can only find one City or Job location. Have Noticed that the City Bengaluru has been written in 20 different ways. Bangalore occurred multiple times, which means we cannot work on this dataset until we clean it properly. Similarly Delhi, Mumbai, Chennai, Kolkata, all of these cities have been written in so many different ways. In this case, use the replace() function to clean up all the inconsistent values one by one for all the Big Cities present in the dataset.
First Argument of the replace function takes in those data which you want to remove from the data set.
Second argument of the replace function takes in those data which you want to use as a replacement for the dirty values present in the data set.
You have cleaned the dirty values for all of the cities. Starting from Bangalore, Hyderabad, Mumbai, NCR which is also known as National Capital Region. Chennai, Pune, Kolkata, Ahmedabad, Chandigarh, Surat, Kochi, Coimbatore, Lucknow, Jaipur, Vijayawada, Vizag, Bhubaneshwar, Patna, Trivandrum, Mangalore, Indore, Guwahati, Nagpur, Raipur, Thane, Bhopal, and at last Vadodara. Look at the value counts after cleaning these values. Go back to the previous cell, you can see only 3775 Jobs available for Bengaluru. After Cleaning, there are 9963 Jobs available for Bengaluru which is a very huge difference. Look at the value counts of the job location address column: Most of the cities have very less number of jobs available. Remove all those cities which have less than 25 number of jobs available in their location and visualize them using the Bar plot. Looking at the chart, you will see that the Cities where the highest number of Jobs are available are Banglore, NCR, Hyderabad, Mumbai, and Chennai. Pune is at number 7, Kolkata at number 8, Ahmedabad at number 9 and Chandigarh at number 10 according to this data set. 
going to Analyze the Industries with the Highest number of Job Openings. Look at the Industry Column: - There are three Industries involved for all the Jobs.
First Industry seems to be important
The second Industry and the third Industry are sub industries of the First Industry.
Split the values using the split() function in the cell. Also impute the missing values present in the Industry Column with the most common value using the mode function. Clean the Industry column by selecting only the first value from the List as the second and third values are inconsistent. You have cleaned the Industry Column, you can see different Industries providing Jobs. Plot the Top 10 Industries providing Jobs using the bar plot: -
The IT Industry stands at number one, for providing Jobs.
Whereas BPOs stand at number 2.
And Banking stands at number 3.
As you know the Top Industries providing Jobs, also plot a Bar Chart to visualize the average Minimum Experience required for each Industry. The Industries such as BPO, Exports, and Government Agencies require lesser experience whereas the Industries such as Tyres, Iron and Steel, Facility Management require more experience in comparison to Others.

going to make an Interactive function using Ipywidgets so that you can search and filter relevant jobs based on certain criteria. You are going to use the Interact function so that you can get responsive Output from the Function. You are going to take 4 factors as Input:
City
Industry
Minimum Experience and
Number of Vacancies.
You are going to make Dropdowns for City, Industry, and Minimum Experience so that you can select any of the values present in the Dropdowns and filter the output. Create a Slider for Number of Vacancies where the base value is set to 10, if you want to change the value just slide the slider and the values will be changed within no time. Only selected columns such as Name of the Company, Title of the Job, Education requirements of the Job, Pay rate provided for the job, and the number of positions available for the Job. Columns are going to help the candidates to understand the quality of the Jobs posted in the Portal and select the most suitable job from all the jobs listed in the data frame. You can see that for the default values, the output is ready. Try changing the value of the City from Bangalore to Hyderabad, Minimum Experience required for the Job as 4 and finally Change the value of Vacancies to 20. 

going to discuss the Key takeaways from this Project. Data Cleaning is one of the most important skills required to become a data scientist. Key Takeaways: -
Understood the Job Market, and Analyzed some of the most important queries.
Function for searching and filtering jobs for certain criteria.
Visualizations for Performing Top N Analysis.

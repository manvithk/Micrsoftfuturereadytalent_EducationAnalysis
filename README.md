# Covid-19_India_Statewise_visualization
## About
The dataset used contains latest Covid-19 India State-wise data till January 2,2022. This dataset has been used to analyze covid in india by using powerbi-desktop to create various visualizations needed to understand covid-19 situation in india state-wise.
## How the project was made
1. First created a resource group (Future_ready_talent_project) under which all resouces such as azure-sqldatabase, azure-sqlserver, azure-datafactory , azure-storage(blob)
   and static web app was deployed.
2. Uploaded the Latest Covid-19 India Status.csv to the blob storage in the input container.
3. wrote sql query in the sqldatabase deployed (running on sql server) to create a table with the column headers that would take the respective data from blob storage during copy    data process.
4. Using data factory transferred the data from csv file to sql table using pipeline (Blob to SQL) with help of 2 linked services (input blob, output sql). The pipeline succeeded
   in transferring data from blob to sql database.
5. After successful transfer of data from blob to sqldatabase , connected the sqldatabase to powerbi-desktop by connecting to sqlserver. Made Visualization using powerbi-desktop      that can be used to analyze the covid-19 situation in india state-wise. Published the report to powerbi-app to get the secure-emmbbeded code which was added to html file that      was made for the static website deployed.
6. Pushed all the html files,png and other files to github repository through github-desktop.
7. Deployed static web app in azure and connected it to github repository to run a website made with basic html integrated with power-bi secure embbeded report.
     
<b>***Note that the secure embedded report in the website will not be accessible in most case (will show unavailable if logged in with normal id) because to access it you will   need organization-id of our university to access it. <p>I tried to publish the publc url but permission to get that been restricted by organization admin of our university</p><b>
<p><b> In case you are unable to see the power-bi dynamic visulization report , I have attached images of the visualization that was created in the website<b></p>

## Project Link -Repository URL
https://github.com/manvithk/Microsoft_futurereadytalent_Covid-19_Statewise_visualization
## Project Demo -Deployment URL
https://black-hill-067e5ca10.azurestaticapps.net


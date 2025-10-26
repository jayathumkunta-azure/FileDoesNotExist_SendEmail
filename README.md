# FileDoesNotExist_SendEmail

# add inside Logic app
{
    "properties":{
    "DataFactoryName": {"type":"string"},
    "PipelineName": {"type":"string"},
    "Subject": { "type":"string" },
    "ErrorMessage": {"type":"string"},
    "EmailTo": { "type":"string" } 
    }, 
    "type": "object"
}

#inside ADF 

{
  "DataFactoryName" : "@{pipeline().DataFactory}",
  "PipelineName" : "@{pipeline().Pipeline}", 
  "Subject" : "An error occured",
  "ErrorMessage" : "The file is missing in blob storage. Please place file",
  "EmailTo" : "xxxxxxxxxx@gmail.com"
}

# create table
CREATE TABLE [dbo].[emp](
	[EmpID] [int] NULL,
	[Name] [varchar](100) NULL,
	[Job] [varchar](100) NULL,
	[Salary] [int] NULL,
	[DNO] [int] NULL,
	[Location] [varchar](100) NULL
)

# emp.csv
EmpID,Name,Job,Salary,DNO,Location
201,Anil,Manager,80000,1,Hyderabad
202,Sunita,Developer,65000,2,Hyderabad
203,Rajesh,Analyst,55000,3,Hyderabad
204,Priya,HR,60000,4,Hyderabad


rgEmail
logicappEmail
datafactoryemailjaya
serveremployee
storageaccountemail (files/emp.csv)
databaseEmployee (serveremployee/databaseEmployee)

<img width="931" height="262" alt="image" src="https://github.com/user-attachments/assets/00fbbfaf-9f9b-45ce-a141-e51c437e39dc" />


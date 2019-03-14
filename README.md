# Project Description

#Azure Databricks# is an Apache Spark-based big data analytics and machine learning framework optimized for the Microsoft Azure Cloud.
Databricks is integrated with Azure to provide one-click setup, streamlined workflows, and an interactive workspace that enables collaboration between data scientists, data engineers, and business analysts.

This repository consists of 6 labs that are designed to help you to understand how to use Azure Databricks for multiple use cases, including:

Analysis of structured and unsstructed data.
Analysis of streaming data.
Machine Learning

The 6 labs are implemented 6 independent Databricks Notebooks and are described below.

#### Lab-01 Data Engineering:

This tutorial is help you understand how Azure Databricks Spark can be used to prepare raw data for analytics.

#### Lab-02 SparkSQL & Performance Optimisation

This tutorial help you to understand the capabilities and features of Spark SQL

#### Lab-03 Machine Learning

This tutorial help you understand the capabilities and features of Azure Spark MLlib for machine learning (ML).The end-to-end process for building and refining a machine learning model can be quite involved.
	
#### Lab-04 Real-time Stream Analytics
		
This tutorial help you understand the process of Azure Spark Structured Streaming.you connect a data ingestion system with Azure Databricks to stream data into an Apache Spark cluster in near real-time.

#### Lab-05 Databricks Delta
	 
This tutorial is to help you understand about Databricks Delta. Databricks Delta extends Apache Spark to simplify data reliability and boost Spark's performance.
		
#### Lab-06: Data orchestration using Azure Data Factory
	
This tutorial is to help you understand how Azure Data Factory (ADF) can be used with Azure Databricks, to create and automate piplines.

# Getting Started

These instruction will get you to download the databricks lab notebooks from Bitbucket Server and import the Notebooks into Azure databricks.

## Step 1:

### Create an Azure Databricks workspace using Azure portal

In this section, you create an Azure Databricks workspace using the Azure portal.

1.In the Azure portal, select Create a resource > Data + Analytics > Azure Databricks.

![deploy](https://i.ibb.co/thPhwmM/tuxpi-com-1551766437.jpg)

2.Under Azure Databricks Service, provide the values to create a Databricks workspace.

![deploy](https://i.ibb.co/pbZpjk8/tuxpi-com-1551766814.jpg)

3.Provide the following values:

a. Workspace name  : Provide a name for your Databricks workspace

b. Subscription    :	From the drop-down, select your Azure subscription.

c. Resource group  :  Specify whether you want to create a new resource group or use an existing one. A resource group is a container that holds related resources for an Azure solution. For more information, see Azure Resource Group overview.

d. Location	      :  Specify the location of your Databricks cluster.

e. Pricing Tier	  :  Choose between Standard or Premium.

Select Pin to dashboard and then click Create.

4.The workspace creation takes a few minutes.During workspace creation, the portal displays the Submitting deployment for Azure Databricks tile on the right side. You may need to scroll right on your dashboard to see the tile. There is also a progress bar displayed near the top of the screen. You can watch either area for progress.

![deploy](https://docs.microsoft.com/en-us/azure/azure-databricks/media/quickstart-create-databricks-workspace-portal/databricks-deployment-tile.png)


5.In the Azure portal, go to the Azure Databricks workspace that you created, and then click Launch Workspace.

![deploy](https://i.ibb.co/1m9HCC4/tuxpi-com-1551939679.jpg) 

6.You are now inside your Databricks workspace.

![deploy](https://i.ibb.co/QKNK488/Web.jpg)

### Next step is to import the labs from this repo into our Databricks workspace. ###

## Step 2:

### Download the labs from the Bitbucket repository.

1.Go to Download tab and Click on Download Repository.

![deploy](https://i.ibb.co/4VVhJyM/tuxpi-com-1551770630.jpg)

2.The downloaded file is in the zip format.

3.If you extract the ZIP file, you will see the different lab notebooks. All the notebooks are of type .dbc, which stands for Databricks Archive.

4.Next step is to import these files into our Databricks workspace.

## Step 3:

### Import our labs into Databricks Workspace.

1.Click the Workspace button![GitHub Logo](https://i.ibb.co/zrpPNZc/DataPic.png) or the Home button ![GitHub Logo](https://i.ibb.co/zNtqM9g/Datapic2.png) in the sidebar. Do one of the following:

2.Next to any folder, click the right side of the text and select Import.

![GitHub Logo](https://i.ibb.co/HHTZkmP/tuxpi-com-1551941692.jpg)

3.Browse to the location of your lab DBC file, and click import.

![GitHub Logo](https://i.ibb.co/bWDTd47/tuxpi-com-1551771056.jpg)


### Now that our notebook is in the workspace, we'll create a Databricks cluster and attach it to our notebook.###

## Step 4:

### Creating a Databricks Cluster

In Databricks you can create two different types of clusters:

1.Standard : Standard clusters are the default and can be used with Python, R, Scala, and SQL. 

2.High Concurrency : High-concurrency clusters are tuned to provide the efficient resource utilization, isolation, security, and the best performance for sharing by multiple concurrently active users.

We'll be using a Standard cluster for our Labs.


1.Click the clusters icon ![GitHub Logo](https://i.ibb.co/NpVHMyf/logo1.png) in the sidebar.

2.Click the Create Cluster button at the top of the page.


![GitHub Logo](https://i.ibb.co/c8f9SrH/tuxpi-com-1551771246.jpg)


3.Click the Create button. The cluster list page shows the status of the new cluster.

a.On the Create Cluster page, specify the cluster name QS.
		
b.select 5.2 (Scala 2.11, Spark 2.4.0) in the Databricks Runtime Version   drop-down.
		
		
		
![GitHub Logo](https://i.ibb.co/qBq9KJQ/tuxpi-com-1551773423-Data-Final.jpg)	
		
c.Click Create Cluster 

## Step 6: 

### Attach your Notebook to your cluster.

1.Go to the Databricks WorkSpace

![deploy](https://i.ibb.co/DDRzWwK/Data1.jpg)

2.Go to your specific notebook in the workspace.

![deploy](https://i.ibb.co/qdS7qWg/picData.jpg)

3.Click on `detached` written on the top-left corner, and you'll see a list of active clusters.

4.Attach your notebook to a running cluster. A green icon shall appear on top, meaning our notebook is now attached to our cluster and is ready to be executed.
![deploy](https://i.ibb.co/QPr9vtF/tuxpi-com-1551771824.jpg)

### Your Databricks Environment is now setup and you can proceed with the labs.

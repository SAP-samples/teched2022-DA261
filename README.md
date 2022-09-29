# DA261 - SAP HANA Cloud Database Administration and Development

## Description

This repository contains the material for the SAP TechEd 2022 session called DA261 - SAP HANA Cloud Database Administration and Development.  

## Overview

This session introduces attendees to the operations required for end-to-end administration and development of SAP HANA Cloud database instances using the tools offered in the SAP Business Technology Platform (SAP BTP).  Attendees will learn how to accomplish administration tasks such as instance monitoring and security management, as well as development tasks such as creating native SAP HANA artifacts and analyzing their performance.  Part 1 will introduce the tools and deploy some sample tables, a calculation view, and a stored procedure.  Part 2 will demonstrate how to further administer these deployed artifacts.  

Optional content can be skipped and will have (Optional) in its title.  
>Content appearing in this format is for additional information and does not need to be followed.


## Requirements

To complete this workshop, you need access to an SAP BTP account. You can access SAP HANA Cloud from within SAP BTP and you can use a trial, free tier,  or productive version of SAP HANA Cloud.  **This workshop assumes that you already have a SAP BTP account and a SAP HANA Cloud database.**  If not, you can register for free at https://www.sap.com/cmp/td/sap-hana-cloud-trial.html.  The exercises make use of a **trial account**, but a [free tier](https://developers.sap.com/tutorials/btp-free-tier-account.html) account can also be used.  A benefit of using free tier is that the account can be upgraded to a paid service plan without having to re-create the account.

In your SAP HANA Cloud account, perform the following steps:

1.  Open the [welcome page](https://account.hanatrial.ondemand.com/trial/#/home/trial) and go to your trial account.
    ![](images/go-to-trial.png)
2.	Enter the subaccount and then select the dev space.
3.	Click SAP HANA Cloud from the left navigation bar.
4.	Click the button Create Instance in the top right and select SAP HANA 
Database to invoke the Create Instance wizard.  
    > Only one instance of a HANA Cloud database can be created in trial or free tier accounts.  If you already have a SAP HANA Cloud database instance created, it can be used.
    
    ![](images/create-hana-instance.png)
5.  Choose SAP HANA Cloud, SAP HANA Database and click the button Next Step.
6.	Enter DEMO_HANA_DB for the instance name.
7.	Enter and confirm your administrator password – ***PLEASE REMEMBER IT AND/OR WRITE IT DOWN!***.
8.  For trial systems, consider changing the allowed connections option to **Allow all connections**.  The rest of the values can be left as a default.
9.	Complete the wizard.

    A new SAP HANA Cloud instance will be created, and this process may take  approx. 10 minutes.  The frequency of updates to the page can be set using the auto-refresh feature in the top right.  Once the instance has been created, its status will change to RUNNING.

    ![](images/running.png)


# Part 1: Introduction to the Tools and Initial Project Deployment

## SAP Business Technology Platform (SAP BTP)
The SAP BTP brings together data and analytics, artificial intelligence, application development, automation, and integration in one, unified environment.

### SAP Business Technology Platform Exercises

- [Exercise 1 - Overview of the SAP Business Technology Platform](exercises/sap_btp/ex1/)

## SAP HANA Cloud Central

The SAP HANA Cloud Central tool provides database administrators (DBAs) with a simple and centralized overview of their SAP HANA Cloud databases and SAP HANA Cloud data lake instances. 

### SAP HANA Cloud Central Exercises

- [Exercise 1 - Overview of SAP HANA Cloud Central](exercises/hana_cloud_central/ex1/)
- [Exercise 2 - Create Instances](exercises/hana_cloud_central/ex2/)
- [Exercise 3 - Edit Instances](exercises/hana_cloud_central/ex3/)
- [Exercise 4 - Start, Stop, Upgrade Instances, and Other Actions](exercises/hana_cloud_central/ex4/)

## SAP HANA Cockpit

The SAP HANA cockpit tool provides administration and monitoring of individual SAP HANA Cloud database instances. 

### SAP HANA Cockpit Exercises

- [Exercise 1 - The Database Overview Page](exercises/hana_cockpit/ex1/)
- [Exercise 2 - Configuring Database Properties](exercises/hana_cockpit/ex2/)


## SAP HANA Database Explorer

The SAP HANA database explorer is a web-based tool for browsing and working with  database schema objects such as tables, views, and stored procedures and executing SQL.

### SAP HANA Database Explorer Exercises

- [Exercise 1 - Launch the SAP HANA Database Explorer](exercises/database_explorer/ex1/)

## SAP Business Application Studio

SAP Business Application Studio is a SAP BTP service that offers a modern development environment tailored for business application development.

### SAP Business Application Studio Exercises

- [Exercise 1 - Create a Development Workspace](exercises/business_app_studio/ex1/)
- [Exercise 2 - Create and Deploy Native Database Artifacts Using Guided Development](exercises/business_app_studio/ex2/)
- [Exercise 3 - Additional HDI Container Details (Optional)](exercises/business_app_studio/ex3/)

# Part 2: Administration and Monitoring

### SAP HANA Database Explorer Exercises

- [Exercise 2 - Using the SQL Console](exercises/database_explorer/ex2/)
- [Exercise 3 - Catalog Browser and Object Search](exercises/database_explorer/ex3/)
- [Exercise 4 - Import and Export of HDI Containers](exercises/database_explorer/ex4/)
- [Exercise 5 - HDI container auditing](exercises/database_explorer/ex5)

### SAP HANA Cockpit Exercises

- [Exercise 3 - Managing Alerts](exercises/hana_cockpit/ex3/)
- [Exercise 4 - Monitoring Memory Usage](exercises/hana_cockpit/ex4/)
- [Exercise 5 - Security Basics](exercises/hana_cockpit/ex5/)

### SAP Business Application Studio Exercises

- [Exercise 4 - Access a Table Outside of the HDI Container using a Synonym](exercises/business_app_studio/ex4/)
- [Exercise 5 - Analyze Performance with PlanViz](exercises/business_app_studio/ex5/)


## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.

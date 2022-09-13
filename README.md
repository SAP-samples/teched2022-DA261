# DA261 - SAP HANA Cloud Database Administration and Development

## Description

This repository contains the material for the SAP TechEd 2022 session called DA261 - SAP HANA Cloud Database Administration and Development.  

## Overview

This session introduces attendees to the operations required for end-to-end administration and development of SAP HANA Cloud database instances using the tools offered in the SAP Business Technology Platform (SAP BTP).  Attendees will learn how to accomplish administration tasks such as instance monitoring and security management, as well as development tasks such as creating native SAP HANA artifacts and analyzing their performance.  Part 1 will introduce the tools and deploy some sample tables and calculation views.  Part 2 will demonstrate how to further administer these deployed artifacts.


## Requirements

To complete this workshop, you need access to an SAP BTP account. You can access SAP HANA Cloud from within SAP BTP and you can use a trial, free tier,  or productive version of SAP HANA Cloud.  **This workshop assumes that you already have a SAP BTP account and SAP HANA Cloud database.**  If not, you can register for free at https://www.sap.com/cmp/td/sap-hana-cloud-trial.html.

In your SAP HANA Cloud account (trial or non-trial), perform the following steps:

1.	Enter the **"trial"** subaccount
2.	Enter the **"dev"** space
3.	Click **"SAP HANA Cloud"** from the left navigation bar
4.	Click the button **"Create Instance"** in the top right to invoke the Create Instance wizard
5.	Enter **"DEMO_HANA_DB"** for the instance name
6.	Enter and confirm your administrator password – ***PLEASE REMEMBER IT!***
7.	Click the button **"Create Instance"** at the bottom

A new SAP HANA Cloud instance will be created and this process will take approx. 25 minutes.  You may need to refresh the page to see the instance as "Running" (as opposed to "Creating").

# Part 1: Introduction to the Tools and Initial Project Deployment

## SAP Business Techology Platform (SAP BTP)
SAP BTP brings together data and analytics, artificial intelligence, application development, automation, and integration in one, unified environment enabling you to develop the exact application you need – without investing in on-premise infrastructure.

### SAP Business Technology Platform Exercises

- [Exercise 1 - SAP Business Technology Platform Overview](exercises/sap_btp/ex1/)

## SAP HANA Cloud Central

The SAP HANA Cloud Central tool provides database administrators (DBAs) with a simple and centralized overview of their SAP HANA Cloud databases and SAP HANA Cloud data lake instances. You can also perform management tasks such as creating new instances, checking their status, reviewing any notifications and alerts that might have been raised, examining memory and storage consumption, and start/stop/edit/delete your instances. This section of the workshop will introduce you to the SAP HANA Cloud Central tool and how you can use it to perform different operations.

To begin, ensure you have logged in to the SAP BTP Cockpit and you have navigated to the "SAP HANA Cloud" page.

### SAP HANA Cloud Central Exercises

- [Exercise 1 - Launch SAP HANA Cloud Central](exercises/hana_cloud_central/ex1/)
- [Exercise 2 - Create Instances](exercises/hana_cloud_central/ex2/)
- [Exercise 3 - Edit Instances](exercises/hana_cloud_central/ex3/)
- [Exercise 4 - Start, Stop, Upgrade Instances, and Other Actions](exercises/hana_cloud_central/ex4/)

## SAP HANA Cockpit

The SAP HANA cockpit tool provides administration and monitoring of individual SAP HANA Cloud database instances. With the SAP HANA cockpit, you can monitor resource utilization (memory, CPU and disk), alerts, table usage, SAP HANA services, SAP HANA native storage extensions (NSE), and database performance metrics (threads, sessions, SQL statements, workload classes and connections). You can also administer backups, configuration parameters, table distribution, smart data access (SDA) and smart data integration (SDI). Finally, you can perform security tasks such as user & role management, data encryption, auditing, data anonymization and trust configuration. This workshop guides you through the basic operations to manage SAP HANA Cloud databases.

### SAP HANA Cockpit Exercises

- [Exercise 1 - The Database Overview Page](exercises/hana_cockpit/ex1/)
- [Exercise 2 - Configuring Database Properties](exercises/hana_cockpit/ex2/)


## SAP HANA Database Explorer

The SAP HANA database explorer is a web-based tool for browsing and working with SAP HANA database objects such as tables, views, functions, stored procedures, executing SQL statements, importing and exporting data, debugging SQLScript, working with multi-model data such as graph, spatial and JSON collections,  viewing trace files, and creating remote sources.  As of March 2021, it also offers support for Data Lake IQ connections.

### SAP HANA Database Explorer Exercises

- [Exercise 1 - Launch the SAP HANA Database Explorer](exercises/database_explorer/ex1/)

## SAP Business Application Studio

SAP Business Application Studio is a SAP BTP service that offers a modern development environment tailored for business application development.

With the enablement of the SAP HANA tool extensions are added, it can be used to build and deploy native SAP HANA database artifacts such as tables and calculation views.  


### SAP Business Application Studio Exercises

- [Exercise 1 - Create a Development Workspace](exercises/business_app_studio/ex1/)
- [Exercise 2 - Create and deploy a project using the SAP HANA Getting Started Wizard](exercises/business_app_studio/ex2/)


# Part 2: Administration and Monitoring

### SAP HANA Database Explorer Exercises

- [Exercise 2 - Using the SQL Console](exercises/database_explorer/ex2/)
- [Exercise 3 - Catalog Browser and Object Search](exercises/database_explorer/ex3/)

### SAP Business Technology Exercises

- [Exercise 2 - Services and keys](exercises/sap_btp/ex2/)


### SAP HANA Cockpit Exercises

- [Exercise 3 - Managing Alerts](exercises/hana_cockpit/ex3/)
- [Exercise 4 - Monitoring Memory Usage](exercises/hana_cockpit/ex4/)
- [Exercise 5 - Security Basics](exercises/hana_cockpit/ex5/)

### SAP Business Application Studio Exercises

- [Exercise 3 - Analyze Performance with PlanViz](exercises/business_app_studio/ex3/)

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.

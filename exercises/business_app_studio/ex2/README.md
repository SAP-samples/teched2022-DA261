# Exercise 2 - Create and deploy a project containing database artifacts using the SAP HANA Getting Started Wizard

This exercise will demonstrate how to create a project containing tables and calculation views using the Getting Started wizard.  

## Exercise 2.1 Creating Database Objects with HDI vs SQL

Explain the benefits of HDI and when to use HDI vs native SQL.
HDI deployment is all or nothing.  (same for SQL with the right automcommit setting?)
Calc View modeler.
Multiple developers working with the same objects can each have their own isolated deployment.
Is it a way to provide isolatation while using one HANA database?
How does this differ from the upcoming (internal only) HANA Cloud multi-tenancy?
Schema less development.

TODO Volker
### Why HDI
 - HDI stands for SAP HANA Deployment Infrastructure
 - HDI is integral part of SAP HANA and SAP HANA Cloud
 - HDI is a scalable design-time \ runtime environment
 - Supports most standard database artifacts like tables, procedures, views, virtual tables, roles
 - Support for advanced SAP HANA artifacts like calculation views, flowgraphs, replication tasks…
 - Determines correct deployment order
 - <B>Evolves the runtime objects</B>
 - Re-deployment of dependent artifacts
 - Transactional all-or-nothing principle
 - Can be generated from higher-level language like CAP CDS
 - Simplifies the need for the developer to write DDL and DML to get schema evolution
 - Eases deployment in a multi-tenant environments


The last step of Ex1 of DBX demonstrating creating a few objects with SQL.


## Exercise 2.2 Create a New SAP HANA Database Project from a Template

1. In the SAP Business Application Studio, start the Guided Development Wizard by selecting it from the bottom of the Welcome screen, or select the View, Find Command menu (or Fn F1) to open the command palette and search for SAP HANA and select the option shown below.

    ![](images/getting-started.png)

    It may take a moment or two for the contents of the Guided Develpment Wizard to appear.  If it does not appear, try reloading the page.
    TODO Volker ... is this a known issue?
    The wizzard is a quite large piece of code and may take a while to show up. It contains all the source code and of course the yeoman part as well.

2. Select Get Started with SAP HANA Cloud.

    ![](images/guided-development.png)

    Select the first sub option Create a New SAP HANA Database Project from a Template.

    ![](images/create-project.png)

    Press Next multiple times to accept the defaults.

    When asked for provide your Cloud Foundry user id and password and select login.

    ![](images/log-in.png)

    Select the option to Open the Output View when asked.

    ![](images/open-output.png)

    The bottom panel can also be shown (or hidden) by selecting View, Toggle Bottom Panel or by the icon in the bottom right.

    ![](images/output.png)

3. In the project explorer, open the generated project.

    ![](images/open-project.png)

4. Examine the created project.

    ![](images/project.png)

    TODO Volker, explain what has just happened, HDI container created, service keys etc.  Maybe some content on what an HDI container is?
    An HDI container is construct one can also describe as a glorified set of schemas. 
    

## Exercise 2.3 Initialize the Git Reprository

1. The Git repository will be initialized now so that after subsequent steps it can be easily seen what changes have been made to the project.

    ![](images/git-init.png)

2. Commit the contents of the project and provide a commit message such as initial commit.  The green U stands for unstaged.

    ![](images/commit.png)

## Exercise 2.4 Add Database Artifacts

1.  In the Getting Started wizard, select Add Database Artifacts.

    ![](images/add-tables.png)

2. Complete all the steps to create two tables (PASSENGERS and FLIGHTRESERVATION), deploy these into tables, and to open the SAP HANA database explorer to view the deployed tables.

    ![](images/tables-in-dbx.png)

3. Note that the new files are again marked with a green U which means they are unstaged or new files.

    ![](images/git-integration.png)

    Commit the changes and continue to do so afer subsequent steps.

    Note that in this way you will have a record of the changes from each step that can be viewed or the project can be restored to the state of a previous commit.

    ![](images/git-history.png)

    For additional details see [Working with GIT Within SAP Business Application Studio](https://learning.sap.com/learning-journey/developing-applications-running-on-sap-btp-using-sap-hana-cloud/working-with-git-within-sap-business-application-studio_532f4c05-c108-4737-af9f-dd31c9c5707c) and [Git Source Control](https://help.sap.com/docs/SAP%20Business%20Application%20Studio/9d1db9835307451daa8c930fbd9ab264/9689c07b64364bbea43725dad9f27320.html).

## Exercise 2.5 Load Data into your SAP HANA Cloud Application's Database Tables

1.  In the Getting Started wizard, select Load Data into your SAP HANA Cloud Application's Database Tables.

2. Complete all the steps to load data into the two previously created tables and to view the deployed data in the SAP HANA database explorer.

    ![](images/data-in-tables.png)

## Exercise 2.6 Create a Calculation View for your Application

Calculation views allow the developers to express their intent instead of defining with SQL code how the data should be processed.

1.  In the Getting Started wizard, select Create a Calculation View for your Application.

2. Complete all the steps to create and deploy a calculation view and view its properties in the SAP HANA database explorer.  It may take a moment or two for the calculation view editor to load after its creation.  Note that the permissions to view its data will be granted in the next step. 

    ![](images/calc-view.png)

## Exercise 2.7 Create Analytic Privileges for your Calculation View

1.  In the Getting Started wizard, select Create Analytic Privileges for your Calculation View and complete the steps.

2. TODO Volker, why does it suggest opening dbx here?  

## Exercise 2.8 Create a Database Role for the Analytic Privilege

1.  In the Getting Started wizard, select Create a Database Role for the Analytic Privilege and complete the steps.

2. I get a insufficient privilege: Detailed info for this error can be found with guid 'D00DD9BE37D9B749B81DCBB1C1B0990A'
 when I try to view the data for the calculation view.  TODO Volker, what are some debugging/tips to help ensure that everything was created properly.

2. Show the data preview functionality in DBX when viewing the data of the calculation view.  Perhaps show count passenger ID by airline.

## Exercise 2.9 Create a Database Procedure File

1.  In the Getting Started wizard, select Create a Database Procedure File and complete the steps.

2.  In the SAP HANA database explorer, call the stored procedure.

    ![](images/call-stored-procedure.png)

3.  In the SAP HANA database explorer, attempt to debug the stored procedure by selecting Open for Debugging, placing a breakpoint on the last line of the stored procedure, and then call the stored procedure again.

    ![](images/debug-stored-procedure.png)

## Summary

You now have now created native SAP HANA database artifacts and deployed them into an HDI container.

Continue to - [Exercise 3 - Exercise 3 Description](../ex3/README.md)


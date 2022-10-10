# Exercise 2 - Catalog Browser and Object Search

In this exercise, we will explore some of the functionality that the catalog browser and object search provide when working with database objects.  Some of this functionality was previously introduced in the exercise that created the tables, calculation view, and stored procedure in the SAP Business Application Studio.

1. Database objects can be viewed in the catalog browser as shown below.

    ![](images/tables.png)

    Alternatively, a table can be found by selecting **Tables** and choosing **Show Tables** from the context menu.
    
    ![](images/TablesInCatalogBrowser.png)

    Additional filters can be applied in this view by clicking on the column header and the list of columns displayed can specified.  

2. A create, select, or insert statement for database objects such as a table or views can be generated as shown below.

    ![](images/GenerateInsert.png)

3. A stored procedure's create statement can be viewed on its properties page.

    ![](images/StoredProcedureSource.png)

4. A graphical debugger can be used.

    ![](images/OpenForDebugging.png)

    *Add a breakpoint on line 19*

    To trigger the breakpoint, call the stored procedure.

    ![](images/CallStoredProcedure.png)

    Once the breakpoint has been hit, the variables can be examined and the code stepped through.

    ![](images/Debugging.png)

5. The source code for a specific stored procedure, for all stored procedures in a schema, or for all stored procedures in a database can also be analyzed.  This can provide suggestions for code quality, security, or performance 

    ![](images/AnalyzeSQLScriptCode.png)

6. Database objects can also be found using the object search.  The below search looks for any objects that use FLIGHTRESERVATION in their definitions in the HDI connection. 

    ![](images/ObjectSearch.png)

    An object can be double clicked on to open its properties page.

    ![](images/OpenInDatabaseBrowser.png)

7. Statement Library
    TODO, add content.  Perhaps it is enough to highlight system vs user.  Add a user statement relevant to the tables and point to additional content of the mini checks.  Consider adding the TechE2021 mini check example to the DBX tutorial.

8. Database diagnostic files can also be viewed or downloaded. 

    ![](images/DiagnosticFiles.png)

    Additional instructions showing how to enable a SQL and expensive statement trace are available in the tutorial [Troubleshoot SQL with SAP HANA Database Explorer](https://developers.sap.com/tutorials/hana-dbx-troubleshooting.html).  For more on executed statement tracing see [SAP Note: 2366291 - FAQ: SAP HANA Executed Statements Trace](https://launchpad.support.sap.com/#/notes/2366291).



This concludes the exercises on the catalog browser and object search.

Continue to - [Exercise 3 - Using the SQL Console](../ex3/README.md)
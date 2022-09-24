# Exercise 3 - HDI Containers in Depth (Optional)

This exercise will further examine the deployed HDI container.  


## Exercise 2.1 Opening a SQL Console as Admin

1.  In the SAP HANA database explorer, open a SQL Console connected to the HDI container.  Execute the following SQL.

    ```SQL
    SELECT * FROM USERS WHERE USER_NAME LIKE '%FLIGHT%';
    SELECT * FROM SCHEMAS;
    SELECT CURRENT_USER, CURRENT_SCHEMA FROM DUMMY;
    SELECT * FROM M_JOBS;  --Fails 
    ```
    
    Notice that the user is the _RT or run time user as opposed to the design time user.
    If you want to access the DT view you have to use the "ADMIN" container access in Database Explorer.

    ![](images/open-admin.png)

    Here is a blog on this topic:
    https://blogs.sap.com/2022/06/13/can-i-see-the-hana-deployment-history/

2.  The design time user has some additoinal privileges.  
TODO Volker what can be shown here?

## Exercise 2.12 Examining the Contents of the HDI Container

1.  In the SAP HANA database explorer, open the parent database of the HDI container.  Notice that you can see the schema and objects but do not have privileges to query them.

    TODO, demonstrate this

## Summary

You have now have a better understanding of some of the HDI concepts.

Continue to - [Exercise ? - Description](../ex?/README.md)


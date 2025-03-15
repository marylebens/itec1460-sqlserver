# SQL Server Repository for ITEC2505-Visual C# .NET Programming

This repository is desgined for students to learn SQL using a Microsoft SQL Server database. This repo contains a Microsoft SQL Server database server that is running in a [Docker](https://www.docker.com) container.

## Setting up the development container

### GitHub Codespaces

Follow these steps to open this sample in a Codespaces:

1. Click the Code drop-down menu and select the **Codespaces** tab.
1. Click on **Create codespaces on main** at the bottom of the pane.

For more info, check out the [GitHub documentation](https://docs.github.com/en/free-pro-team@latest/github/developing-online-with-codespaces/creating-a-codespace#creating-a-codespace).


## Things to try

1. **Connect via SQLCMD and create a new database**

    SQLCMD is already installed within the container. You can use it from the **Terminal** tab, using the *bash* shell. For example, you can execute a SQL Script. This example creates a new Northwind database and populates it with data.

    ```sql
    sqlcmd -S localhost -U sa -P P@ssw0rd -d master -i 01-CreateDatabase.sql
    ```

    > Note: The SQL Server instance is created with user `sa` and password `P@ssw0rd`. Y

2. **Explore your database with SQL Server extension**

    SQL Server extension allows you to explore your SQL Server and Azure SQL instances right within Visual Studio Code. Let's explore the database we have just created.

    - On the primary sidebar (on the left), click on **SQL Server** tab.
    - The _SQL Server_ pane appears. You should already see `mssql-container` listed. Click on it
    - Type the password listed previously
    - The treeview will be populated with Database items. For example, you can explore the tables or even select the rows in the `dbo.Users` table created with the SQL Database project at the previous step.



## License

Modified by Dr. Mary Lebens and Licensed under the MIT License. See LICENSE in the project root for license information.



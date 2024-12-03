# DataBases

[Visit Class notes for 15 June](https://directdevops.blog/2024/06/15/multi-cloud-classroom-notes-15-june-2024/)

* Relational databases are not scaled, this can be replicated. the replicated servers will accept only read.

* if you have two server , the second is replication server of 1st server , incase 1st server goes down the write operation fails we need to make server 2 to accept writes this is called as **Failover**

### AWS Relational Databases 

[Check notes for understanding concepts](https://directdevops.blog/2024/06/16/multi-cloud-classroom-notes-16-june-2024/)


Brief Revew :

* Types of Databases:
    * Structured
    * Unstructured
  
* Structured:
    * RDBMS(Relational databases)
        * MYSQL
        * Oracle
        * MSSQL
        * Postgres

* UnStructured:(These are not strict on schema)
    * NO SQL

* For this, cloud offered service named Database as a service, here we just need to maintain data
    * AWS:
        * AWS has a service named RDS, here in RDS they support 5 engines
            * MYSQL
            * MS SQL
            * Oracle
            * Postgres
            * IBM DB2
        * Aws re-written databases engines and started giving as Aurora Databases, Main advantages using this is your throughput will be faster(Accessing data is faster, your quires will be faster)
        * For No Sql
            * Aws has a propritery Database which is widely used called 'Dynamo Db', amazon created for themselves to store their data
            * Dynamo Db is very fast in creation and very fast in quering 
            * select *(All) operation is a costliest option, the way you design the data chnage
            * Mongo Db-(Document Db)
            * Cassandra (Keyspaces)
            * For running Graph databases we have Neptune
        * Cache :
            * Aws has two things
                * Elstic cache(this runs on opensources of Redis cache software)
                * Mem Cache(Enterprice editions of Redis)
            
    * Azure:
        * Azure Sql(This support three types of databases)
            * MS SQL
            * Postgres
            * MY SQL
        * Here some databases will be your part of network and some not
            * Azure SQL is not part of Our network
        * Since microsoft SQL gives you a cheaper way of SQL server they gave three options
            * Azure SQL Database:(it is not a complete sql sever but it have all features of database) A fully managed, scalable, and intelligent relational database service in the cloud, ideal for modern app development.

            * Azure SQL Managed Instance: A fully managed SQL Server instance that offers near-complete SQL Server compatibility with all the benefits of a managed service.

            * SQL Server on Azure Virtual Machines: A cloud-based virtual machine running SQL Server, providing full control over the SQL Server instance and operating system, ideal for custom configurations and legacy applications.
        * For NO SQL
            * Azure has CosmosDB
                * in cosmosdb they will provide APi's to create differernt types of no Sql databases
                * Cassandra APi 
                * Mongo APi
                * etc..
        * Cache:
            * In azure we have Azure Redis Cache

* Backups:
    * If you want to take backups of any Database, generally there is automatic
    * you can also take by centralizing from backup service 
        * in Azure(Azure backup center ) 
        * In AWs(AWS backup service)
    * Here you need to create a vault with some plan based on how frequently is has been used.
* Recovery
    * recovery do not exist for databases, all you need to do is restore
    * for virtual machines Azure has Recovery services Vault, here you can recover 
    * Aws has Disaster recovery services.

    
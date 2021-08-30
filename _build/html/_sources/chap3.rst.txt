.. _chap3:

Data Storage
============

Data Table
----------

A data table is similar to a standard relational database table, but differs greatly in terms of performance. Generally, data tables should be used if you have less than 100,000 rows of data. For larger datasets, a relational database should be used and then connected via a Database Thing template. A Data Shape defines the columns or fields of the data table.

.. Caution:: If a data table is using a custom data shape that defines the timestamp field with a different data type, an error will occur when executing a query service.

A data table has the following predefined fields:

• **Timestamp:** The time the entry was created. It is also possible to provide a timestamp when adding a data table entry.
• **Tag:** Each data table entry can be tagged. Data tags help to search for and consume specific run time data.
• **Source:** The source of the data table entry. This is usually the name of the Thing writing to the data table or an identifier of an external system.
• **SourceType:** The entity type of the source (such as Thing or user).
• **Location:** The location of the data table entry's source.



Data Table Templates
--------------------
The configuration for a data table allows you to define additional table indexes. This is similar to a relational database table, where in addition to the primary key (the primary key is defined in the Data Shape), you need to query the table based on other fields. 


+-----------------+----------+-----------+-----------+-----------+-----------+-----------+-----------+
| Name            |                              Description                                         |
+=================+==========+===========+===========+===========+===========+===========+===========+
| ContentCrawler  | A content crawler Thing is used to call a service on another entity.             |
|                 |                                                                                  |
+-----------------+----------+-----------+-----------+-----------+-----------+-----------+-----------+
| DataTable       | DataTable Stores non time-series data.                                           |
|                 |                                                                                  |                                                                         
+-----------------+----------+-----------+-----------+-----------+-----------+-----------+-----------+
| ContentCrawler  | Creates a local proxy object to a data table Thing that is running.              |
|                 |                                                                                  |
+-----------------+----------+-----------+-----------+-----------+-----------+-----------+-----------+


           

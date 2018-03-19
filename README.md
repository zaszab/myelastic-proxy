# MyElastic proxy

MySQL proxy using read-write query split. Helps seperating your queries: all SELECT queries will go the read server, every other to the write.

https://www.myelastic.io/

### Installation

Download the source and edit the proxysql.cnf. Add the writer and reader MySQL server IP address or hostname. Create a mysql user in your database and fill it in the config.

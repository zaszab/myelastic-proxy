# MyElastic proxy

MySQL proxy using read-write query split. Helps seperating your queries: all SELECT queries will go the read server, every other to the write.

https://www.myelastic.io/

### Installing to production

You can create a high-available read-write split mysql proxy on AWS less then $30/month. I have created a documentation how to do that with AWS Aurora. It is compatible with AWS RDS MySQL too, or any other master-slave mysql cluster.

http://bit.ly/2GGmNf8

### Testing locally

You can download the source to your local machine. You will need Docker installed.
Edit the proxysql.cnf, add the writer and reader MySQL server IP address or hostname. Create a mysql user in your database and fill it in the config. Then run docker run.

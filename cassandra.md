# Install Cassandra database installation -- Dokcer

**step:1**
-------------
*Starting cassandra instance. -- first time*
```bash
docker container run -d --name cassandra-node -p 9042:9042 cassandra
```

*Run cassandra*

```bash
docker start cassandra-node
```

*Access Bash*
```bash
docker exec -it cassandra-node bash
```

*Access Cassandra Shel*
```bash
cqlsh
```

*Create Keyspace*
```sql
-- Create a keyspace
CREATE KEYSPACE IF NOT EXISTS store WITH REPLICATION = { 'class' : 'SimpleStrategy', 'replication_factor' : '1' };
```

*Check all the keyspaces*
```
desc keyspaces
```
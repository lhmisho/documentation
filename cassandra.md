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

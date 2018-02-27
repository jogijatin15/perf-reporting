# Performance test reporting using Jmeter, InfluxDB and Grafana

### Start the containers
```shell
docker-compose build
docker-compose up -d
```

### Execute Jmeter JMX file
JMX file is executed as a maven project.
```
mvn verify
```


### URLs
Hit the below URLs to open the tools running on containers
```
Jmeter:				http://localhost:2003
InfluxDB Admin:			http://localhost:8083
Grafana:			http://localhost:3000 [Username & Password: admin/admin]
```

### Access InfluxDB Container
```shell
docker exec -it {container_id} /bin/bash
```
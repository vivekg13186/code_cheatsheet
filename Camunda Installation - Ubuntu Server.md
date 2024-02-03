[https://docs.camunda.io/docs/self-managed/platform-deployment/manual/#download-and-run-elasticsearch](https://docs.camunda.io/docs/self-managed/platform-deployment/manual/#download-and-run-elasticsearch)

## Elastic Search Setup
1. Download .tar file `curl  https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.16.2-linux-x86_64.tar.gz --output es_7.16` 
2. Unzip the file `tar -xzf es_7.16`
3. `rm -fr ex_7.16`
4. `./bin/elasticsearch`
5. Create new user `./bin/elasticsearch-users useradd vivek`
6. Add role to new user `./bin/elasticsearch-users roles vivek -a superuser`
7. Test connection using `curl  https://localhost:9200`

## Camunda Local Setup
 1. `curl https://github.com/camunda/camunda-platform/releases/download/8.2.8/camunda-identity-8.2.8.tar.gz --output camunda-identity`
 2. `curl https://github.com/camunda/camunda-platform/releases/download/8.2.8/camunda-operate-8.2.8.tar.gz --output camunda-operate`
 3. `curl https://github.com/camunda/camunda-platform/releases/download/8.2.8/camunda-tasklist-8.2.8.tar.gz --output camunda-tasklist`
 4. `curl https://github.com/camunda/camunda-platform/releases/download/8.2.8/camunda-zeebe-8.2.8.tar.gz --output camunda-zeebe`
 5. `tar -xvf camunda-identity`
 6. `tar -xvf camunda-operate`
 7. `tar -xvf camunda-tasklist`
 8. `tar -xvf camunda-zeebe`

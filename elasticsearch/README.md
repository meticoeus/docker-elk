

### Fixing Elasticsearch
```
docker-machine start default \
&& docker-machine ssh default "sudo sysctl -w vm.max_map_count=262144" \
&& docker ps \
&& docker-compose up -d
```
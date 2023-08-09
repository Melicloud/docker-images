This image contains:

* alpine
* mysql-client
* jq

# Usage
```bash
export _tag=`date +%Y%m%d`
docker build -t 036221503996.dkr.ecr.eu-west-1.amazonaws.com/alpine-mysql:$_tag .
docker push 036221503996.dkr.ecr.eu-west-1.amazonaws.com/alpine-mysql:$_tag
```
This image contains:

* alpine
* mysql-client
* jq

# Usage
```bash
export _tag=`date +%Y%m%d`
docker buildx build --platform linux/amd64 -t public.ecr.aws/d9k2s2v9/alpine-mysql:$_tag .
docker push public.ecr.aws/d9k2s2v9/alpine-mysql:$_tag
```
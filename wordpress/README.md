This image contains:

* wordpress


# Usage
```bash
export _tag=`date +%Y%m%d`
docker buildx build --platform linux/amd64 -t public.ecr.aws/v2h5r4g8/wordpress:$_tag .
docker push public.ecr.aws/v2h5r4g8/wordpress:$_tag
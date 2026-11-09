# mongodbtools-with-awscli

This is a debian/ubuntu based image that contains:
* mongo database tools
* awscli

We use either debian or ubuntu, and use the public [mongo-database-tools download](https://www.mongodb.com/try/download/database-tools) as outlined in [guide](https://www.mongodb.com/docs/database-tools/installation/?operating-system=linux&package-type=deb)

##  Usage (Local dev)
```bash
export _tag=100-20-1-trixie
docker build --platform linux/amd64 -t public.ecr.aws/a7r6j8c8/mongodbtools-aws:$_tag .
docker push public.ecr.aws/a7r6j8c8/mongodbtools-aws:$_tag
```

## CICD

The deployment for this image builds only on push of a tag formatted as `mongodbtools-aws-*` to the repo. Please use the mongo database tools and the debian/ubuntu version in the tag, e.g mongodbtools-aws-100-20-1-trixie for the image to be tagged as public.ecr.aws/a7r6j8c8/mongodbtools-aws:100-20-1-trixie.

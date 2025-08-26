# postgresclient-with-awscli-openvpn

This is a debian/ubuntu based image that contains:
* postgres client
* awscli
* openvpn

We use either debian or ubuntu, depending on which of the two has postgresql-client available in a stable release. References:

- https://packages.debian.org/search?keywords=postgresql-client
- https://launchpad.net/ubuntu/+search?text=postgresql-client

##  Usage
```bash
export _tag=15.5-bookworm
docker build -t public.ecr.aws/d9k2s2v9/postsgreql-aws-openvpn:$_tag .
docker push public.ecr.aws/d9k2s2v9/postsgreql-aws-openvpn:$_tag
```

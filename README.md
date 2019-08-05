# docker_scoutsuite

This is a Dockerised version of [NCC Group's ScoutSuite](https://github.com/nccgroup.scoutsuite). Currently it's only been tested for AWS, as that's what most of my requirements are at the moment. It should also work with GCP/Azure at the moment, but that's not been tested yet. 

Usage:

```
docker run --rm -e "AWS_ACCESS_KEY_ID=xxxxx" -e "AWS_SECRET_ACCESS_KEY=xxxxx" -v {host_path_for_report}:/reportdir scout aws --report-dir /reportdir
```
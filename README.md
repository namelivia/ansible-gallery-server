# Gallery client Ansible role

## This is a WIP

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/namelivia/ansible-gallery-server
```

## Required variables

 - `cloudwatch_region` Cloudwatch region to send the logs to.
 - `cloudwatch_log_group` Cloudwatch log group to send the logs to.
 - `gallery_api_endpoint` API endpoint for connecting the client to the server API.
 - `user_info_service_endpoint` API endpoint for user information service.
 - `aws_access_key_id` Access key id to access the images S3 bucket.
 - `aws_secret_access_key` Secret key to access the images S3 bucket.
 - `aws_default_region` Region for the images S3 bucket.
 - `aws_bucket` Name for the images S3 bucket.
 - `domain_name` Domain name in wich the application will be served from.

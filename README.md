# Automating AWS with Python

## 01-script

This script will sync a local directory to an s3 bucket, and optionally configure Route 53 .

### Features

Webotron currently has the following features:

- List bucket
- List contents of a bucket
- Create and set up bucket
- Sync directory tree to bucket
- Set AWS profile with --profile=<profileName>
- Configure route 53 domain

### Usage

Usage: script.py [OPTIONS] COMMAND [ARGS]...

this will deploys websites to AWS.

Options:
--profile TEXT Use a given AWS profile.
--help Show this message and exit.

Commands:
list-bucket-objects List objects in a s3 bucket.
list-buckets List all s3 buckets.
setup-bucket Create and configure s3 bucket.
sync Sync contents of PATHNAME to BUCKET.

### Examples

List all my S3 buckets with profile admin:
python script.py --profile=admin list-buckets

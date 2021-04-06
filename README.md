# aws-cli

Docker image for AWS CLI, also source for the AWS CLI GitHub Action.

## Example Usage

```
- name: S3 Sync
  uses: giboow/action-aws-cli@v1
  with:
    args: s3 sync --delete --acl public-read localdir/ s3://remote-bucket/
  env:
    AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
    AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    AWS_DEFAULT_REGION: "eu-west-3"
```

## Source
I have duplicate [ItsKarma/aws-cli](https://github.com/ItsKarma/aws-cli) repository, my action use the latest aws-cli version. 
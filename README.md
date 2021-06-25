# github-last-deploy-diff
Get the list of file names which are changed between last successful deploy and current run


## Action inputs

The following settings must be passed as environment variables as shown in the example. Sensitive information, especially `aws_key_id` and `aws_secret_access_key`, should be [set as encrypted secrets](https://help.github.com/en/articles/virtual-environments-for-github-actions#creating-and-using-secrets-encrypted-variables) — otherwise, they'll be public to anyone browsing your repository's source code

| name                    | description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| `AWS_KEY_ID`            | (Required) Your AWS Access Key. [More info here.](https://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html) |
| `AWS_SECRET_ACCESS_KEY` | (Required) Your AWS Secret Access Key. [More info here.](https://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html) |
| `AWS_BUCKET`            | (Required) The name of the bucket you're upload to.
| `AWS_REGION`            | (Required) The AWS region where the bucket is located.


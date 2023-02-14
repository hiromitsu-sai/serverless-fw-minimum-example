# sample-service

Minimum sample of Serverless Framework with python3 that can deploy to AWS.

# Reference

* Real Example - https://serverless.co.jp/blog/25/
* `serverless.yml` reference - https://www.serverless.com/framework/docs/providers/aws/guide/serverless.yml

# How to Create this Project

```bash
$ serverless create --template aws-python3 --name sample-service --path sample-service

✔ Project successfully created in "sample-service" from "aws-python3" template (5s)
$
```

# How to Deploy

```bash
$ aws configure --profile dev  # set access key and secret
$ serverless deploy --aws-profile dev --stage dev # deploying with aws dev profile

Deploying sample-service to stage dev (ap-northeast-1)

✔ Service deployed to stack sample-service-dev (116s)

functions:
  hello: sample-service-dev-hello (389 B)

Need a better logging experience than CloudWatch? Try our Dev Mode in console: run "serverless --console"

$
```

# How to Remove

```bash
$ serverless remove --aws-profile dev
Removing sample-service from stage dev (ap-northeast-1)

✔ Service sample-service has been successfully removed (17s)
$
```


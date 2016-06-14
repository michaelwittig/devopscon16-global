# DevOpsCon 2016: The Life of a Serverless Microservice on AWS

Global resources needed by all services.

## Setup

0. Create CloudFormation stac based on `global.json` template.
1. Upload public SSH Key to IAM user
2. For each service
  0. Create repo in CodeCommit us-east-1 (N. Virgina)
  1. `git clone ssh://***@git-codecommit.us-east-1.amazonaws.com/v1/repos/xxx-service`
  2. deploy xxx-service-pipeline stack baesd on `pipeline.json` template
  3. edit pipeline and reconnect with Solano CI
  4. remove disabled stage transition
  5. release change to rerun pipeline

## See also

* https://github.com/michaelwittig/devopscon16-auth-service
* https://github.com/michaelwittig/devopscon16-profile-service
* https://github.com/michaelwittig/devopscon16-location-service

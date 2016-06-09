0. Upload public SSH Key to IAM user
1. For each service
  0. Create repo in CodeCommit us-east-1 (N. Virgina)
  1. git clone ssh://APKAIB7BO6QQA4FTLRNQ@git-codecommit.us-east-1.amazonaws.com/v1/repos/xxx-service
  2. deploy xxx-service-pipeline stack baesd on pipeline.json template
  3. Edit pipeline and reconnect with Solano CI
  4. remove disabled stage transition
  5. release change to rerun pipeline
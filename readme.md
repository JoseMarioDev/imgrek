Serverless image recognition app built using core AWS services

1. Cognito
2. API Gateway
3. S3
4. SQS
5. Lambda
6. DynamoDB
7. Rekognition

![app architecture](img/imgrek-arch.jpeg)

### Ep. 1

- setup cdk
- setup S3 image bucket
  - used for storing the imgs for our app
  - output to cfn
- setup DynamoDB
  - table 'Image'
  - output to cfn
- built Lambda function
  - python runtime
  - envs: table and imagebucket
  - add event source
  - grant permissions to imagebucket and tble
  - add IAM policy
- end of episode - cdk destroy to cleanup

### Ep. 2

- creating lambda fun to interact with the api gateway
- setting up dynamodb table to interact with the Lambda api Fn
- creating s3 bucket for thumbnails to be stored after being sent to rekognition

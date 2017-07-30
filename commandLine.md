# Command Line Arguments for Lambda Deployment with Claudia

1. Install claudia as global npm utility

`npm install claudia -g`

2. Initial deploy to lambda

`claudia create --region us-east-1 --handler lambda.handler --profile personal-account`

*Last arg specifies aws keys to use in .aws/credentials*

3. Invoke lambda function from console

`claudia test-lambda --profile personal-account`

4. 

# Command Line Arguments for Lambda Deployment with Claudia

* Install claudia as global npm utility

`npm install claudia -g`

* Initial deploy to lambda

`claudia create --region us-east-1 --handler lambda.handler --profile personal-account`

*Last arg specifies aws keys to use in .aws/credentials - could instead use AWS_PROFILE=personal-account claudia... or define this ENV variable elsewhere*

* Invoke lambda function from console

`claudia test-lambda --profile personal-account`

* Invoice lambda function with test event

`claudia test-lambda --event event.json --profile personal-account`

# Chatbot
Generic Chatbot for managing appointments using Amazon Lex. Separate Chatbot stack for each client specific to their schedule requirement

Steps to deploy the project:
	Create a S3 bucket in the region you are deploying the chatbot.

	Upload zip of the source code in the S3 bucket created in step-1. (name it package.zip since CloudFormation defaults to package.zip, although you can change it in CloudFormation as well)

	Go to CloudFormation and upload CloudFormation template.

	In ChatBotLambdaCodeS3BucketName, enter bucket name created in step-1.

	In ChatBotLambdaCodeS3ObjectKey, enter zip file name uploaded in step-2.

	Optionally change any other parameter you wish to.

	Create CloudFormation.

	In Chatbot json, change ARN of the lambda to the newly created lambda in step-7. NOTE: There are three places which need Lambda ARN.

	Package the json in a zip and import it in the amazon lex.

	Once import is done, build and test!

	For publishing Chatbot, follow instructions here.



Sign in to AWS Amazon and then click on Lambda under services. This page will show the lambda functions list, which is already created.

Here are the steps required to create our lambda:
"Select Author from scratch"
“Configure triggers” (in our case we don't have any triggers or events)
“Configure function”:
Name: Provide LambdaRequestStreamHandler,
Description: Anything that describes our lambda function
Runtime: Select java8
Code Entry Type and Function Package: Select “Upload a .ZIP and Jar file” and click on “Upload” button. Select the file which contains lambda code.
Under Lambda function handler and role:
Handler name: Provide lambda function handler name com.dinesh.LambdaRequestStreamHandler::handleRequest
Role name: If any other AWS resources are used in lambda function, then provide access by creating/using existing role and also define the policy template.
Under Advanced settings:
Memory: Provide memory that will be used by our lambda function.
Timeout: Select a time for execution of lambda function for each request.
Once you are done with all inputs, click “Next” which will show you to review the configuration.
Once a review is completed, click on “Create Function”.

Test:
create new test event in the lambda function and trigger

Find sample in the below web site:
https://www.baeldung.com/java-aws-lambda

Find so many AWS/java examples in the below  git hub location,

https://github.com/eugenp/tutorials/tree/master/aws

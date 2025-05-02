# Serverless Web Application
This hands-on lab demonstrates how to build and troubleshoot a serverless web application using AWS services, including Lambda, DynamoDB, S3, API Gateway, and X-Ray for tracing.

# 🛠️ Features
Created a DynamoDB table and populated it with data from items.json

Developed a Lambda function to interact with DynamoDB and configured it for Python 3.9

Set up an API Gateway endpoint for the Lambda function

Configured S3 static website hosting

Enabled X-Ray tracing for Lambda and API Gateway

Implemented Lambda Layer for enhanced functionality

# 📦 Requirements
AWS Account with necessary permissions

AWS CLI installed and configured

Python 3.9 environment for Lambda function

Basic knowledge of AWS services (Lambda, S3, DynamoDB, API Gateway, X-Ray)

# 🚀 Setup Instructions
1. Create the DynamoDB Table
     Create a DynamoDB table using the AWS Management Console.
     Populate the table with data from the items.json file located in the Building_and_Troubleshooting_a_Serverless_Web_Application folder.

2. Create the Lambda Function
     Create a new Lambda function using the lambda_function.py file.
     Configure the Lambda function to use Python 3.9 and 256 MB of memory.
     Test the function to ensure it works.

3. Diagnose and Fix Lambda Errors
   If any errors occur during testing, diagnose and fix them based on error messages or logs.

4. Create API Gateway Endpoint
   Once the Lambda error is fixed, create a function URL endpoint for your Lambda using API Gateway.
   Modify index.html to include the invoke URL of your API Gateway endpoint.

5. Create S3 Bucket for Website Hosting
   Create an S3 bucket with public access enabled.
   Upload the following website files to the bucket with public-read permissions:index.html,error.html,cookie.html
   Enable static website hosting in the S3 bucket settings.
   Verify you can access the website via the S3 website-hosting URL.

7. Enable Lambda Tracing
   Enable tracing for the Lambda function from within the Lambda settings.
   Ensure that the API Gateway endpoint is configured to send traces.

8. Add Lambda Layer
   Upload the Lambda Layer using the layer.zip file.
   Ensure you select Python 3.9 as the runtime for compatibility.
   Update your Lambda function code to import the X-Ray SDK using the lambda_function_xray.py snippet provided.
   Test the function again to ensure it works with the layer.

8. Diagnose and Fix Errors in Lambda Configuration
   If there are any issues, diagnose and resolve them based on the error messages or logs.

9. Generate Website Traffic
   Visit the website to generate traffic and test the setup.
   Ensure the Lambda function, API Gateway, and S3 static website hosting are working as expected.

10. Review X-Ray Traces and Service Map
    Open the X-Ray console to view the service map and traces.
    Verify that the Lambda function and API Gateway traces are correctly captured and displayed.

# 🧰 Skills Demonstrated
Lambda Function development and troubleshooting

DynamoDB table creation and data population

API Gateway endpoint creation and integration with Lambda

S3 Static Website Hosting

X-Ray Tracing for monitoring and troubleshooting

Lambda Layer integration for enhanced functionality

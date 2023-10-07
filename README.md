# AWS-CICD
AWS CodeCommit, CodeBuild, CodePipeline and Lambda functions to create a complete CI/CD pipeline

1. build the image first before tagging it. docker build -t node
2. Create a sample API using NodeJS.
3. Build a Docker image from the application and push it to ECR.
4. Use CodeCommit as a Git repository to store our code.
5. Define our build instructions in a CodeBuild project
6. Trigger the CodeBuild job automatically when code is pushed to the master branch using CodePipeline.
7. Write a simple test for our NodeJS app using Mocha.
8. Create a second CodeBuild project (QA) to apply our automated test.
9. Configure the CodeBuild QA project to be triggered when a Pull Request is created or modified using a Lambda function.
10. Provide fast feedback to the Pull Request creator by commenting on the PR with the test results using another Lambda function.
11. Implement Continuous Delivery (CD) by deploying an EC2 instance and configuring the CodeBuild project to deploy the Docker image to the instance and update the application using docker-compose.

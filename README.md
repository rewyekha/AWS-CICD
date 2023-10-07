# AWS-CICD
AWS CodeCommit, CodeBuild, CodePipeline and Lambda functions to create a complete CI/CD pipeline

1. Create a sample API using NodeJS.
2. Build a Docker image from the application and push it to ECR.
3. Use CodeCommit as a Git repository to store our code.
4. Define our build instructions in a CodeBuild project
5. Trigger the CodeBuild job automatically when code is pushed to the master branch using CodePipeline.
6. Write a simple test for our NodeJS app using Mocha.
7. Create a second CodeBuild project (QA) to apply our automated test.
8. Configure the CodeBuild QA project to be triggered when a Pull Request is created or modified using a Lambda function.
9. Provide fast feedback to the Pull Request creator by commenting on the PR with the test results using another Lambda function.
10. Implement Continuous Delivery (CD) by deploying an EC2 instance and configuring the CodeBuild project to deploy the Docker image to the instance and update the application using docker-compose.

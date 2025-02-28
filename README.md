# DevOps Project - Hybrid Continuous Delivery of Vprofile Project using AWS, Jenkins, Nexus, SonarQube and Slack

This is a DevOps project for _Hybrid Continuous Delivery_ of vprofile project using AWS, Jenkins, Nexus, SonarQube and Slack. This project is a continuation of [_vprofile-project-ci-jenkins_](https://github.com/durrezahmed/vprofile-project-ci-jenkins) project.

[Link](https://github.com/durrezahmed/vprofile-project-devops) for vprofile app repository.

## Prerequisites:

- [**Continuous Delivery with Jenkins and Tools**](https://github.com/durrezahmed/vprofile-project-cicd-jenkins)

- [**Continuous Delivery on AWS**](https://github.com/durrezahmed/vprofile-project-cicd-aws)

## About:

- Jenkins for CI (Continuous Integration)

- _PaaS_ and _SaaS_ Services of AWS

## Tools used in the Project:

- [**Amazon EC2**](https://aws.amazon.com/ec2/) - Compute Resource

- [**AWS Elastic Beanstalk**](https://aws.amazon.com/elasticbeanstalk/) - Artifact Deployment

- [**AWS CLI**](https://aws.amazon.com/cli/) - Deploying Artifact from Jenkins

- [**Amazon S3**](https://aws.amazon.com/s3/) - Upload Artifact

- [**Jenkins**](https://www.jenkins.io/) - Continuous Integration and Continuous Delivery Server

- [**Git and GitHub**](https://github.com/) - Version Control System

- [**Maven**](https://maven.apache.org/) - Build Tool

- [**Checkstyle**](https://checkstyle.org/) - Code Analysis Tool

- [**Nexus Sonatype Repository**](https://www.sonatype.com/products/nexus-repository) - Artifact / Software Repository

- [**SonarQube**](https://www.sonarsource.com/products/sonarqube/) - Code Analysis Server

- [**Slack**](https://slack.com/) - Notifications

## Usage (Flow of Execution):

1. Validate CI Pipeline

2. Install `AWS CLI` in Jenkins

3. AWS Services

   - Create an S3 Bucket

   - IAM user with Access Keys, Beanstalk Policy and S3 Policy

   - Create Beanstalk Application with name `vproapp`

4. `Jenkinsfile` in the Git Repository and Test the Pipeline

5. `Jenkinsfile` for Production

   - Create new Beanstalk Environment for Production

   - `Jenkinsfile` , Create a new Pipeline for Production
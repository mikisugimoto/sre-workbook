# SRE-workbook

Learning how to do SRE stuff!

## Modules

Each module is a small task representing a skill or technology

### Jenkins Server

**Objective**: Set up a Jenkins server to deploy code

**Definition of Done**:
- [ ] Provision infrastructure to run Jenkins server in cloud provider of choice
- [ ] Install and configure the Jenkins server using IaC (Terraform/Ansible recommended)
- [ ] Create an admin and a developer user in Jenkins
- [ ] Install an update on the server (not manually)
- [ ] Set up server for automatic backups
- [ ] Create a build agent which will build Docker containers

**Resources**:

Note: Resources may contain relevant information but not be a complete solution

- [Set up Jenkins server on AWS](https://aws.amazon.com/blogs/devops/setting-up-a-ci-cd-pipeline-by-integrating-jenkins-with-aws-codebuild-and-aws-codedeploy/)
- [Set up Jenkins server on Azure](https://docs.microsoft.com/en-us/azure/developer/jenkins/)

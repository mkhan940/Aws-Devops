### Aws-Devops
To deploy this infrastructure, visit the AWS Management Console, navigate to CloudFormation, and create a new stack.
## Overview of Infrastructure Components:

The provided CloudFormation template creates the following infrastructure components:

- **VPC (Virtual Private Cloud):**
Virtual Private Cloud with specified CIDR block.

- **ECS Cluster**:
Container cluster for running Docker containers.

- **ECR Repository**:
Docker container image repository for managing images.

- **RDS Instance**:
PostgreSQL RDS database instance.

- **EC2 Security Groups:**
Security groups for database and load balancer access.

- **Load Balancer:**
Internet-facing load balancer for distributing traffic.

- **CodeCommit Repository:**
Version-controlled repository for source code.

- **CodePipeline:**
CI/CD pipeline for build, test, and deployment.

- **CodeBuild Project:**
Build project for compiling and packaging source code.

- **CodeDeploy Application and Deployment Group:**
Application and deployment group for managing deployments.

- **IAM Roles:**
Roles for AWS services with necessary permissions.

- **S3 Bucket:**
S3 bucket used by CodePipeline for storing artifacts.

**Outputs:**
- **VpcId, PublicSubnetId, PrivateSubnetId:**
IDs of VPC and subnets.

- **RDSDatabaseEndpoint:**
Endpoint address of the RDS database.

- **LoadBalancerDNSName:**
DNS name of the load balancer.

- **CodeCommitRepositoryCloneUrlHttp:**

HTTP clone URL for accessing the CodeCommit repository.

# AWS DevOps Questions

1. About your self

- This tirumala total i have 5 years of experience in software(IT), it is more into cloud and devops i have
- Im started my career start with linux admin either its moved into cloud and devops.
- cloud i have worked aws and azure, devops i have worked in docker, Kubernetes, Jenkins, Terraform, Ansible most of the ci/cd tools i have worked

2. Can you explain your recent ci/cd pipeline configuration:

- HSBC is my clint we are supporting and we have the differnt ATM Networking backend applications we are managing, which are java spring boot microservices based applications we have
- and comming to my pipeline i have use the jenkins and we have the declarative pipeline and if the source code we have configure the webhook it automatically going to trigger when code commit happens than
- Maven is the build job we have static code analisys, unit testing all these all we integrating using junit and sonarqube, than we have artifactory after thac CD iam going to deploy into like terraform and containerized images, docker files than i go to scan those images push to the registory than deploy into AKS cluster.

3. If you need to migrate an application one aws reasion to another reasion how did you manage thise

- so one method we can use is AMI. We can convert. After that conversion, we can move to another region. We can switch. Otherwise we can use AWS migrate, kind of volume level we can migrate, and what about the database level we have see if you are

- yes in one reason to another reason. If you want to migrate data set at the database level, first I need to create a one more VPC I can create instead of replicating the VPC with the same side of. Block on another region, the same subnets, all these, I'm going to create in another region. I'm going to create for the VPC, whatever the methods we have, route tables, all these, I'm going to create after this, for the Server migration. I choose better to go to the amis, because we can copy those Amis into another region. And coming to the like a target groups, auto scaling all those also I'm going to replicate in the another region, because it's already have the same Ami. And I'm going to create a new load balancer, and I'm going to do the same load balancer rules. All these are going to configure. After this, I'm going to replicate the database using the DMS kind of operations. So using the database migration service, I'm going to migrate the data into another region with the schema level changes we can perform, or only the replication also we can perform, into another region we can perform. Then, if we have any s3 buckets. All these also are supported for the replications by default. In the s3 itself, we have the replicate options, or using the CLI, I can replicate those s3 because duplicate names are not possible with the s3 bucket at the multi account level. Also, as a result, I need to, I need to make sure, like, because once we create the bucket names, also leading those names also not so renaming this also is not possible in the AWS. So then the data migrations. Also, I need to take care. From the replication jobs, I need to take care. So these are the things I need to make sure I didn't have any Redis clusters on this. Also, we need to take care. And whenever we have lambda functions I need migrated. I have provision laws, or we can use any automation solution, also by importing all these resources in the TerraForm. And from that TerraForm where, also we can try to use another region. From that also we'll try to migrate.

4. In deployment pipeline, which is using Jenkins and TerraForm Okay, which is paying due to some permission issues when updating AWS resources in my production environment. How would you direct this and resolve this kind of problems?

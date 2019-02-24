### Cloud formation stack set
The goal of this project is to create a convenient template for deploying an environment for an application in Docker on ECS Cluster, with Bastion host (Jenkins instance with tools), RDS Instance (MySQL or Postgresql to choose from) and some aws tools for notifications and logging.

#### Content:
- stack-set file
- create-vpc file
- create-ecs cluster file

#### Requirements:
1) For start Stack Set operations you need grant permissions by this [manual](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs.html#stacksets-prereqs-accountsetup)
Or you can use two templates in the .init / directory (With caution and understanding of what you share);

2) Before start you need create Amazon EC2 key pairs for every instance, or instance type ([manual](https://docs.aws.amazon.com/servicecatalog/latest/adminguide/getstarted-keypair.html));

#### Possible problems and their solutions:
1) Q: ASG error: "Failed - Launching a new EC2 instance" 
   A: To do so please visit https://aws.amazon.com/marketplace/pp?sku=aw0evgkw8e5c1q413zgy5pjce. Then, Continue to Subscribe .
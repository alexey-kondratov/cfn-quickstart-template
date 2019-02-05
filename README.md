### Cloud formation stack set
#### Content:
- stack-set file
- create-vpc file

#### Requirements:
1) For start Stack Set operations you need grant permissions by this [manual](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs.html#stacksets-prereqs-accountsetup)
Or you can use two templates in the .init / directory (With caution and understanding of what you share);

2) Before start you need create Amazon EC2 key pairs for every instance, or instance type ([manual](https://docs.aws.amazon.com/servicecatalog/latest/adminguide/getstarted-keypair.html));
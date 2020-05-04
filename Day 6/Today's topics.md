# Topic for today

1. VPC in AWS.
2. Cloud watch.
3. Cloud trail. (CCTV)
4. User-data
5. More on Lambda

---

* ## VPC 

**What VPC contains**

AWS contains VPC contains subnets contains *route table*, *internet gateways*, *security groups*...

---

**What is VPC ?**

A virtual private cloud (VPC) is a virtual network dedicated to your AWS account. It is logically isolated from other virtual networks in the AWS Cloud. You can launch your AWS resources, such as Amazon EC2 instances, into your VPC. You can specify an IP address range for the VPC, add subnets, associate security groups, and configure route tables.

---
**What is subnet ?**

A subnet is a range of IP addresses in your VPC. You can launch AWS resources into a specified subnet. Use a public subnet for resources that must be connected to the internet, and a private subnet for resources that won't be connected to the internet. For more information about public and private subnets, see VPC and subnet basics.

We can select subnet in *configure instance details*

---

To protect the AWS resources in each subnet, you can use multiple layers of security, including security groups and network access control lists (ACL). For more information, see Internetwork traffic privacy in Amazon VPC.

*Note* : 1. Internet is not inside AWS, AWS connects to internet.
         2. We get IP address from CIDR block.
         3. VPC and subnets are given to us by our company, we need to make our *Security groups*.

---
---

* ## Cloud trail.

Every action that we perform on AWS UI is stored in Cloud trail. **It tracks user activity**, just like CCTV of VITA :p 
**Company me jana, toh jyada hushiyari mat marna - Pradeep Sir**

*Kachha chitta of you*

---
---

* ## Cloud watch

**It monitors resources and applications**
Eg: Trail monitors what EC-2 you created, Watch monitors the EC-2 you created.

*Kachha chitta of your resources*

---
---

* ## User Data

In case we want any application to download, we can add our commands at the time of creating an instance.

---
---

* ## Lambda

**Event driven automation**

We can configure event in S3. For eg: When someone puts a file in my S3, I can trigger Lambda at that time. 
Whenever I put a file in Bucket, lambda function can read that file and print its data.














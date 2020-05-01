
# How to Link 2 services on AWS
---

for eg: I want connect my EC2 with my S3.
By deafault it is not possible, so have to create IAM and lay down some Policies 
and then we have to attach this IAM to our EC2 and then we can use S3 in EC2.


Steps 
---
1) Make IAM with certain polices ( uses JSON ), We can also write our own. Policies are nothing but rules defined for EC2 which dictates how much
control it has over our S3

2) attach IAM to our EC2, go to instance, select Actions, Instance Settings -> attach/replace IAM role

3) to use S3 in our EC2(linux). go to mobaxterm and in our linux EC2 type ' aws s3 ls ' to get the folders present in our s3. In short
   in order to access S3 the syntax is ' aws s3 <command> '. 






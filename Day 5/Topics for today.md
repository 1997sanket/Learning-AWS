# Topics for today

## Contents ---
1. How to connect local PC to AWS service.
2. Why we use MySql service when we can just download MySql on our EC-2 ?
3. What is **Lambda function** in AWS.
---

## In detail
---
* **How to connect local PC to AWS service**
1. Download AWS CLI on your local PC.
2. Open *Windows* cmd promt (not AWS CLI cmd).
3. Now follow this, C:// -> Users -> YourUser -> .aws -> Credentials and delete everything from the editor.
4. Now go to your AWS workbench -> Account details, copy AWS CLI, go to Credentials againg and paste it.
5. Now go to Windows CMD and type your AWS commands. Eg: *aws s3 ls* to to list all the buckets in your S3.
 
---
**Note** : Your *access_key_id* and *secret_access* are VVI. Sogenerally, companies dont allow you to connect with local PCs.           These keys should never be leaked.

---
**Why we didnt use IAM role for our local PC ?**

---
1. IAM role doesnt work outside of AWS.
2. For local PC to connect with AWS, only secret key is the option. But for EC2 we can use both IAM role and secret key.
3. IAM role is better than secret key, one reason is security.

---
---
* **Why we use MySql service when we can just download MySql on our EC-2 ?**
1. MySql service in AWS is completely managed by AWS, whereas if we download MySql locally, it has be managed by us.
   It could be managable for a database with small amount of data, but with huge amount it would be very difficult to manage on our own.
   That is why it is better to give this burden to AWS :)
2. AWS is not responsible for malicious activity/virus that may occur due to us downloading apps on EC2, it may crash and we may lose 
   data, let AWS manage the service.
3. Multiple EC-2's can acces the MySql service by AWS whereas only one PC can access the downloaded database.
4. MySql service is scalable, and it is done automatically by AWS when data increases in size.

---
---
* **What is **Lambda function** in AWS.**
---
1. In EC-2 we are charged money while the instance is running. We can store our code and not run it, but it will cost us
   if the instance is running. We if run the code we are not using the *2 core* processor or *4GB RAM* we bought, it may merely
   use a fraction of that, but yet we pay the full price.
2. Here comes *Lambda function*, in this we store our code and AWS will not charge us a single penny. No matter how much amount of
   code we store, lakhs, crores, you name it. AWS will only charge us when we *actually* run the code. The charge is dependent on the
   amount of processor, ram... used for running the code. Just how delightful is this ??  **<3 Thank your AWS <3** .




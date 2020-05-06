# Topics for today

1. SNS (Simple notification service)
2. Creating Snapshot of a EC2 volume
3. Creating EC2 image
4. Uploading a programming language package on S3 so that we can use it in our Lambda function. ( No practical, since Java was not done)
5. More features of S3
   * Versions of bucket.
   * Can run queries on CSV, JSON, parquet files of a bucket.
   * Default encryption.
   * Object lock.
   * Requester pays.



---
* ## SNS

1. Just as the name says, it is a notification service. We need to select subcribers ( ones who will get our notifications), publisher  (any service in our AWS), and we need to create topic. We need to give access policy to everyone, and create an IAM role for publisher (service) to connect with the our SSN topic.

2. So suppose I select a S3 bucket as a publisher, then whenever I add anything in my bucket, I will get notification to the email
I set as a subscription.

---
---
* ## Creating Snapshot of a EC2 volume

1. In our EC2s we have volume( hardisk ). We can create snapshot of that volume if we want to delete our Virtual machine.
2. But this snapshot are formed in incremental order i.e If we create a snapshot of our volume, then a copy is made, but then if 
   we add/modify in our EC2 volume and again take a snapshot then the new snapshot will have the newly modified information only and not
   the entire information.

---
---

* ## Creating EC2 image

1. We can create an image of our EC2.
2. It is nothing but a custom AMI (Amazon machine image) (OS), which we can select at the time of creation of an EC2.

---
---

* ## More features of S3

* Versions of bucket

For critical data like for eg transaction details or order details of our E-commerce website we can store different versions of our bucket, by using *Versioning* feature of S3. It's similar to version control of Git. We can see past data through the version feature.



* Can run queries on CSV, JSON, parquet files of a bucket

Just as the title suggests, we can run queries on some of the files in S3. It's a very useful feature - *Pradeep Sir*



* Default encryption

If you upload a copyrighted file on Google drive, google deletes the data and sends you the message. But who is Google to know what you
have uploaded ? How can google access your personal data ? So AWS is much more professional in this regards, they give you encryption 
option in S3 by which your data remains untouchable.

It's a very frequently used feature in the Industry.



* Object Lock

If you dont want ANY data in your S3 to be deleted, you can enable **Object lock** at the time of creating a bucket.
This way your *sensitive* data cannot be delete even by mistake.



* Requester pays

Any one who is downloading/uploading/requesting data of your bucket, that person will pay for the AWS bills.
Eg: Suppose i've made multiple buckets for my multiple clients, I can enable the *Requester pays* option so that the AWS bill directly 
goes to that particular client.






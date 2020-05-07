# Topic for today

1. CFT (CloudFormation template)

2. Deploying a very basic website on AWS (no pratical)

3. TASK
   



---

* ## What is CFT

1. As the name suggests, it is a service provided by the AWS in order to make multiple resoures at the same time.
   It takes less time to create all the resources using CFT.It uses JSON to create the resources. Sample templates are provided by the AWS. 

2. Advantage of using CFT is, suppose I make multiple resources in my CFT eg: EC-2, Lambda, S3, Snapshot, RDBMS, IAM role,
   then I dont have to remember to delete each of the resources individually, I can delete all at one go by deleting the
   CFT itself. 

3. We can even update resources in our CFT. We cannot delete a particular resource from CFT.

4. CFT is completely free, only the resources we create will charge.


**NOTE** : If you made 50 EC2's using CFT and then you go to UI and manually delete 2 EC2's, then at the time of deleting your CFT,
           your CFT deletion process will give error saying "I made 50 EC2s, 2 of them are missing; cannot delete the CFT".
           'So aise keede kand mat karna' - *Pradeep Sir*

---
---

* ## Deploying a very basic website on AWS 

1. Sir created a windows EC2 on aws, installed JDK and TomCat, created a .var file, uploaded it in TomCat's *WebApps* folder.

2. He then edited EC2's inbound rule and added 8080 port (TomCat's port number), and in inside his EC2 (windows) he edited Firewall
   inbound rule and added 8080 port.

3. By doing this, the server which was originally created inside EC2, was now accessible in Sir's local PC (mac).

4. He just put in the browser url box, **localhost:8080/dac** (dac is the folder created when we add the var file in *WebApps* and 
   run the TomCat)




## How to run TomCat

1. Install JDK, install TomCat

2. Go to TomCat folder --> bin --> Run *startup.bat* file.

3. If there is an error saying `JAVA_HOME` not defined, then goto Windows variables -> Environment variables -> add `JAVA_HOME' and 
   in the value copy_paste your JDK folder location.

4. Shut down and restart your PC and then run the TomCat again. Your server is hopefully ready :D

---
---

* ## Task

1. In your local PC, Install *Slack* application, create a channel.

2. When you type in `create linux ec2` a new basic linux ec2 should be made in your AWS, similary EC2 should get deleted when you type
   `delete ec2 <id of EC2>` , same for **starting** and **stoping** your EC2.

3. This message will go from your local PC's  Slack's  channel to your *Lambda* of AWS and will create the EC2.

4. Slack/Telegram has **Web Hooks** through which you can talk to *Lambda*.

5. Below is the explaination shown by Pradeep Sir.

<img src= "images/Day 8 miniproject explained by Sir.png">


**SIDE NOTE** 

*Why is this useful ??*

Suppose you are in a lec which is about to be finished in 10 mins, so you just type in your mobile `start ec2 <id>` and thus 
by the time you reach your Labs, your EC2 is running, tada....













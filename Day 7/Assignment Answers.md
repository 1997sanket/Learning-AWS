# Assignment

## 1. Send notification to your email when CPU utilisation is <= 50%

Steps:

* Go to your EC2 -> Monitoring -> create alarm -> choose CPU utilisation and other desired setting -> Create a topic if you havent already -> While creation of topic make sure to give IAM role (For success and failure).

**NOTE:** Subscriber = Person who will receive the notification,
          Publisher  = Service which is attached to Topic created which will then send the notification.
          Topic      = SNS topic is like a medium between the two.


I have upload the G-mail image of the notification, in the same folder where I received when my CPU utilisation was <= 50 percent. 

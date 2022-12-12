# E-Wallet-Backend
This is Digital wallet project which transacts money from one user's wallet to another and simultaneously sends email notifications to the respective users

# Different Services In Project :
1. User Services
2. Wallet Services
3. Transaction Services
4. Email Services

# How Project Works
1. All communications bewtween differnt service layers of the project happens with the help of kafka.
2. To fetch the information quickly, I have used redis so that it can fetch fro cache.
3. When a User is created from User Services Layer -> It calls for Wallet Services to Create its Wallet
4. When a User Wants to transact money -> Transaction services calls for wallet update.
5. Now wallet again send information to the transaction services about updation of the trasaction.
6. When transaction become complete, It calls for Email service to send the emails for Sender and Receiver.


# Teck Stack Used :
1. Spring-Boot
2. Redis 
3. Kafka
4. MySQL
5. OOPs Concepts
6. Java

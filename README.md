# Deploy a Simple Web Application

In this guide I will show you how to deploy a web  application using AWS cloud step by step. Let's get started !

# Step 1 : Login to AWS 

- Open AWS cloud console. Login to console using credential
- Launch an EC2 instance
- Select an appropriate amazon machine (AMI)
- Instance type (e.g. t2 micro for free tier)
- Configure security groups to allow HTTP (port 80) SSH (port 22)
  
![1](https://github.com/user-attachments/assets/246906fd-a91c-47b6-9a9a-532b83144b65)

![2](https://github.com/user-attachments/assets/819d73a6-0377-4293-804e-a47991bdce3b)

![3](https://github.com/user-attachments/assets/5a5361b0-bb76-4099-8ca4-ac5e710e1057)

# step 2 : SSH into Instance

Once the instances is running, click on connect aws CLI and run the command
` ` ` bash
 sudo su -
` ` `

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
``` git
 sudo su -
```
``` git
 yum update -y
```

![4](https://github.com/user-attachments/assets/ded460db-c244-4461-9c5b-5044b96c879d)

# step 3 : Install httpd
``` git
 yum install httpd
```

![5](https://github.com/user-attachments/assets/b37f8973-e0ed-46a3-b9d6-e964476019bb)

# step 4 : Check status of httpd
``` git
  systemctl status httpd
```
![14](https://github.com/user-attachments/assets/48300c92-2f3d-4444-b56a-3636f4ab6ad8)

# step 5 : Create directory 
``` git
mkdir test
```

![6](https://github.com/user-attachments/assets/2361de79-607f-4183-8ad4-2c1801e66ea1)

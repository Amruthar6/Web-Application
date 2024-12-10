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

![6](https://github.com/user-attachments/assets/375b9a82-088f-41e6-9b08-95a8af14a7b1)

# step 6 : Clone the Application code from Github
``` git
wget https://github.com/Amruthar6/Web-Application/archive/refs/heads/main.zip
```

![7](https://github.com/user-attachments/assets/60157923-6985-4988-bb7b-1ed77938d69b)

# step 7 : Unzip the main zip file
``` git
unzip main.zip
```
``` git
 ls -l
```

![8](https://github.com/user-attachments/assets/2d8c41ee-5514-46ce-a31a-4659f6208049)

# step 8 : Check httpd status again if not started run the enable command
``` git 
systemctl status httpd
```
``` git
systemctl enable httpd
```

![9](https://github.com/user-attachments/assets/df1943f6-a226-421a-9048-d41f12395abb)

# step 9 : Run the application using Public Ip  
e.g.
http://3.83.129.16/

![10](https://github.com/user-attachments/assets/ec4a0460-0d58-4677-ab95-142788b7a6b5)
![11](https://github.com/user-attachments/assets/38839e11-ca5d-4c81-a66f-273871d46805)
![12](https://github.com/user-attachments/assets/e379c51a-d1ee-4297-a242-9fbed3c61257)
![13](https://github.com/user-attachments/assets/79ea34a9-410c-4cec-87d5-d2f8f87b4c7d)



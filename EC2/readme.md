
# EC2- Elastic Compute Cloud

### Instance Types:
1. General Purpose  ( t series )
2. Compute optimized ( c series )
3. Memory Optimized ( r series )
4. Storage Optimized ( i series )
5. Accelerated Computing ( p series )


### Purchasing Options:
1. On Demand
2. Reserved
3. Dedicated Host
4. Spot Instance

### Steps To Launch EC2 Instance:
- Launch an instance 
- Application and OS Images (Amazon Machine Image) 
![image](https://github.com/user-attachments/assets/6142ef7d-818b-45ce-b7ab-169c646e065a)

- Instance type 
- Key pair (login) 
- Network settings 
![image](https://github.com/user-attachments/assets/e2aaed6c-c4ee-4a8e-82b7-ebc6d2fb4b83)

- Configure storage
- Launch Instance

### Ec2 status check
- 2/2 --> Instance is Healthy/All Okay
- 1/2 --> Software Issue
- 0/2 --> Hardware Issue
### Nginx Installation Script for Amazon Linux
```bash
sudo -i
yum update -y
yum install nginx -y
systemctl start nginx
systemctl enable nginx
systemctl status nginx
curl localhost
```


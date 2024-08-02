## AMI - Amazon Machine Image
# AWS <span style="color:orange;">AMI</span> Setup Guide
- Amazon Machine Images (AMIs) are templates that contain the software configuration
- (operating system, application server, and applications) required to launch an instance on AWS.

## Benefits of Using AMIs

1. **Consistency**: Ensures new instances are identical to the original, reducing configuration errors
2. **Scalability**: Easily launch multiple instances from the same AMI to handle increased traffic
3. **Backup and Recovery**: Use AMIs as backups for your instances; in case of failure, launch a new instance from the AMI
4. **Customization**: Tailor AMIs to specific application needs, including pre-installed software and configurations

  ### Create an AMI from the Instance

1. **Launch an EC2 instance** with Amazon Linux 
2. **Connect to the instance** using SSH
3. **Install Apache**:
    ```sh
    sudo yum update -y
    sudo yum install httpd -y
    sudo systemctl start httpd
    sudo systemctl enable httpd
    ```

1. **Stop the Instance**
    
2. **Create Image**
    - Go to the EC2 Dashboard, select instance -> click on Actions -> Image and Template and select "Create Image"
      
    ![image](https://github.com/user-attachments/assets/13e61c02-a1db-4ef5-91d4-422c906db9f5)

    - Provide a name and description for the image
    - Specify the volumes to include in the image
    - Click "Create Image"



### Launch a New Instance from the AMI

1. **Find the AMI**
    - Go to the "AMIs" section in the EC2 Dashboard
      ![image](https://github.com/user-attachments/assets/b013baec-cdb2-4673-9db9-78047cb77135)
      
2. **Launch Instance**
    - Select your AMI and click "Launch"
    - Follow the steps to configure and launch the new instance
3. **Launch a new instance** from the created AMI to ensure Apache is pre-installed and running












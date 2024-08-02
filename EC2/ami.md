## AMI - Amazon Machine Image
- Amazon Machine Images (AMIs) are templates that contain the software configuration
- (operating system, application server, and applications) required to launch an instance on AWS.

  ### Create an AMI from the Instance

1. **Stop the Instance**
    - It’s recommended to stop the instance before creating an AMI to ensure data consistency
2. **Create Image**
    - Go to the EC2 Dashboard, right-click the instance, and select "Create Image"
    - Provide a name and description for the image
    - Specify the volumes to include in the image
    - Click "Create Image"

## Using the AMI

### Launch a New Instance from the AMI

1. **Find the AMI**
    - Go to the "AMIs" section in the EC2 Dashboard
2. **Launch Instance**
    - Select your AMI and click "Launch"
    - Follow the steps to configure and launch the new instance

## Optional: Share or Copy the AMI

### Share an AMI

1. **Select the AMI**, click "Actions", and choose "Modify Image Permissions"
2. **Add the AWS account IDs** you want to share with

### Copy an AMI

1. **Select the AMI**, click "Actions", and choose "Copy AMI"
2. **Select the destination region** and provide a name

## Benefits of Using AMIs

1. **Consistency**: Ensures new instances are identical to the original, reducing configuration errors
2. **Scalability**: Easily launch multiple instances from the same AMI to handle increased traffic
3. **Backup and Recovery**: Use AMIs as backups for your instances; in case of failure, launch a new instance from the AMI
4. **Customization**: Tailor AMIs to specific application needs, including pre-installed software and configurations

## Example Scenario

1. **Launch an EC2 instance** with Amazon Linux 2
2. **Connect to the instance** using SSH
3. **Install Apache**:
    ```sh
    sudo yum update -y
    sudo yum install httpd -y
    sudo systemctl start httpd
    sudo systemctl enable httpd
    ```
4. **Create an AMI** from the customized instance
5. **Launch a new instance** from the created AMI to ensure Apache is pre-installed and running

![image](https://github.com/user-attachments/assets/02a2afd1-e1ee-4b75-9f47-fda0147f2fa7)

![image](https://github.com/user-attachments/assets/13e61c02-a1db-4ef5-91d4-422c906db9f5)

![image](https://github.com/user-attachments/assets/b013baec-cdb2-4673-9db9-78047cb77135)

![image](https://github.com/user-attachments/assets/780605e2-e4af-4c46-ac81-c0f57ff94e12)




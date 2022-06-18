# Deploy-a-High-Availability-Web-App-Using-CloudFormation

## Author
Nyashadzashe Ndhlovu, Cloud DevOps Udacity Student

## Outputs
 I have used the intrinsic function `!Join` to achieve a URL with the Load Balancer DNS Name and “http” in front of it . 

![url output](./Docs/http%20DNS%20output.PNG)

 My output successfully redirected to a “it works! Udagram, Udacity” page as requested. ![url output](./Docs/it%20works!%20udagram%2C%20Udacity.PNG)

## Design Considerations :

I made use of the [AWS SSM Session Manager](https://aws.amazon.com/blogs/mt/replacing-a-bastion-host-with-amazon-ec2-systems-manager/) to provide access to the web application servers.

The reason why i chose this instead of the bastion is because the Bastion;<br>
- Like any other infrastructure host, it must be managed and patched.<br>
- It accrues a cost while it is running.
 
 While the AWS SSM Session Manager reduces your system’s attack surface while also offering greater visibility into commands issued on your hosts. 


## Docs
This folder has some screenshots of the progress of the project during the course of deployment
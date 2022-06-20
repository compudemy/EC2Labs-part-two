# EC2Labs-part-two

An EC2 instance can be launched in multiple ways such as using a console which is a basic method used, another way is using CLI commands, either using Lambda (API function) and one more way is using an Infrastructure as Code service i.e. Cloudformation service.

Your EC2 instance can be of two types one being a Public instance and another is a Private instance.

A Public instance is one which is having public IP and is reachable from outside your network whereas, a Private instance will have only private IP and cannot be reached from outside of your defined network. When you stop and start a public instance its IP address will be changed and in a private instance, its IP remains the same.

Below are the steps to launch an Amazon Linux EC2 machine using the console.
Login to console and choose EC2 wizard and click on launch instance. Here, we are choosing Amazon Linux 2 AMI.
An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch your instance. You can select an AMI provided by AWS, user community, or the AWS Marketplace; or you can select one of your own AMIs.

![image](https://user-images.githubusercontent.com/103466963/174646505-2cd3db3e-aab1-48b7-b56e-a5822beb5433.png)

2. Choose the required instance type (instance types are discussed in our other article). Here, we are choosing t2.micro general purpose instance as it is available in the free tier.

![image](https://user-images.githubusercontent.com/103466963/174646691-47ce1f00-5407-4a53-9733-ca7c8e61c06f.png)

3. This step allows you to configure your instance details such as VPC, Subnet, Public IP, IAM role and few other pre defined parameters. Here, we are launching 1 t2.micro instance into default VPC and Public Subnet. (We will be discussing in details regarding VPC in our coming blogs).


4. In this step we will choose required storage capacity as well type of volumes. In general Linux machine’s Root volume will be “/dev/xvda” and for Windows it will be “/dev/sda”. We can add additional storage if required as well as encryption for the data.

![image](https://user-images.githubusercontent.com/103466963/174649820-dec83986-2fda-47b7-a4be-1b52b214a7c8.png)


5. Add Tags as per the standards followed. A tag consists of a case-sensitive key-value pair. These are very useful when you are defining any API function based on Tags.
![image](https://user-images.githubusercontent.com/103466963/174649652-f50528f6-2d36-45cb-9bf7-6a5386a1eaf2.png)


6. A security group is a set of firewall rules that control the traffic for your instance. On this page, you can add rules to allow specific traffic to reach your instance. You can choose existing Security Group or can define your own. We are going with default here as port 22 is allowed from internet and this is sufficient for connecting to this machine.

![image](https://user-images.githubusercontent.com/103466963/174649752-258856bc-6c0d-47c3-805c-abe1d6fada5f.png)







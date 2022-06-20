# EC2Labs-part-two

An EC2 instance can be launched in multiple ways such as using a console which is a basic method used, another way is using CLI commands, either using Lambda (API function) and one more way is using an Infrastructure as Code service i.e. Cloudformation service.

Your EC2 instance can be of two types one being a Public instance and another is a Private instance.

A Public instance is one which is having public IP and is reachable from outside your network whereas, a Private instance will have only private IP and cannot be reached from outside of your defined network. When you stop and start a public instance its IP address will be changed and in a private instance, its IP remains the same.

Below are the steps to launch an Amazon Linux EC2 machine using the console.
Login to console and choose EC2 wizard and click on launch instance. Here, we are choosing Amazon Linux 2 AMI.
An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch your instance. You can select an AMI provided by AWS, user community, or the AWS Marketplace; or you can select one of your own AMIs.

https://miro.medium.com/max/1400/1*M4s1n5_U2-mZONV9JSspRw.jpeg

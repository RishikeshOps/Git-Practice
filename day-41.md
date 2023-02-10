# Day 41 AWS EC2 Automation - Load Balancing with ELB ☁

![LB2](https://user-images.githubusercontent.com/115981550/218145297-d55fe812-32b7-4242-a4f8-eb66312caa2c.png)

### Hi, I hope you had a great day yesterday learning about the launch template and instances in EC2. Today, we are going to dive into one of the most important concepts in EC2: Load Balancing.

## What is Load Balancing?
Load balancing is the distribution of workloads across multiple servers to ensure consistent and optimal resource utilization. It is an essential aspect of any large-scale and scalable computing system, as it helps you to improve the reliability and performance of your applications.

## Elastic Load Balancing:
**Elastic Load Balancing (ELB)** is a service provided by Amazon Web Services (AWS) that automatically distributes incoming traffic across multiple EC2 instances. ELB provides three types of load balancers:

Read more from [here](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/what-is-load-balancing.html)

1) **Application Load Balancer (ALB)** - _operates at layer 7 of the OSI model and is ideal for applications that require advanced routing and microservices._

- Read more from [here](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html)


2) **Network Load Balancer (NLB)** - _operates at layer 4 of the OSI model and is ideal for applications that require high throughput and low latency._

- Read more from [here](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/introduction.html)


3) **Classic Load Balancer (CLB)** - _operates at layer 4 of the OSI model and is ideal for applications that require basic load balancing features._
- Read more [here](https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/introduction.html)

## Task:
![LoadBalancer](https://user-images.githubusercontent.com/115981550/218143557-26ec33ce-99a7-4db6-a46f-1cf48ed77ae0.png)
- Create an Application Load Balancer (ALB) in EC2 using the AWS Management Console.
- Add two EC2 instances to the ALB as target groups.
- Verify that the ALB is working properly by checking the health status of the target instances and testing the load balancing capabilities.

 Read more about ELB [here](https://rushikesh-mashidkar.hashnode.dev/create-an-application-load-balancer-elastic-load-balancing-using-aws-ec2-instance).

Don't forget to share your progress on LinkedIn.

Happy Learning! :)

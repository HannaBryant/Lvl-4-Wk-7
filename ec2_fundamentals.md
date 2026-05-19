---Theoretical Analysis---

1.) Explain why Amazon EC2 stands for "Elastic Compute Cloud." What does the word elastic specifically refer to in cloud architecture? EC2 stands for "Elastic Compute Cloud" because it delivers flexible, on demand virtual computing power. Elastic refers to its ability to scale and compute resources up or down on demand.

2.) Name and describe the four essential infrastructure features provided by EC2 that classify it as Infrastructure as a Service (IaaS).
     --) It provides virtual machines, which are the EC2 instances. A computer running virtually inside of a data center than physically on a desk.

    --) It stores data on virtual storage units (EBS - Elastic Block Store) where you can choose the type of disk, SSD or HDD.

    --) It distributes the load across machines using Elastic Load Balancer (ELB). Load balances between multiple instances to use resources efficiently.

    --) It enables service scaling, this allows your infrastructure to grow or shrink automatically based on traffic. It optimizes cost while maintaining performance.


3.) Detail the billing model used by EC2. What happens to your costs when you scale down or shut down instances when demand decreases? Amazon EC2 uses a pay as you go billing model which means you only pay for the computing resources being used. When demand decreases, the costs will go down if you reduce the number or size of instances and/terminate instances. When you delete an instance, you stop paying the cost for that instance entirely.


--- Bootstrapping Design (User Data)---

1.) What is the process of bundling configuration commands into a script called? Bootstrapping, also called "User Data".


2.) Under which specific user profile are User Data scripts executed? Can only be executed by the root user of the instance.


3.) How many times does a User Data script run during the lifecycle of an EC2 instance? They only run once during the first boot of the instance and arent executed again during the lifecycle of the instance.
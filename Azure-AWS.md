# Azure - AWS


```
Azure Functions and AWS Lambda are both serverless computing services that allow you to run code without managing the underlying infrastructure. However,
they are part of different cloud platforms (Microsoft Azure and Amazon Web Services, respectively) and have some differences in terms of features,
integrations, and pricing. Here's a comparison between Azure Functions and AWS Lambda:
```

|Service | Description | AWS                      | Azure                      |
|-------|--------- |------------------------------- | --------------------------------------------- |
|Virtual servers|  Allows users to deploy, manage, and maintain OS and server software; instance types provide configurations of CPU/RAM | Virtual Machine  | Elastic Compute Cloud EC2 |
|Container management| Supports Docker/Kubernetes containers and allows users to run applications on managed instance clusters | EC2 Container Service (ECS) EC2 Container Service Kubernetes (EKS | Container service Azure Container service, AKS |
| | Allows customers to store Docker formatted images. Used to create all types of container deployments on Azure. | EC2 Container Registry | Azure Container Registry |
|| Allows customers to spin up container instances at will without any additional installation of underlying infrastructure or hosts | Fargate  | Container Instance |
|Backedn Process Logic | Integrates systems and runs backend processes in response to events or schedules without provisioning or managing servers. | lambda | Azure Functions, Event Grid |
|Microservice-based applications | Orchestrates and manages the execution, lifetime, and resilience of complex, interrelated code components that can be either stateless or stateful | - | Service fabric |
| Job orchestration | When processing across hundreds or thousands of compute nodes, this tool orchestrates the tasks and interactions between compute resources that are necessary | Batch | Batch |
| Scalability| Automatically changes the number of instances providing a compute workload. Users set defined metrics and thresholds that determine if the platform adds or removes instances. | Auto Scaling  | Virtual Machine scale sets, App Service Scala Capability, AutoScaling |
| Pre-defined templates | Community-led templates for creating and deploying virtual machine-based solutions. | Quick Start | QuickStart Templates and Blue prints |
| Time Sync |  Enables customers to access time servers from within the cloud network| Time Sync Service | - |
| Object storage | Object storage service for use cases including cloud apps, content distribution, backup, archiving, disaster recovery, and big data analytics | Simple Storage Services S3    | Storage  |
| Virtual Server disk infrastructure| SSD storage optimized for I/O intensive read/write operations| Elastic Block Store (EBS) | DIst Storage-(page blobs for VHDS other random write type data) Dist srorage, Premium Storage |
|| | | |
|| | | |
|| | | |
|| | | |
|| | | |
|| | | |
|| | | |
|| | | |

|||Azure Functions: Supports multiple programming languages including C#, F#, Node.js, Python, PowerShell, Java, and more.  | AWS Lambda: Supports languages such as Node.js, Python, Java, Ruby, Go, .NET Core, and custom runtimes using the Runtime API. |
||| Azure Functions: Integrates well with other Azure services and provides seamless connectivity with Azure Logic Apps, Event Grid, and other Azure components.  | AWS Lambda: Integrates with various AWS services like Amazon S3, DynamoDB, API Gateway, and more. It also allows custom integrations with other AWS services. |
||| Azure Functions: Supports a variety of triggers, including HTTP triggers, timer triggers, message-based triggers using Azure Service Bus, Azure Event Hubs, and more | AWS Lambda: Triggers can be events from different AWS services, such as changes in an S3 bucket, updates to DynamoDB tables, or API Gateway invocations |
|||Provides the option of running functions in a dedicated App Service plan or a consumption plan where resources are allocated dynamically based on demand  | Automatically scales based on the number of incoming requests, and you pay only for the compute time consumed |
||| Generally has a slightly higher cold start time compared to AWS Lambda | Known for its fast cold start times, making it suitable for scenarios where low latency is crucial. |
||| Pricing is based on execution time and resource consumption | Pricing is based on the number of requests and the compute time required to run the code |
||| Growing ecosystem and community with strong integration into Microsoft technologies. |  Mature ecosystem with extensive community support and integration with a wide range of AWS services |


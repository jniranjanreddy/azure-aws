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
| Shared file storage | A simple interface to create and configure file systems quickly as well as share common files. | Elastic File System | Files  |
| Archiving—cool storage | A lower cost tier for storing data that is infrequently accessed and long-lived | S3 IA Glacier | Storage-Hot, Cool A Archive Tier |
| Backup | Backup and archival solutions that allow files and folders to be backed-up and recovered from the cloud, and provide off-site protection against data loss. | - | Back Up |
| Hybrid storage | Integrates on-premises IT environments with cloud storage. Automates data management and storage, plus supports disaster recovery | Storage gateway  |  StorSimple |
| Bulk data transfer |  A data transport solution that uses secure disks and appliances to transfer substantial amounts of data. | Import/Export Disk | Import/Export |
| | Petabyte- to Exabyte-scale data transport solution | Import/Export Snowball, Snowball Edge, Snowmobile | DataBox |
| Disaster recovery | Automates protection and replication of virtual machines with health monitoring, recovery plans, and recovery plan testing.| - | Site Recovery |
| Cloud virtual networking | Provides an isolated, private environment in the cloud. | Virtual Private Cloud | Virtual Network |
| Cross-premises connectivity  | Connects Azure virtual networks to other Azure virtual networks or customer on-premises networks. It also supports VPN tunneling. | VPN Gateway | VPN Gateway |
| Domain name system management | Manage DNS records using the same credentials, billing, and support contract as other Azure services. |  Route 53 | DNS |
|  | Service that hosts domain names, routes users to Internet applications, manages traffic to apps, and improves app availability with automatic failover. | Route 53 | Traffic manager |
| Content delivery network |  Global content delivery network that transfers audio, video, applications, images, and other files. | CloudFront  | FrontDoor |
| Dedicated network | Establishes a dedicated, private network connection from a location to the cloud provider. | Direct Connect  | Express Route |
| Load balancing  | Automatically distributes incoming application traffic to add scale, handle failover, and route to a collection of resources. | Elastic Load Balancing | Load Balancer, Application Gateway |
| Relational database | SQL Database is a high-performance, reliable, and secure database you can use to build data-driven applications and websites, without needing to manage infrastructure. | RDS | SQL Database Including PostgreSQL, MySQl and MariaDB |
| NoSQL—document storage |  A globally-distributed, multi-model database that natively supports multiple data models: key-value, documents, graphs, and columnar| DynamoDB, Neptune  | Cosmos DB |
| NoSQL—key/value storage | A non-relational data store for semi-structured data. | DynamoDB and SimpleDB | table Storage  |
| Caching |  An in-memory–based, distributed-caching service thatprovides a high-performance store typically used to offload non-transactional work from a database. | ElastiCache | Redis cache |
|Database migration | Focuses on migration of database schema and data from one database format to a specific database technology in the cloud. | Database Migration Service | database Migration Service, Data Migration Assistant |
| Elastic data warehouse |  A fully managed data warehouse that analyzes data using business intelligence tools. | Redshift | SQL Data WareHouse|
| Big data processing | Supports technologies that break up large data processing tasks into multiple jobs, and then combine the results to enable massive parallelism. | Elastic MapReduce (EMR)  | HDinsight |
| Data orchestration | Processes and moves data between different compute and storage services, as well as on-premises data sources at specified intervals. | Data Pipeline | Data Factory |
| | Cloud-based ETL/data integration service that orchestrates and automates the movement and transformation of data from various sources | Glue Data Catalog | Data factory + Data catalog |
| Analytics  | Storage and analysis platforms that create insights from massive quantities of data, or data that originates from many sources. | Kinesis Analytics | Stream Analytics, Data Lake Analytics, Data Lake Store |
|Streaming data  | Storage and analysis platforms that create insights from massive quantities of data, or data that originates from many sources | Kinesis Streams,   Kinesis Firehose | Event Hubs, Events hub capture|
|Visualization | Business intelligence tools that build visualizations, perform ad-hoc analysis, and develop business insights from data. | QuickSight | Power BI |
| | Allows visualization and data analysis tools to be embedded in applications. | | Power BI Embedded |
| Search  | A scalable search server based on Apache Lucene. | Elasticsearch Service  | Market place Elastic Search |
| | Delivers full-text search and related search analytics and capabilities. | CloudSearch | search |
| Machine learning | Produces an end-to-end workflow to create, process, refine, and publish predictive models from complex data sets. | Machine Learning, Sage maker | machine learning Studio, machine learning Workbench |
| Data discovery |  Provides the ability to better register, enrich, discover, understand, and consume data sources. | | data catalog |
| | A serverless interactive query service that uses standard SQL for analyzing databases. | Athena  | Data lake Analytics|
| Conversational user interfaces virtual personal assistant | Suite that covers intelligence cognitive services, machine learning, analytics and more. | Alex Skills Kit | Cortona Intelligence Suite- Cortona Integration |
| | Builds and connects intelligent bots that interact with users via text messaging, Skype, Teams,  | Lex | Micro service Bot Framework, Bot service |
| Text to Speech  | Enables speech-to-text.  | polly  | Bing Speech API |
| Speech to Text | Enables converting speech to text. | Transcribe |  Bing Speech API |
| Text translation | Enables language translation automation | Translate |  Translator Text API + Emotions API|
| Text analysis | Capabilities such as key phrases, languages and sentiment Analysis  | Comprehend | Text Analytics API |
| Visual recognition | Distills actionable information from images, generates captions, and identifies objects in images | Rekognition |  The Computer Visions API + face API|
| | Detects, identifies, analyzes, organizes, and tags faces in photos. | |  Face API |
| Recognizes emotions in images. | | | Emotions API |
| | Intelligent video processing which produces stable video output, detects motion, creates intelligent thumbnails, detects and tracks faces. | Rekognition Video |  Media Analytics and Video indexer|
| | Allows developers to take advantage of machine learning models already deployed to the device. | DeepLens | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |


|||Azure Functions: Supports multiple programming languages including C#, F#, Node.js, Python, PowerShell, Java, and more.  | AWS Lambda: Supports languages such as Node.js, Python, Java, Ruby, Go, .NET Core, and custom runtimes using the Runtime API. |
||| Azure Functions: Integrates well with other Azure services and provides seamless connectivity with Azure Logic Apps, Event Grid, and other Azure components.  | AWS Lambda: Integrates with various AWS services like Amazon S3, DynamoDB, API Gateway, and more. It also allows custom integrations with other AWS services. |
||| Azure Functions: Supports a variety of triggers, including HTTP triggers, timer triggers, message-based triggers using Azure Service Bus, Azure Event Hubs, and more | AWS Lambda: Triggers can be events from different AWS services, such as changes in an S3 bucket, updates to DynamoDB tables, or API Gateway invocations |
|||Provides the option of running functions in a dedicated App Service plan or a consumption plan where resources are allocated dynamically based on demand  | Automatically scales based on the number of incoming requests, and you pay only for the compute time consumed |
||| Generally has a slightly higher cold start time compared to AWS Lambda | Known for its fast cold start times, making it suitable for scenarios where low latency is crucial. |
||| Pricing is based on execution time and resource consumption | Pricing is based on the number of requests and the compute time required to run the code |
||| Growing ecosystem and community with strong integration into Microsoft technologies. |  Mature ecosystem with extensive community support and integration with a wide range of AWS services |


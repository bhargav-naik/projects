
#### ML workflow orchestration : Project aims to orchestrate the complete lifecycle of collecting labeled data to re-training machine learning models 
- Responsible for requirements gathering, high level design, low level design
- Leading development effort and integration with other systems
- Planning of release milestones and onboarding first machine learning model

#### Disable "Cash On delivery" payment option : Aim of this project was to identify the fraudulent users to disable "Cash On delivery" payment option on orders.
- Collaboration with the data science team to understand feature definition
- Generation of one time feature dump for training the machine learning models
- Developed batch pipeline to import data, generate required features, ingest in cache

#### Returns fraud detection : Aim of this project was to automate the manual process of detecting the fraudulent users who created refund claims on orders
- Collaboration with the operations team to understand the Standard Operating Procedure (SOP) for fraud detection
- Feature engineering to generate features needed for rule evaluation
- Designed, developed and deployed a configurable rule based system which identifies/rejects fraud refund claims
- 20K refund_request/day are evaluated by the system eliminating manual intervention

#### Ratings reviews fraud detection : Aim of this project was to weed out fake accounts/reviews/ratings created by seller who up-voted their own product and dinged the competitor to get better sales
- Collaboration with data Scientist to understand the algorithm for detecting cluster of user who upVoted product of one seller and downVoted products of competitor
- Development of clustering approach using Hive queries and Spark GraphX
- Presented the solution in Flipkart Spotlight Event

#### Pricing abuse detection : Aim of the project was to identify and blacklist the fake products which had hiked up maximum retail price (mrp) and lucrative discounts to dupe the customers
- Collaboration with the product and analytics team to understand the problem
- Proposed a solution with rules at different granularity in hierarchy of product taxonomy
- Designed and developed a rule based framework where analytics team can configure new rules and modify existing threshold
- Debian packaging, Jenkins pipeline for build and deployment on production server

#### SPF fraud detection : Aim of this project was to identify the sellers which were abusing the system and gaining a large amount of seller protection fund by submitting documents/images for same broken product.
- Collaboration with the operations team to understand the Standard Operating Procedure (SOP) for fraud detection
- Feature engineering to generate features needed for rule evaluation
- Designed, developed and deployed a configurable rule based system which identifies/rejects fraud refund claims
- 20K refund_request per week are evaluated by the system eliminating manual intervention
- Experimented with image similarity algorithms to identify if the seller is using the same image of broken product

#### SellerOnboarding fraud detection : Aim of this project was to identify the sellers who were already convicted of doing fraud on the platform and trying to onboard again providing different address etc.
- Collaborated with User graph team to consume the account linking based on attributes
- Collaborated with SellerOnboarding team to integrate in the onboarding process
- Designed, developed and deployed a solution based account lining and seller profile to identify such cases
- Flipkart had more leverage now to keep fraud seller out of the system

#### Re Arch of Backend Service : Aim of this project was to come up with a set of microservices which can address a specific set of requirements (e.g. Booking Service, Billing Service, User Service, Driver Service etc) and can scale to handle 1 million bookings per day
- Contributed to re-arch discussions
- Contributed to the development of booking microservice which could handle upto 1 million bookings per day

#### Framework for REST services and Audit logging : Aim of this project was to create framework which enables async audit logging, integration with flipkart alerting & monitoring framework, meets Service Level Agreement (SLA) of 100ms response time for REST Endpoints
- Wrote a wrapper for IO calls using Netflix Hystrix  which is a latency and fault tolerance library designed to isolate points of access to remote systems, services and 3rd party libraries, stop cascading failure and enable resilience in complex distributed systems where failure is inevitable
- Integrated with multiple REST services for the first use case
- Developed Kafka consumers to ingest audit data is audit store
- Performance testing to meet the Service Level Agreement (SLA) requirements 100ms response time with 15K QPS
- Created scripted dashboard for monitoring the web services
- Wrote parameterized scripts for setting up the alerts for all future use cases

#### Installation of Hadoop cluster : Deploying dedicated hadoop cluster to execute Hive/spark jobs for crunching TBs of data for fraud detection
- Evaluation of the machine types for setting up different services of hadoop cluster
- Procuring required machines from Flipkart Internal Cloud
- Setting up all the Hadoop services using wrappers written for Hortonworks Ambari

#### Hadoop alerting and monitoring : Aim of the project was to make the alerting and monitoring robust such that any unhealthy process in hadoop cluster is surfaced and corrective measures can be taken immediately
- Designed the solution using nagios_procs plugin which publishes process health status
- Debian packaging of the solution and deployment on hadoop cluster using ansible
- Created graphs, alerts using Flipkart alerting monitoring framework

#### CICD pipeline for web-services : Aim of this project was to remove manual intervention in deployment lifecycle and reduce time to production for any newly developed code
- Evaluation of different approaches ansible, jenkins, in-house deployment service
- Development/testing of robust deployment template which enabled one click deployment
- Gave a talk on onboarding and debugging issues with deployment
- Impact - Manual intervention completely eliminated in deployment process
- We have 5 microservices, 20 boxes running in this setup
- Guided User Service team which maintains 40 node cluster of microservice to onboard to the solution

#### Performance monitoring of Scale Out Network Attached Storage : Aim of this project was to provide unified view for monitoring health of storage clusters.
- Developed collectors which collected CPU, Memory, Disk Usage metrics
- Integrated collectors with the framework which ingested the metrics to OpenTsDB and aggregated at different granularity for different timespan

#### Ola Auto : Aim of this project was to develop an alternate booking model in which the booking is broadcasted to multiple drivers and one of the drivers who accept the booking is chosen based on set of criterias
- Part of 3 member team which implemented and maintained the end-to-end system
- Primary contributor in the development of alternate booking model for Ola auto

#### CDMI based object Store : Aim of this project was to build an objectstore based on CDMI specification and ecosystem products using the Object Store
- Developed a Command Line Interface for performing file operations on CDMI store.
- Contributed to development of POC Object Store Browser
- Contributed to bug fixes in the bug fix cycle of the product

#### Satellite TCP Performance Enhancement Proxy : All the existing solution for satellite communication were proprietary, and vanilla TCP gave limited performance due to inherent long round trip time(RTT) and higher error rate in satellite communication. This was an experimental project at ISRO aimed at coming up with an proxy layer on top of TCP to enhance throughput of satellite communication. 
- Developed the proposed packet for which encapsulated the actual TCP packets
- Created a laboratory setup to test the experiments

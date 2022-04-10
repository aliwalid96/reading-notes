# Serverless

Serverless is a cloud execution model that enables a simpler, more cost-effective way to build and operate cloud-native applications.

1. Automatically provisions the computing resources required to run application code on demand, or in response to a specific event;
2. Automatically scales those resources up or down in response to increased or decreased demand;
3. Automatically scales resources to zero when the application stops running. 

Serverless offloads all management responsibility for backend cloud infrastructure and operations


Amazon Web Services introduced serverless in 2014 with AWS Lambda; today every leading cloud service provider offers a serverless platform including Microsoft Azure (Azure Functions), Google Cloud (Google Cloud Functions) and IBM Cloud (IBM Cloud Code Engine).

## Serverless vs. FaaS (function as a service)

Serverless and function as a service (FaaS) are often conflated. But FaaS is actually a subset of serverless - it's the compute paradigm central to serverless, wherein application code or containers run only in response to events or requests. Serverless includes FaaS plus all the other associated resources and cloud services and resources supporting the code - e.g. storage, databases, networks, API gateways, authentication - for which configuration, management and billing of services are invisible to the user.


## Use cases for serverless
Serverless and microservices

The most common use case of serverless today is supporting microservices architectures. The microservices model is focused on creating small services that do a single job and communicate with one another using APIs

API backends
Any action (or function) in a serverless platform can be turned into a HTTP endpoint ready to be consumed by web clients.

Data processing
Serverless is well-suited to working with structured text, audio, image, and video data, around tasks such as data enrichment, transformation, validation, cleansing; PDF processing; audio normalization; image processing (rotation, sharpening, noise reduction, thumbnail generation); optical character recognition (OCR); and video transcoding



Massively parallel compute/“Map” operations
Any kind of embarrassingly parallel task is a good use case for a serverless runtime, with each parallelizable task resulting in one action invocation.


Stream processing workloads
Combining managed Apache Kafka with FaaS and database/storage offers a powerful foundation for real-time buildouts of data pipelines and streaming apps


Common applications
In a recent IBM survey, IT professionals reported using serverless across a wide range of applications, including customer relationship management (CRM), analytics and business intelligence,
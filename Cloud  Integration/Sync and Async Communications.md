• When we start deploying multiple applications, they will inevitably need to communicate with one another
• There are two patterns of application communication

-  Synchronous -> application to application
- Asynchronous -> application to queue to application

• Synchronous between applications can be problematic if there are
sudden spikes of traffic
• What if you need to suddenly encode 1000 videos but usually it’s 10?
• In that case, it’s better to decouple your applications:
	• using [[SQS - Simple Queue Service]]: queue model
	• using [[SNS - Simple Notification Service]]: pub/sub model
	• using [[Amazon Kinesis]]: real-time data streaming model
• These services can scale independently from our application!
• Elastic Beanstalk is a developer centric view of deploying
an application on AWS
• But it’s all in one view that’s easy to make sense of!
• We still have full control over the configuration
• Beanstalk = Platform as a Service (PaaS)
• Beanstalk is free but you pay for the underlying instances

**How it works**

• Managed service
• Instance configuration / OS is handled by Beanstalk
• Deployment strategy is configurable but performed by Elastic Beanstalk
• Capacity provisioning
• Load balancing & auto-scaling
• Application health-monitoring & responsiveness
• Just the application code is the responsibility of the developer
• Three architecture models:
• Single Instance deployment: good for dev
• LB + ASG: great for production or pre-production web applications
• ASG only: great for non-web apps in production (workers, etc..)

**Health Monitoring**

• Health agent pushes metrics to CloudWatch
• Checks for app health, publishes health events
### Marcia Villalba
### Rovio

##### Basics of Monitoring Serverless

Serverless is a spectrum from nocode to containers on ec2

Serverless can be a lot of things (dynamodb, sns, sqs, step functions), doesn't have to functions

Normally a part of a distributed system
Event Driven
Asynchronous

Monitor the relationships of the different components
Some resources are owned by us, some not
Serverless presents risks with integrations of non-owned services

normally has memory limits, simple hardware, exec time limits

functions are stateless

What to monitor:

    latency
    traffic
    errors
    saturation

Metrics from every part of the serverless application is important, functions are a part of this but not the end

Base metrics/alarms on use cases, if your application doesn't read/write disk at all then why are you alarming on disk usage? (not so much serverless here)

##### How to make a serverless applications easier to Monitor

pick easily monitorable services, if they're not monitorable they'll be a nightmare to operate

##### Tooling for Serverless Monitoring

Feature wishlist:
*   Real time
*   Very little overhead in the code
*   Montioring needs to be definable in IaC
*   Support async tracing
*   Good UX/UI (not AWS)

# BUILDING RESILIENT SERVERLESS SYSTEMS
John Chapin

## What is Serverless? 
See paper done with O'Reilly and Chapin's company

## Loss of Control
The more we use serverless, we lose control. 

* Limited configuration options
* Fewer opportunities for optimization
* Hands-off issue resolution. 

Example: when S3 went down

## Werner
TODO: READ!! 10 Lessons from 10 Years of AWS
* Embrace failure

Two broad classes of failures:
- Application failures
- Service failures (our problem but not our resolution)

* What happens when those vendor-managed services fail?

## Mitigate through architecture
(aside) Open tracing

* No control over resolving actue vendor failures
* Plan for failure, architect and build applications to be resilient
* Take advantage of: 
    - Vendor designed isolation mechanisms
    - Vendor services 

* AWS Reliability Pillar

> Serverless systems tend to be continuously deployed because they are so damned hard to manage otherwise

## Not Just Resiliency

Infrastructure as a code minimizes incremental work in deploying to new region

## Demo
* Global, highly resilient service
* SAM: Serveral Application Model 
* He provides the source code

## Additional Approaches
* Multi-region-codepipeline (Github)

## AWS Resources Page



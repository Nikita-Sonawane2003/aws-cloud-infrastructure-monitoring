# AWS Cloud Infrastructure Monitoring & Automated Alert System

## Project Overview
This project monitors an AWS EC2 instance using Amazon CloudWatch. It uses CloudWatch dashboards and alarms to monitor CPU utilization and network traffic, with email notifications through Amazon SNS.

## Objectives
- Monitor EC2 CPU utilization.
- Visualize monitoring metrics using CloudWatch dashboards.
- Generate alerts when CPU utilization crosses a configured threshold.
- Monitor EC2 network traffic using NetworkIn and NetworkOut metrics.
- Send email notifications through Amazon SNS.

## AWS Services Used
- **Amazon EC2** – Virtual server
- **AWS IAM** – Permissions for CloudWatch Agent
- **Amazon CloudWatch** – Metrics, dashboards, and alarms
- **Amazon SNS** – Email notifications
- **CloudWatch Agent** – Additional system monitoring metrics

## Implementation
1. Launched an EC2 instance.
2. Configured an IAM role and installed the CloudWatch Agent.
3. Created a CPU utilization alarm with a 70% threshold.
4. Configured an SNS email notification.
5. Created a CloudWatch dashboard and added a CPU graph.
6. Created a network traffic alarm using the NetworkIn metric.
7. Tested the CPU alarm using a stress test.

## Testing Results
The CPU stress test triggered the CloudWatch alarm, and an email notification was received. The network traffic alarm was created; its triggering behavior has not yet been verified.

## Screenshots
See the `Screenshots` folder for project implementation screenshots.

## Future Enhancements
- Configure SMS notifications.
- Verify memory and disk monitoring.
- Test network traffic alarms.
- Add additional monitoring metrics.

## Author
Nikita Sonawane

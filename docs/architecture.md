# Architecture

This project deploys a static website on an AWS EC2 instance using Nginx.

## AWS Architecture

VPC CIDR: 10.0.0.0/16

Subnets:
- Frontend subnet: 10.0.0.0/24
- Backend subnet: 10.0.1.0/24
- Database subnet: 10.0.2.0/24

The EC2 instance hosting the website is deployed in the frontend subnet.

An Internet Gateway allows public access to the instance through HTTP and HTTPS.

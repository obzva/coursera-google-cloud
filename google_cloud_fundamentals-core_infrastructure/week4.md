# Recap from quiz
## VMs and Networks in the Cloud
### VPC
- VPC belongs to Google Cloud projects
### VPC Network
- Networks are **global** and subnets are **regional**
### VPC Compatibilities
- Routing tables: Built-in so that you don't have to provision or manage it
- Firewall: You don't have to provision or manage
### Cloud load balancing
- The job of a load balancer is to distribute user traffic across multiple instances of an application
- VPC offers a suite of load-balancing options
- Global HTTP(S): When cross-regional load balancing for a web application is in need
- Global SSL Proxy: For SSL(Secure Sockets Layer) traffic that is not HTTP
- Global TCP Proxy: If it’s other TCP traffic that doesn’t use SSL
- Regional: If you want to load balance UDP traffic, or traffic on any port number
- Regional Internal: For load balancing traffic inside of project, say, between presentation layer(FE) and business layer(BE) of the application

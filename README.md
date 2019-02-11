# Your-Own-VPN
## You NEED to have GCP or AWS account to set up your own VPN. There are two approaches creating VPN.
### I strongly recommand you that apply for a new account. GCP gives you $300(+$54)credit, and AWS allows you to use Cloud service 1 year for free. 

### It is important that the AWS free tier only gives you 750 hours/month for all running VM instance(s) for free. If you go beyond 750 hours you need to pay. For instance, I have a Ubuntu instance and a Centos instance running on AWS, and keep them running for whole month. 2(instances) * 24(hour/day) * 31(day/month) = 1488 hrs. 1488 > 750, you need to pay extra. 

### ![Image of equation](https://github.com/shanerbo/Your-Own-VPN/blob/master/Sumation.gif) n = days in calendar month, alpha beta and gamma are daily average running time for each instance. If you are in free tire, you can only have **ONE** instance running 24/7. 1 * 24 * 31 = 744 hrs.
## **So keep it in mind, never keep two or more than two instances running unless you are Bruce Wayne.**

## GCP:

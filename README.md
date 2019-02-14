## YourOwnVPN
#### Going back to China without a solid VPN is a nightmare. Tons of VPN's get banned in China, and the rest of them charges like crazy. Why don't you have your own personal private VPN?
#### You NEED to have [GCP](https://console.cloud.google.com/home/dashboard?project=person-web) or [AWS](https://portal.aws.amazon.com/billing/signup#/) account to set up your own VPN. 
##### I strongly encourage you to apply for a new account if you *DO NOT* have a account yet. GCP gives you $300(+$54)credit, and AWS allows you to use Cloud service 1 year for free (some [restrictions](https://aws.amazon.com/free/?awsf.Free%20Tier%20Types=categories%2312monthsfree) may apply). They are pretty much same.

#### It is important that the AWS free tier only gives you 750 hours/month for all running VM instance(s) for free. If you go beyond 750 hours you need to pay. For instance, I have a Ubuntu instance and a Centos instance running on AWS, and keep them running for whole month. 2(instances) * 24(hour/day) * 31(day/month) = 1488 hrs. 1488 > 750, you need to pay extra. 

#### ![Image of equation](https://github.com/shanerbo/Your-Own-VPN/blob/master/Sumation.gif) n = days in calendar month, alpha beta and gamma are daily average running time for each instance. If you are in free tire, you can only have **ONE** instance running 24/7. 1 * 24 * 31 = 744 hrs.
### *So keep it in mind, never have two or more than two instances keep running 24/7 unless you are Bruce Wayne.*

#### Personal speaking, I prefer GCP to AWS, because its UI looks nicer than AWS. Its all up to you. One thing needs to be mentioned that you need to be aware of your GCP credit, setting up a budget alert can prevent you from bankrupt. 
## GCP:
- Log into GCP, Click on "Compute Engine" -> "VM instances" -> "Create"
### Create Instance
![createInstance](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPCreateInstance.png)
### Set up Firewall
![SetUpFirewall](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPVPCNetwork.png)

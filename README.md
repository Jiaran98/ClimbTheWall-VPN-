## Create Your Own VPN
#### Going back to China without a solid VPN is a nightmare. Tons of VPN were banned in China, and the rest of them charges like crazy. Why don't you have your own personal private VPN?
#### To set up your own VPN, you NEED to have accounts for [GCP](https://console.cloud.google.com/home/dashboard?project=person-web) or [AWS](https://portal.aws.amazon.com/billing/signup#/) . 
##### I strongly encourage you to apply for a new account if you *DO NOT* have an account already. GCP gives you $300(+$54)credit, and AWS allows you to use Cloud service 1 year for free (some [restrictions](https://aws.amazon.com/free/?awsf.Free%20Tier%20Types=categories%2312monthsfree) may apply). They are pretty much the same.

#### The AWS free tier offers a 750 hours/month running time for all running VM instance(s). If all VM instances running time goes over 750 hours, extra fees will be charged. (E.g. I kept a Ubuntu instance and a Centos instance running on AWS for a whole month. 2(instances) * 24(hour/day) * 31(day/month) = 1488 hrs. 1488 > 750, Therefore, I have to pay extra fees.)

#### ![Image of equation](https://github.com/shanerbo/Your-Own-VPN/blob/master/Sumation.gif) n = days in calendar month, alpha beta and gamma are daily average running time for each instance. If you are in free tire, you can only have **ONE** instance running 24/7. 1 * 24 * 31 = 744 hrs.
### *So keep it in mind, never have two or more than two instances keep running 24/7 unless you are Bruce Wayne.*

#### Its all up to you to choose between Google Cloud Platform and Amazon Web Service. Personal speaking, I prefer GCP over AWS because of GCP has a nicer UI. One thing worth mentioning is that you need to be aware of your GCP credit. Setting up a budget alert can prevent you from bankrupcy. 
## GCP:
- Log into GCP, Click on "Compute Engine" -> "VM instances" -> "Create"
### Create Instance
#### You may need to create your own project so that you could create a vm instance.
![createInstance](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPCreateInstance.png)
### Set up Firewall
![SetUpFirewall](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPVPCNetwork.png)
### Create Firewall Rules
![FirewallRules](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPFirewallRules.png)
### Create Rules For Ingress and Egress
### Ingress:
![Ingress](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPAddRules.png)
### Egress:
![Egress](https://github.com/shanerbo/YourOwnVPN/blob/master/GCPAddRulesEgress.png)
## Use default VM instance for saving money(roughly $20/month).
##### AWS cloudformation does not support VPN



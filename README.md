# Project 9 - Honeypot

Time spent: 15 hours spent in total

> Objective: Setup a honeypot and intercept some attempted attacks in the wild

## Which Honeypots You Deployed

1. **Dionaea over HTTP**

    The first honeypot that I deployed was the Dionaea over HTTP honeypot because it was the honeypot that
    we configured in the Codepath instructions which were given to us. I configured this honeypot using a 
    vm that I provisioned on the GCP. The main purpose of the Dionaea over HTTP honeypot is to trap malware
    samples and gain access to those malware samples. 

2. **Shockpot Sinkhole**
    
    The second honeypot that I deployed was the Shockpot Sinkhole honeypot which I also configured by 
    following the Codepath instructions that were given to us. I configured this honeypot using the same
    stack as the first honeypot, and I provisioned a vm for this honeypot on the GCP. The main purpose
    of the Shockpot Sinkhole honeypot is to find attackers attempting to exploit the Bash remote code
    vulnerability. 

## GIFs and Screenshots

1. Screenshot of VMs on Google Cloud: https://imgur.com/yabrO6e
2. Screenshot of MHN Server Sensors: https://imgur.com/a/E3uwiXx
3. Screenshot of MHN Server Attack Stats: https://imgur.com/a/jiFQd5K
4. Screenshot of MHN Server Attacks Report - Dionaea: https://imgur.com/a/gtTWnQx
5. Screenshot of MHN Server Attacks Report - Shockpot: https://imgur.com/a/20Zvp6S
6. ***GIF***

## Issues Encountered 
There were a few issues which I encountered while doing this assignment, however, most of these issues
were resolved by an email sent out by my TA Shashank.

1. At first, I was not able to connect to the MHN Admin console even though I had provisioned my VM
   on Google Cloud by following the directions. I later found out that this problem was caused by
   not allowing traffic to the external IP via HTTP and HTTPS
2. The directions were not clear on how to sign in to `gcloud` through the command line. I had to 
   research this online and used the command `gcloud auth login` in order to authenticate with 
   `gcloud`
3. I was trying to use `yum` in order to install the gcloud sdk, however using the command provided
   by my TA `curl https://sdk.cloud.google.com | bash` was much simpler 
    
## A Summary of the Data Collected: Number of Attacks, Number of Malware Samples, etc.

1. **Dionaea over HTTP**


2. **Shockpot Sinkhole**

## Any Unresolved Questions Raised by the Data Collected

## JSON 

## Resources
* GIFs created with LiceCap
* https://github.com/rep/dionaea
* https://github.com/threatstream/shockpot

## License

    Copyright [2018] [Kamran Rana]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

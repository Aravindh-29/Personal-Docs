# Platform As A Service 
* Code into Cloud 

* Compute services in the cloud are used to run applications developed.
* Available Clouds:
    * public cloud
    * private cloud
    * Hybrid cloud
    * community cloud (not much popular)

#### Let look at an application :

* We have an calulator application that calculates loans, we can run this in on physical computer.
* how to make it available for everyone to access this
    * go to website who sells domains like Hostinger,godaddy..etc
    * when we buy a domanin, we get DNS servers hosted by doimain seller where we have records.
* whenever you try to type a name of site in browser for accessing any site it resolved into ip address
* How DNS works:
![alt text](image.png)
    * when you type bookmyshow.com in browser, your computer will first check in Resolving Name server(Name to Ip address), then Root Name (.in or .com)server and TLD(top level domain) Name Server and 
    
    * Resolving Name server
        * Name to Ip address
    * Root Name server
        * these servers holds all the websites that ends with .in or .com...etc
    * TLD server(Top level domain server)
        * your application will be stored
    * Authritative servers
        * all the record are saved here
        * like A records(Name to Ip address), c records(Alias records like fb.com)
* DNS lookup , go to dns lookup website site from internet and enter the website names and check ip address and records like : bookmyshow.com,instagram.com..etc

* Hosting options:
    * on- prem
    * cloud

* IN on-prem:(VM ware)
    * on physical server, companies tries to create vmware esxi and create server instances, they will host websites in each of the instances.

* ON Cloud:
    * from AWS perspective, EC2 will replace this scenario 
    * from Azure perspective, Azure VM replaces this scenario
    * these falls under IAAS 

* For above things we need to maintain patches, installing of programmming languages on server. Maintaines from our side is needed.

* There comes an idea , For running any application do we need Os or program Runtime obiviously it is Run time, because you can install run time on any os and you can run the app.

* Here comes idea of PAAS:
    * Cloud provides Run time execution environments according to techology/platform
    * In Azure = App Services
    * in Aws   = Elastic Bean Stalk

* This is not stoped yet, there is another idea came Serverless stalks
* The idea is if you think your website is not much used, and you need to save costs on this, here comes the idea of serverless
* Serverless feature costs you only when your server is used, there is no cost if no one is using your server.

* In Azure = Azure Functions.
* In AWS   = Lambda.
![alt text](<PAAS _images/1.png>)


**8 May**





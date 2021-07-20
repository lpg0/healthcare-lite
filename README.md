### Goals 

Gain hands-on experience writing an IaaS cloud application, specifically by using Amazon Web Services (AWS). Secondary goals are to gain experience administering a Windows Server machine and to gain/reinforce experience with SQL and Web programming. 

### Introduction

This projects is a “Lite” version of healthcare.gov by following the instructions below (the original roll-out of healthcare.gov was a mess). This project consisted generally of 3 parts: [1] setting up the Web frontend; [2] setting up the cloud database to hold the specific health plans; [3] creating the Web functionality (which is given to you) to show the health plans on the Web page and making it so that a person can register for a plan.  

### Setup

Due diligence for any cloud project starts with setting a budget to limit resource usage overflow. Always be sure to consistently change the AWS region to what is physically closest (as seen in the top right of the dashboard). Create a cost budget, giving adequate notification metrics. It is recommended that an email notification would be sent after 75% of the indicated budget. Below is a screenshot of the budget I created.

![budget](C:\Users\lukep\Desktop\Projects\UVA Engineering Items\4740 Cloud\pa1\pa1-budget.png)

### Strategy

The first step was creating a working frontend using a local SQL server. The frontend for the site was created using a “Microsoft Windows Server 2016 with SQL Server 2017 Express” EC2 instance. The default size was changed to "t3a.xlarge" for cost-feature maximization. The second step was to port the database functionality tested in part 1 to the cloud. An RDS “Microsoft SQL Server” was used to test fake health information data. Below is a sample SELECT query to test the frontend display, and the final project being displayed on localhost.

![pa1-sql-server](C:\Users\lukep\Desktop\Projects\UVA Engineering Items\4740 Cloud\pa1\pa1-sql-server.png)

![pa1-web](C:\Users\lukep\Desktop\Projects\UVA Engineering Items\4740 Cloud\pa1\pa1-web.png)

### Notes

This project is no longer being served on AWS due to budget constraints.

### Acknowledgements

Thanks goes to Marty Humphrey (University of Virginia, 2021) for providing project guidelines during CS 4740 S21.
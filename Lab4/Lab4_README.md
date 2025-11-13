# Lab #4: Alerts and Automation Accounts

**Student: Olga Durham**

**Student#: 040687883**

---

## <u>Main Tasks for Azure:</u>

1. Create Virtual Machine based on these settings:

   a. Region: east US 2

   b. Availability options: no infrastructure redundancy required

   c. Security type: Standard

   d. Image: Ubuntu server 24.04 LTS

   e. VM Architecture: X64

   f. Size: standard B1s ( should be around $3.80 a month)

   g. Public inbound ports: None

   h. OS disk type: standard SSD(locally redundant storage)

   i. no load balancers or NIC network security groups are necessary

   j. Create a meaningful tag and value /10

2. Create alert rule and corresponding action group for virtual machine created in step 1, if Percentage CPU goes over certain metric stop the virtual machine /6

3. Create an Automation account /1

4. Create a runbook in powershell in the automation account /1

5. Edit the code so that it will stop the virtual machine you created in Step 1 if it has a specific tag and test the code to see if it stops the virtual machine /6

6. After demo delete all resources and policies created /1

Total: /23

<u>Screenshots:</u>

<u>Step 1:</u>

Include screenshots that display each of those settings being selected and the virtual machine being created

<u>Step 2:</u>

Include screenshots of alert rule being created for the virtual machine, with logical aggregation type, operator, threshold value and checks. Also, include the screenshots of the action group being created in the correct region, and selecting the correct action group which has a built-in functionality that will let you stop the virtual machine.

<u>Step 3:</u>

Include screenshots showing you have created the automation account in the same region as all other resources (East US 2)

<u>Step 4:</u>

Include screenshots displaying the creation of a runbook that uses powershell 5.1 as the runtype and version.

<u>Step 5:</u>

Include screenshots of the final code, of you selecting test pane and testing the code to see if it works and stops the virtual machine, and final screenshot of the stopped virtual machine you created in step 1

<u>Step 6:</u>

Screenshot showing resources have all been deleted or just delete resource group

**Some students are having issues with this lab and if that's the case, please show the screenshots of the errors creating the automation account, and do this lab below.**

**Main Tasks for Azure**

1. In a GitHub repo, you can add just a simple html file, or also CSS file and anything else needed for a web application, you want /6

2. Create a static web app select Free as plan type and link to your GitHub account /2

3. Ensure that in your GitHub repo a workflows folder was created and there is a .yml file /2

4. Click to go to your new site(this may take a couple of minutes for it to be deployed) /1

5. Update the html file in repo change the name or add something to it /2

6. Confirm that site get automatically updated with new change /1
   Delete resources /1

<u>Step 1:</u>

Screenshot of html file content in repo and all other files, provide link but make sure I have access

<u>Step 2:</u>

Screenshot must show the process of creating static web app, show that free plan was selected and that github account was linked and repo name selected

<u>Step 3:</u>

Screenshot should show that workflow folder was added to repo and content of .yml file

<u>Step 4:</u>

Screenshot of the site

<u>Step 5:</u>

Screenshot of the file you’ve updated, so I can view the difference.

<u>Step 6:</u>

Screenshot of new site showing the change.

<u>Step 7:</u>

Resources being deleted, or resource group being deleting, show either no resources available or confirmation of deletion of resources

Due on Nov 23, 2025 11:59 PM

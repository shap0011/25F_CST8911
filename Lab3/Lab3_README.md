# Lab #3: Deploy Virtual Machine via Custom Templates

**Student: Olga Durham**

**Student#: 040687883**

---

## 1. Using the deploy a custom template azure service, create a custom template to deploy a linux virtual machine, that contains the following settings:

a. Region: east us

b. Availability Options: no infrastructure redundancy required

c. Security Type: standard

d. Image: ubuntu server 22.04 LTS

e. Size: standard_b1ls -1 vcpu, 0.5 Gib memory

f. Authentication type: password (include username and password in the template)

g. Public inbound ports: None

h. Os Disk type: Standard SSD

i. Specify virtual network in the template

j. NIC network security Group: None

k. Load balancing options: None

l. Add a tag

Once created ensure it deploys and verify that the virtual machine was created /20

## 2. Delete resources created in this lab /1

### Screenshots:

<u>Step 1:</u>

Attach your json custom template as a separate file

Screenshot showing successful deployment from the custom template

So I can verify that the virtual machine from the json template was created. Screenshots should include verifications of each of the settings in step 1, so the screenshots should show the virtual machine once it is created and its settings ensure you display the

- Region
- Availability Options
- Security Type
- Image
- Size
- Public inbound ports
- Os Disk type
- virtual network
- Load balancing options
- tag that was created

<u>Step 2:</u>

Screenshot showing that all resources were deleted

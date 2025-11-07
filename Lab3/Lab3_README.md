# Lab #3: Deploy Virtual Machine via Custom Templates

**Student: Olga Durham**

**Student#: 040687883**

---

## 1. Using the deploy a custom template azure service, create a custom template to deploy a linux virtual machine, that contains the following settings:

a. Region: Canada Central (as "east us" doesn't work for the "Azure Student" subscription)

changed 'location -> default value' to 'canadacentral'

```
"location": {
      "type": "string",
      "defaultValue": "canadacentral",
      "metadata": {
        "description": "Specifies the location for all resources."
      }
    }
```

b. Availability Options: no infrastructure redundancy required

no changes needed

c. Security Type: standard

added to 'resources -> Microsoft.Compute/virtualMachines'

```
		"securityProfile": {
			"securityType": "Standard"
		},
```

d. Image: ubuntu server 22.04 LTS

edited imageReference `sku` to the non-gen2

```
          "imageReference": {
            "publisher": "Canonical",
            "offer": "0001-com-ubuntu-server-jammy",
            "sku": "22_04-lts",
            "version": "latest"
          }
```

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

[How to create a Linux virtual machine with Azure Resource Manager templates](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/create-ssh-secured-vm-from-template)

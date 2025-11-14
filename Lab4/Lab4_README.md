# Lab #4: Alerts and Automation Accounts

**Student: Olga Durham**

**Student#: 040687883**

---

# Main Tasks for Azure:

## 1. Create Virtual Machine based on these settings:

a. Region: `east US 2`

b. Availability options: `no infrastructure redundancy required`

c. Security type: `Standard`

d. Image: Ubuntu server `24.04 LTS`

e. VM Architecture: `X64`

f. Size: `standard B1s` ( should be around $3.80 a month)

g. Public inbound ports: `None`

h. OS disk type: `standard SSD`(locally redundant storage)

i. no load balancers or NIC network security groups are necessary

j. Create a meaningful tag and value /10

**2. Create alert rule and corresponding action group for virtual machine created in step 1, if Percentage CPU goes over certain metric stop the virtual machine /6**

**3. Create an Automation account /1**

**4. Create a runbook in powershell in the automation account /1**

**5. Edit the code so that it will stop the virtual machine you created in Step 1 if it has a specific tag and test the code to see if it stops the virtual machine /6**

**6. After demo delete all resources and policies created /1**

**Total: /23**

---

# Screenshots:

## ➡️ Step 1: Create Virtual Machine based on given settings

Include screenshots that display each of those settings being selected and the virtual machine being created

<img src="./screenshots/step_1_1_settings_selected.png" alt="" title="Setting tab Basics" width="700"/>

<img src="./screenshots/step_1_2_settings_selected.png" alt="" title="Setting tab Basics" width="700"/>

<img src="./screenshots/step_1_3_settings_selected.png" alt="" title="Setting tab Disks" width="700"/>

<img src="./screenshots/step_1_4_settings_selected.png" alt="" title="Setting tab Networking" width="700"/>

<img src="./screenshots/step_1_5_settings_selected.png" alt="" title="Setting tab Tags" width="700"/>

<img src="./screenshots/step_1_6_vm_created.png" alt="" title="Virtual Machine created" width="1100"/>

<img src="./screenshots/step_1_7_vm_overview.png" alt="" title="Virtual Machine overview" width="1100"/>

<img src="./screenshots/step_1_8_properties.png" alt="" title="Virtual Machine Properties" width="1100"/>

<img src="./screenshots/step_1_9_properties.png" alt="" title="Virtual Machine Properties" width="1100"/>

---

## ➡️ Step 2: Create alert rule and corresponding action group for virtual machine

Include screenshots of alert rule being created for the virtual machine, with logical aggregation type, operator, threshold value and checks. Also, include the screenshots of the action group being created in the correct region, and selecting the correct action group which has a built-in functionality that will let you stop the virtual machine.

<img src="./screenshots/step_2_1_create_an_alert_rule_scope.png" alt="" title="Create an alert rule Scope" width="700"/>

<img src="./screenshots/step_2_2_create_an_alert_rule_condition.png" alt="" title="Create an alert rule Condition" width="1100"/>

<img src="./screenshots/step_2_3_create_an_alert_rule_select_actions.png" alt="" title="Create an alert rule Select Action" width="700"/>

<img src="./screenshots/step_2_4_create_an_alert_rule_action_group_basics.png" alt="" title="Create an alert rule, Action Group Basics" width="800"/>

<img src="./screenshots/step_2_5_create_an_alert_rule_action_group_actions_configure_runbook.png" alt="" title="Create an alert rule, Action Group Actions, configure runbook" width="1100"/>

<img src="./screenshots/step_2_6_create_an_alert_rule_action_group_actions_selections_conpleted.png" alt="" title="Create an alert rule, Action Group Actions, settings completed" width="700"/>

<img src="./screenshots/step_2_7_create_an_alert_rule_action_group_review.png" alt="" title="Create an alert rule, Action Group review" width="600"/>

<img src="./screenshots/step_2_8_create_an_alert_rule_action_group_failure_error.png" alt="" title="Create an alert rule, Action Group failure error" width="500"/>

<img src="./screenshots/step_2_9_create_an_alert_rule_action_group_failure_error_copilot_troubleshooting.png" alt="" title="Create an alert rule, Action Group failure error Copilot troubleshooting" width="1100"/>

❗**To fix the error the Automation Account must be created first**

‼️**Create action group after completing Task 3 and Task 4**

<img src="./screenshots/step_2_10_recreate_action_group.png" alt="Configure Runbook" title="" width="1100"/>

<img src="./screenshots/step_2_11_virtual_machine_contributor_role_assigned.png" alt="" title="Virtual Machine Contributor role assigned notification" width="1100"/>

<img src="./screenshots/step_2_12_create_action_group_review+create.png" alt="" title="Create action group review" width="400"/>

<img src="./screenshots/step_2_13_action_group_created_successfully.png" alt="" title="Action group created successfully" width="400"/>

<img src="./screenshots/step_2_19_action_group_shown_up.png" alt="" title="Action Group shown up" width="1100"/>

**Creating alert rule**

<img src="./screenshots/step_2_14_create_an_alert_rule_select_action_group.png" alt="" title="Create an alert rule. Select action groups" width="1100"/>

<img src="./screenshots/step_2_15_create_an_alert_rule_review.png" alt="" title="Create an alert rule. Review" width="500"/>

<img src="./screenshots/step_2_16_create_an_alert_rule_review.png" alt="" title="Create an alert rule. Review" width="500"/>

<img src="./screenshots/step_2_17_created_an_alert_rule_notification.png" alt="" title="Created the alert rule. Notification" width="500"/>

<img src="./screenshots/step_2_18_alert_rule_under_VM.png" alt="" title="Alert rule show up under VM -> Alerts" width="1100"/>

---

## ➡️ Step 3: Create an Automation account

Include screenshots showing you have created the automation account in the same region as all other resources (East US 2)

<img src="./screenshots/step_3_1_create_an_automation_account_review.png" alt="" title="Create an Automation Account Setting review" width="500"/>

<img src="./screenshots/step_3_2_create_an_automation_account_created.png" alt="" title="Automation Account created" width="1100"/>

<img src="./screenshots/step_3_3_create_an_automation_account_overview.png" alt="" title="Automation Account overview" width="1100"/>

---

## ➡️ Step 4: Create a runbook in powershell in the automation account

Include screenshots displaying the creation of a runbook that uses powershell 5.1 as the runtype and version.

<img src="./screenshots/step_4_1_create_a_runbook_review.png" alt="" title="Create a runbook setting review" width="400"/>

<img src="./screenshots/step_4_2_runbook_is_created.png" alt="" title="Runbook is created notification" width="1100"/>

---

## ➡️ Step 5: Edit the code so that it will stop the virtual machine

Include screenshots of the final code, of you selecting test pane and testing the code to see if it works and stops the virtual machine, and final screenshot of the stopped virtual machine you created in step 1

<img src="./screenshots/step_5_1_final_code.png" alt="" title="Final code" width="800"/>

<img src="./screenshots/step_5_2_saved_runbook.png" alt="" title="Successfully saved runbook" width="400"/>

<img src="./screenshots/step_5_3_published_runbook.png" alt="" title="" width="400"/>

<img src="./screenshots/step_5_4_redirect_to_test_pane.png" alt="" title="" width="500"/>

<img src="./screenshots/step_5_5_test_result_succeeded.png" alt="" title="" width="500"/>

<img src="./screenshots/step_5_6_virtual_machine_stopped.png" alt="" title="" width="500"/>

---

## ➡️ Step 6: After demo delete all resources and policies created

Screenshot showing resources have all been deleted or just delete resource group

<img src="./screenshots/step_6_1_resource_group_deleted.png" alt="" title="" width="500"/>

<img src="./screenshots/step_6_2_resource_group_deleted.png" alt="" title="" width="500"/>

---

_Due on Nov 23, 2025 11:59 PM_

**References:**

1. [Get-AzVM](https://learn.microsoft.com/en-us/powershell/module/az.compute/get-azvm?view=azps-14.6.0)
2. [Azure Automation runbook types](https://learn.microsoft.com/en-us/azure/automation/automation-runbook-types?tabs=lps74%2Cpy10)

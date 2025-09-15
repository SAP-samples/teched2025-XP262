# Exercise 1 - SAP Application Extension Methodology

In this exercise, you'll assume the role of an Enterprise Architect. You’re a member of ACME Corporation’s Enterprise Architecture team, tasked with creating a target solution diagram to prepare for the implementation of this extension use case. Having recently learned about the SAP Application Extension Methodology, you plan to apply it to guide the architecture of this project.

## Exercise 1.1: Use case example: Sales order process extension

> 1. Read the Business Case.
> 2. Read the Architecture Principals and Business Context.


### Business Case

The sales department at ACME Corporation has specific requirements for its end-to-end lead-to-cash sales order process - specifically for sales order data entry and the approval workflow. The Cloud ERP will remain the system of record for sales orders. A fit-to-standard workshop concluded these requirements cannot be met with SAP standard applications. Because the custom process offers a competitive advantage, ACME’s leadership approved its development on the condition that it follows the Clean Core strategy.
A custom sales order entry app on SAP BTP validates input and posts orders to the Cloud ERP using standard APIs. The UI displays customer, product, quantity, and delivery date. Product data is retrieved from the Cloud ERP. An internal sales representative enters the order details and triggers the automated approval workflow.
ACME’s sales order entry requires additional validations and approvals. The automated approval workflow is triggered when the quantity exceeds defined thresholds (e.g., >10). All these scenarios require approval from the Sales Manager. The solution must include two forms — "Sales Order Approval" and "Sales Order Rejected" — each displaying product, quantity, customer name, expected delivery date, and a free-text message field for the buyer.

### Architecture Principals and Business Context:
- Extensions needs to be upgrade stable and follow Clean Core Level A
- SAP Build Low-code/No-code tools are preferred for development (?Citizen Developer?)
- Side-by-Side options are preferred for workflow implementation and UIs
- ACME employees are used to access SAP application through SAP Build Work Zone

## Exercise 1.2: Assess Extension Use Case

> 1. Learn about the SAP Application Extension Methodology - 
 <a href="https://help.sap.com/docs/sap-btp-guidance-framework/sap-application-extension-methodology/phase-1-assess-extension-use-case?locale=en-US)" target="_blank">Phase 1: Assess Extension Use Case</a>
> 2. Read the example solution for System Context, Business Context & Requirement, and Application Extension Use Case. To speed up the hands-on exercicse, we already provide you with the solution. In later exercises you will fill out the templates on your own.

### System Context
<details>
<summary>🔵 Click to expand.</summary>

![System Context](./images/example_system_context.jpg)

</details>

### Business Context & Requirement
<details>
<summary>🔵 Click to expand.</summary>

![System Context](./images/Business%20Context%20&%20Requirement.jpg)

</details>

### Application Extension Use Case
<details>
<summary>🔵 Click to expand.</summary>

![System Context](./images/Application%20Extension%20Use%20Case%20Scene%20-%20Sales%20order%20process%20extension.jpg)

</details>

## Exercise 1.3: Assess Extension Technology

> 1. Learn about the SAP Application Extension Methodology - 
<a href="https://help.sap.com/docs/sap-btp-guidance-framework/sap-application-extension-methodology/phase-2-assess-extension-technology?locale=en-US" target="_blank">Phase 2: Assess Extension Technology</a>. 
> 2. Focus on Extension Tasks and the Extension Technology Mapping.

### Exercise 1.3.1: Extension Task
You start to translate your business requirement into a technical requirement through extension tasks, by mapping each requirement from the use case description (phase 1) to one or many extension tasks. 

At this step, you’re still technology-agnostic, thus empowering you to ignore any possible technical limitations. This enables you to think freely without worrying about technical limitations. 

> 1. Download the PowerPoint template (link). 
> 2. The template is pre-filled with the business use case details for Phase 1.
> 3. Fill out Phase 2 (Extension Task) of the template for each scene.
> 4. Ask yourself: Which Extension Task can solve the business requirement as defined in the "Actions" and "Application Logic" row?

<details>
<summary>⚠️ Click to expand - spoiler - example solution</summary>

</details>

### Exercise 1.3.2: Extension Technology Mapping
The extension technology mapping outlines the relationship between extension tasks and technical extension building blocks.

> 1. Download the spreadsheet template for the Extension Technology Mapping (link).
> 2. The contents of the spreadsheet were greatly reduced to make the exercise simpler and faster.
> 3. Make yourself familiar with the various technical options for each extension task.

## Exercise 1.4:  Define Extension Target Solution
> 1. Learn about the SAP Application Extension Methodology - 
<a href="https://help.sap.com/docs/sap-btp-guidance-framework/sap-application-extension-methodology/phase-3-define-extension-target-solution?locale=en-US" target="_blank">Phase 3: Define Extension Target Solution</a>

### Exercise 1.4.1: Extension Technology per Extension Task
> 1. Fill out Phase 3 (technical extension building block) for each scene.
> 2. Use the Extension Technology Mapping spreadsheet to choose the right building block for each extension task.
> 3. Remember the Architecture Principals and the Business Context from the business use case (exercise 1.2) to make an informed decision.


<details>
<summary>⚠️ Click to expand - spoiler - example solution</summary>

</details>

### Exercise 1.4.2: Extension Target Solution Diagram
Create your extension target solution by reusing the official SAP Business Technology Platform diagrams & icons.

> 1. Download the [BTP Solution Diagrams](https://sap.github.io/btp-solution-diagrams/) Icons.
> 2. Create the solution diagram. 
> 3. To speed up the process you can use the pre-filled PowerPoint template from exercicse 1.3.1.

<details>
<summary>⚠️ Click to expand - spoiler - example solution</summary>

</details>

## Summary

- You have now completed the first part of the hands-on workshop
- You successfully used the SAP Application Extension Methodology.
- You have a clear understanding about the business use case.
- You have made informed decisions about which technologies to use.
- You ensured a future-proof and clean core architecture.
- You have created a solution diagram, which is the starting point for your implementation.

Continue to - [Exercise 2 - SAP Build Process Automation](../ex2-SAP_Build_Process_Automation/README.md)
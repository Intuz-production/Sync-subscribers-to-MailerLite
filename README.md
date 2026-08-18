# Intuz — Your automation partner, one workflow at a time.

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

# Sync new subscribers from Google Sheets to MailerLite without duplicates

Intuz helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[Website](https://intuz.com) · [N8N Creator](https://n8n.io/creators/intuz/) · [Workflow Automation](https://www.intuz.com/workflow-automation-services/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

---

This n8n template from Intuz provides a complete solution to automate the syncing of new subscribers from Google Sheets to MailerLite. It intelligently identifies and adds only new contacts, preventing duplicates and ensuring your email lists are clean and accurate.

## Who's this workflow for?

* Marketing Teams
* Email Marketers
* Small Business Owners
* Community Managers

## How it works

### 1. Read from Google Sheets

The workflow begins by reading all contact rows from your designated Google Sheet.

### 2. Check for Existing Subscribers

For each contact, it performs a search in MailerLite to check if a subscriber with that email address already exists.

### 3. Handle Duplicates

If the subscriber is found in MailerLite, the workflow stops processing that specific contact, preventing any duplicates from being created.

### 4. Create New Subscribers

If the contact is not found, the workflow proceeds to create a new subscriber in MailerLite, using all the details from the Google Sheet, such as name, company, and country, and assigns them to the specified group.

## Setup Instructions

### 1. Google Sheets Setup

* Connect your Google Sheets account to n8n.
* Create a sheet with the required columns: `Email`, `first_name`, `last_name`, `Company`, `Country`, and `group_id`.
* In the **"Get row(s) in sheet"** node, select your credentials and specify the Document ID and Sheet Name.

### 2. MailerLite Setup

* Connect your MailerLite account to n8n using your API key.
* In both the **"Get a subscriber"** and **"Create subscriber..."** nodes, select your MailerLite credentials.
* Make sure the `group_id` values in your Google Sheet correspond to valid Group IDs in your MailerLite account.

### 3. Activate Workflow

Save the workflow and click **"Execute workflow"** to run the sync whenever you need to update your subscriber list.

## Connect with us

* **Website:** https://www.intuz.com/n8n-workflow-automation-templates
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz
* **Get Started:** https://n8n.partnerlinks.io/intuz
* **For Custom Workflow Automation:** https://www.intuz.com/get-started/

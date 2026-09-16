*Intuz — Your automation partner, one workflow at a time.*

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

[Intuz](https://www.intuz.com) helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[N8N Creator](https://n8n.io/creators/intuz/) · [Business Process Automation](https://www.intuz.com/ai-automation-services/) · [AI Development Company](https://www.intuz.com/company/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

# Sync new subscribers from Google Sheets to MailerLite without duplicates

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

## FAQ

**Is this template free to use?**
Yes. It's an open-source n8n workflow published by Intuz — copy the workflow JSON from this repo and import it into your own n8n instance at no cost.

**Do I need a paid n8n plan to run this?**
No. It runs on n8n's free self-hosted Community Edition or on n8n Cloud. You'll need your own credentials for the services this workflow connects to, not a specific n8n pricing tier.

**Will it create duplicate subscribers if I re-run it?**
No — the workflow checks for existing contacts before adding new ones, so re-running it against the same sheet won't create duplicates in MailerLite.

## Related n8n templates from Intuz

- [Automate QuickBooks customers & sales receipts generation from a Google Sheet](https://github.com/Intuz-production/Automate-QuickBooks-Customer-Sales-Receipt-Creation)
- [Automate AI Upwork proposal generation with Apify, Google Gemini & Sheets](https://github.com/Intuz-production/Upwork-proposal-generation-automation)
- [Automate cold outreach with email personalization using Gemini and Google Sheets](https://github.com/Intuz-production/Personalized-Sales-Outreach-Automation-with-AI)

See all of Intuz's free n8n templates: https://www.intuz.com/n8n-workflow-automation-templates/

## Connect with us

Intuz is a USA-based AI & workflow automation company with 16+ years of experience building custom AI-enabled workflow automations for SMBs and Enterprises, specializing in agentic AI, LLM integrations, and CRM/ERP sync across Healthcare, FinTech, eCommerce, Manufacturing, and Real Estate. Explore 30+ free templates at intuz.com/n8n-workflow-automation-templates or get a custom workflow built at intuz.com/get-started.

* **Website:** https://www.intuz.com/n8n-workflow-automation-templates/
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz/
* **Get Started:** https://n8n.partnerlinks.io/intuz

## For Custom Workflow Automation

[Click here - Get Started](https://www.intuz.com/get-started/)

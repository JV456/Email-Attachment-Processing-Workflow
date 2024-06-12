# Email-Attachment-Processing-Workflow

Welcome to the Email Attachment Processing Workflow repository! This project contains a `Microsoft Power Automate workflow` that helps you automate the tedious task of processing email attachments, specifically invoices. The workflow triggers upon the arrival of a new email, extracts information from invoice attachments, and adds the extracted data into a table for further use.

## How It Works

Here's a step-by-step breakdown of what this workflow does:

#### Trigger: When a new email arrives (V3)
- The workflow starts when a new email lands in your inbox.

#### Condition Check
##### If the Condition is True:
###### Get Attachment:
- Grabs any attachments from the incoming email.
###### Extract Information from Invoices:
- Processes these attachments to pull out specific data, such as invoice number, date, amount, and vendor details.
###### For Each Loop:
- Loops through each piece of extracted information or each attachment.
- For each iteration, it adds a new row into a designated table with the extracted data.
##### If the Condition is False:
- Currently, no actions are defined for this path.

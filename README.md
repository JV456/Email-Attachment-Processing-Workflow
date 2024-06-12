# Email-Attachment-Processing-Workflow

Welcome to the Email Attachment Processing Workflow repository! This project contains a detailed guide on creating a `Microsoft Power Automate workflow` that helps you automate the tedious task of processing email attachments, specifically invoices. The workflow triggers upon the arrival of a new email, extracts information from invoice attachments, and adds the extracted data into a table for further use.

## How It Works

Here's a step-by-step breakdown of what this workflow does:

1. **Trigger: When a new email arrives (V3)**
   - The workflow starts when a new email lands in your inbox.

2. **If the Condition is True:**
   - **Get Attachment:**
     - Grabs any attachments from the incoming email.
   - **Extract Information from Invoices:**
     - Processes these attachments to pull out specific data, such as invoice number, date, amount, and vendor details.
   - **For Each Loop:**
     - Loops through each piece of extracted information or each attachment.
     - **Add a Row into a Table:**
       - For each iteration, it adds a new row into a designated table with the extracted data.

3. **If the Condition is False:**
   - Currently, no actions are defined for this path.


## Requirements

- A Microsoft Power Automate account.
- Access to the email inbox where invoices are received.
- Permissions to create and update tables in your chosen storage solution (like Excel or a SQL database).


## Setting It Up

1. **Configure the Email Trigger:**
   - Set up the trigger to monitor the inbox where you receive your invoices.

2. **Define the Condition:**
   - Specify the condition that should be checked (e.g., email subject, sender, or content).

3. **Attachment Processing:**
   - Make sure the steps for retrieving attachments and extracting information are properly configured. You might need to tweak these based on your specific invoice formats.

4. **Link to Your Data Storage:**
   - Connect the ‘Add a Row into a Table’ step to your storage solution (Excel, SQL database, etc.). Make sure the columns match the data you’re extracting.

5. **Test It Out:**
   - Send a test email with an invoice attachment to see if everything works correctly. Check that the data is being extracted and added to your table as expected.


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## Acknowledgements

- **Microsoft Power Automate Team**: For creating such an intuitive and powerful automation tool that makes workflows like this possible.
- **The GitHub Community**: For providing a platform to share and collaborate on projects.


**By following this README, you should have a good understanding of how to set up and use the workflow. If you run into any issues or have any questions, don't hesitate to reach out!**

**Happy automating! 😊**








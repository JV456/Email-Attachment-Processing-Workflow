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


## Step-by-Step Guide to Creating the Workflow

1. **Start with a Trigger:**
   - In Power Automate, create a new flow and choose "When a new email arrives (V3)" as the trigger.
   
2. **Add a Condition:**
   - After the trigger, add a condition to evaluate specific criteria. This might be checking if the email subject contains certain keywords, or if the sender is a specific person.

3. **Handle Attachments if Condition is True:**
   - **Get Attachments:**
     - Add the action "Get Attachment" to retrieve attachments from the email.
   - **Extract Information:**
     - Use an action like "Extract information from invoices" to process the attachments and extract relevant data. This might involve OCR or a predefined template.
   - **For Each Loop:**
     - Add a "For Each" loop to process each piece of extracted information or each attachment.
     - **Add Data to Table:**
       - Inside the loop, add an action to "Add a row into a table" where you specify the target table and map the extracted data to the table columns.

4. **Handle False Condition:**
   - If the condition is false, you can either leave it empty or add any other necessary actions.

5. **Test and Deploy:**
   - Save and test your workflow. Send a sample email with an invoice to verify that the workflow runs as expected and the data is correctly added to your table.


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## Acknowledgements

- **Microsoft Power Automate Team**: For creating such an intuitive and powerful automation tool that makes workflows like this possible.
- **The GitHub Community**: For providing a platform to share and collaborate on projects.


**By following this README, you should have a good understanding of how to set up and use the workflow. If you run into any issues or have any questions, don't hesitate to reach out!**

**Happy automating! 😊**








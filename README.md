# Automated Email Dispatch System


Mail contact through Gmail with Python & Excel

This project automates sending personalized emails (with attachments) to multiple recipients using Python, Gmail, and an Excel sheet.
________________________________________
Features

•	Sends personalized emails through Gmail SMTP

•	Attaches resume or custom files to each email

•	Marks emails as ‘Sent’ in the same Excel sheet

•	Updates email sent Timestamp in the same Excel sheet

•	Skips emails already marked as sent

•	Supports graceful exit and error handling

________________________________________
📂 Document Uploaded

gmail-mail-merge-python/

├── mail_merge.pynb           # Main script

├── mail_contact_file.xlsx    # Sample Excel file

├── requirements.pdf        # Python package list

├── README.md               # Project documentation

________________________________________
Getting Started

1. Set Your Gmail App Password
   
      Enable 2FA on your Gmail account
   
      Generate an App Password
   
      Use that in your script (never your real Gmail password).
   

2. Import necessary libraries  & Run the code in jupeter Notebook

     import os
     import pandas as pd
     from datetime import datetime  #  Clean import
     import smtplib
     from email.message import EmailMessage

3. Prepared excel file for mail contact.   

   Only rows with Status blank will receive emails and correspnding date and time has been recorded for the mail contact. so that, we can track the mail records and do follow ups in future.
________________________________________
Example Console Output

    Email sent to hr@Xyz.com
    
    Already sent
    
    Attachment not found
 
________________________________________
Security Notes

   •	Avoided uploading real Excel data that contained company mail_id and credentials.
   
   •	Do not share or commit your App Password
   
   •	Better use desktop version of git and use gitignoreI to exclude sensitive or unnecessary files. I have not used desktop version of GitHub due to system limitation.

________________________________________
Future Improvements

   •	HTML formatted email body or multiple email template uses for diffrent purpose
   
   •	Resume failed email attempts
   
   •	Email preview mode before sending
   
   •	GUI support with Tkinter or Streamlit

________________________________________
License

   MIT License. Free to use and modify.
________________________________________
🌐 Author

Mridhul T P

Feel free to fork, improve, or connect on GitHub
________________________________________



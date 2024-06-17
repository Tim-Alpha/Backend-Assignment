# User Data Management API

## Overview
This assignment involves building a set of APIs that manage user data, interact with a database, and handle email notifications. The APIs will handle operations such as uploading user data, viewing user data, backing up the database, and restoring the database.

## Language & Framework
**Language**: PHP
**Framework**: Symfony
**Database**: Mysql

## Requirements

### Data.csv File
Create a `data.csv` file that contains the following columns: `name`, `email`, `username`, `address`, `role`. Include 10 users with a mix of roles (`USER`, `ADMIN`) include at least 2-3 valid email IDs.

Example CSV data:
```
name,email,username,address,role
John Doe,john.doe@example.com,johndoe,123 Main St,USER
Jane Smith,jane.smith@example.com,janesmith,456 Elm St,ADMIN
Michael Johnson,michael.j@example.com,mjohnson,789 Pine St,USER
Emily Davis,emily.d@example.com,emilydavis,101 Oak St,ADMIN
David Brown,david.b@example.com,davidbrown,202 Maple St,USER
Sarah Wilson,sarah.w@example.com,sarahwilson,303 Birch St,USER
Daniel Lee,daniel.l@example.com,daniellee,404 Cedar St,ADMIN
Jessica Martinez,jessica.m@example.com,jessicam,505 Walnut St,USER
Paul Garcia,paul.g@example.com,paulgarcia,606 Ash St,USER
Laura Clark,laura.c@example.com,lauraclark,707 Cherry St,ADMIN
```

### Build APIs
1. **Upload and Store Data API**
   - **Endpoint**: POST /api/upload
   - **Description**: Allows an admin to upload the `data.csv` file.
   - **Functionality**:
     - Parse the `data.csv` file.
     - Save the data into a database.
     - Send an email to each user upon successful storage.
     - Ensure the email sending does not block the API response.

2. **View Data API**
   - **Endpoint**: GET /api/users
   - **Description**: Allows viewing of all user data stored in the database.

3. **Backup Database API**
   - **Endpoint**: GET /api/backup
   - **Description**: Allows an admin to take a backup of the database.
   - **Functionality**:
     - Generate a backup file (e.g., backup.sql).

4. **Restore Database API**
   - **Endpoint**: POST /api/restore
   - **Description**: Allows an admin to restore the database from the backup.sql file.
   - **Functionality**:
     - Restore the database using the backup file.

### Email Sending
- Utilize an email service to send emails to users upon successful data storage.
- Ensure emails are sent asynchronously to avoid blocking the API response.

### Project Completion
- Ensure the project is API-based; non-API projects will not be considered.
- Inform us upon completion to schedule an interview.

### Interview and Contact Information
- The interview will be conducted via Google Meet.
- If you have any queries, you can directly message us on WhatsApp: +91 8278085253.
- Please ensure the project is complete; incomplete projects will be considered as rejected.

# Backend Developer Assignment – User Data Management & Twitter OAuth API  

## **Overview**  
This assignment is designed to evaluate your ability to build robust APIs, interact with a MySQL database, and integrate third-party authentication using Twitter OAuth. The assignment consists of two parts:  To know more about as explore our product [ANDROID](https://play.google.com/store/apps/details?id=com.empowerverse.app) || [iOS](https://apps.apple.com/us/app/empowerverse/id6449552284).

1. **User Data Management API** – Handles CSV uploads, user management, and database backup/restore.  
2. **Twitter OAuth Integration** – Implements authentication using Twitter API in a Symfony-based backend.  

## **Technology Stack**  
- **Language**: PHP  
- **Framework**: Symfony  
- **Database**: MySQL  

---

## **Part 1: User Data Management API**  

### **Data Upload & Management**  
You will work with a CSV file (`data.csv`) containing user details with the following columns:  

- `name`  
- `email`  
- `username`  
- `address`  
- `role` (`USER`, `ADMIN`)  

### **API Endpoints to Implement**  

#### **1. Upload and Store Data API**  
- **Endpoint**: `POST /api/upload`  
- **Description**: Allows an admin to upload the `data.csv` file.  
- **Functionality**:  
  - Parses the `data.csv` file.  
  - Saves the data into a database.  
  - Sends an email notification to each user upon successful storage.  
  - Ensures email sending is handled asynchronously (does not block API response).  

#### **2. View Data API**  
- **Endpoint**: `GET /api/users`  
- **Description**: Returns all stored user data from the database.  

#### **3. Backup Database API**  
- **Endpoint**: `GET /api/backup`  
- **Description**: Allows an admin to take a backup of the database.  
- **Functionality**:  
  - Generates a backup file (e.g., `backup.sql`).  

#### **4. Restore Database API**  
- **Endpoint**: `POST /api/restore`  
- **Description**: Allows an admin to restore the database from `backup.sql`.  
- **Functionality**:  
  - Restores the database using the provided backup file.  

### **Email Notification**  
- Use an email service to send notifications to users upon successful data storage.  
- Ensure emails are sent asynchronously.  

---

## **Part 2: Twitter OAuth Integration**  

Your task is to integrate Twitter authentication into the Symfony backend. This includes:  

- Implementing Twitter login using **OAuth 1.0a**.  
- Storing authenticated user details in MySQL.  
- Providing an API endpoint for the mobile app to initiate authentication.  
- Handling the OAuth callback from Twitter and saving user data.  
- Redirecting users back to the app upon successful authentication.  

### **API Endpoints to Implement**  

#### **1. Initiate Twitter Authentication**  
- **Endpoint**: `GET /auth/twitter`  
- **Description**: Redirects the user to Twitter for authentication.  

#### **2. Handle Twitter Callback**  
- **Endpoint**: `GET /auth/twitter/callback`  
- **Description**: Handles the OAuth response, fetches user details, stores them in MySQL, and redirects the user back to the app.  

---

### **Submission Guidelines**  

To successfully complete the assignment, you must submit the following:  

## **Deliverables**  
1. **Symfony Project** with:  
   - Functional **User Data Management API**.  
   - **Twitter OAuth integration** for authentication.  
2. **Database Migration Script** to store user details.  
3. **README.md File** explaining:  
   - How to set up and run the project.  
   - How to configure Twitter API keys.  
   - Example API responses.  
4. **Postman Collection** for testing API endpoints.  
5. **Video Submission**:  
   - **Introduction Video (30-40 sec)**:  
     - Show your face in the video.  
     - Provide a brief introduction about yourself.  
     - Explain what you built in this assignment.  
   - **Screen Recording**:  
     - Run the APIs using **Postman** and show the working endpoints.  
     - Demonstrate how Twitter authentication works.  
     - Show how data is stored and retrieved from the database.  

---

## **Submission Guidelines**  
- Submit your assignment as a **GitHub repository**.  
- Include all files, including the **README.md** and **Postman collection**.  
- Upload the **videos** to Google Drive or YouTube (unlisted) and provide the link in your submission.  
- Notify us upon completion via our **Telegram group**.  

---

### **Important Notes**  
✅ Ensure that all APIs work correctly before submission.  
✅ Incomplete submissions will not be considered.  
✅ The video submission is mandatory.  

Good luck! 🚀

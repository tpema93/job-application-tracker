# **Job Application Tracker - Chrome Extension**

The **Job Application Tracker** is a Chrome extension built to simplify the job application process by allowing users to easily track their job applications across multiple platforms. It offers a streamlined experience for saving job postings, adding personalized notes, and tracking the application progress from submission to final decision.

## **Features**
- **Save Job Postings**: Save job listings directly from websites while browsing.
- **Track Application Status**: Monitor each stage of the job application process, from submission to offer or rejection.
- **Add Personalized Notes**: Keep track of key details such as interview dates, notes, tasks, or important deadlines.
- **Organized Dashboard**: View the status of applications in one place with clear and concise details.
- **Browser Integration**: Access your saved job applications and notes right from the browser without leaving the job search website.

## **Tech Stack**
- **React**: Used for building the UI and managing dynamic content within the Chrome extension.
- **Node.js & Express**: Backend services to handle user requests and manage job data.
- **MongoDB**: NoSQL database to store job application data securely.
- **AWS Lambda**: Serverless architecture for backend processing.
- **AWS S3**: Cloud storage for files and user-generated content.

## **Installation**

To install and run this project on your local machine, follow these steps:

### **Prerequisites**
- **Node.js**: Make sure you have [Node.js](https://nodejs.org/) installed on your system.
- **MongoDB Atlas**: Set up a free MongoDB Atlas account and cluster [here](https://www.mongodb.com/cloud/atlas).
- **AWS Account**: Create a free-tier AWS account for Lambda and S3 services [here](https://aws.amazon.com/free/).
- **Git**: Ensure you have Git installed to manage version control.
- **Code Editor**: You can use any IDE of your preference (e.g., VSCode, Sublime Text, IntelliJ, etc.).

### **Clone the Repository**
1. Visit the GitHub repository page.
2. Click on the **Code** button and copy the URL.
3. Open your preferred IDE and clone the repository from the URL.

### **Install Dependencies**

Navigate to the cloned repository and install the necessary packages for both frontend and backend.

```bash
# Frontend (React)
cd chrome-extension
npm install

# Backend (Node.js + Express)
cd backend
npm install
```

### **Run the Application Locally**

**Running the Frontend**

To start the React frontend, go to the chrome-extension folder and run:

```bash 
npm start
```

This will start the frontend server and open the application in your browser.


**Running the Backend**

To start the Node.js/Express backend, go to the backend folder and run:

```bash
npm run dev
```

Ensure your MongoDB connection string is correctly set up in your server.js file for the database to function properly.

## **Adding the Extension to Chrome**

1.	In Chrome, go to chrome://extensions/.
2.	Enable Developer Mode (top right).
3.	Click Load unpacked and select the build folder from your React project (chrome-extension/build).
4.	The extension will now be loaded and visible in your browser.

## **AWS Setup (Optional)**

To deploy the backend to AWS Lambda and use S3 for file storage:

1.	Set up a Lambda function in AWS and upload the backend code (you can zip the backend folder).
2.	Configure API Gateway to interact with Lambda functions.
3.	Set up an S3 bucket for storing any files related to the application (if needed).

Refer to the [AWS Documentation](https://docs.aws.amazon.com/) for detailed steps.

## **Usage**

1.	Once the Chrome extension is loaded, click on the extension icon to open it.
2.	Start saving job applications by entering details such as the job title, company, application status, and any additional notes.
3.	You can edit or update the status of the applications as you progress through the hiring process.
4.	The extension saves the data locally and securely in your MongoDB database.

## Roadmap

Here are some planned improvements for future versions:

- Browser Sync: Sync job application data across multiple devices.
- Customizable Application Stages: Allow users to define their own stages (e.g., phone screen, technical interview).
- Job Alerts: Notify users when they have not updated a job application after a specific time period.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1.	Fork the repository.
2.	Create a new branch:
    ```bash
    git checkout -b name-new-branch
    ```
3.	Make your changes and commit:
    ```bash
    git commit -m "your commit message"
    ```
4.	Push to your branch:
    ```bash
    git push origin name-new-branch
    ```
5.	Open a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

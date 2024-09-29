Desktop Agent Application


Team Members:

Virender Kumar
Vishwakarma Singh
Vivek Kumar
Wazida Tabbasum
Yogesh Devtulla


Application Report File
Report File: https://docs.google.com/document/d/1izG0VkWIr1CWLUJ2wWcI2BcSDLHbiufjMzN4nHTamRo/edit?usp=sharing

Application ZIP File
ZIP File: https://drive.google.com/file/d/1w2UaA7fL2JVbp20mffkrIuY3ZSzwMhNs/view?usp=sharing

Technologies Used
1. Python
Core Language: Python will be the primary language for developing the desktop agent application.
Libraries:
pyautogui: For capturing screenshots.
pynput: For monitoring keyboard and mouse activity.
asyncio: For handling asynchronous tasks like periodic screenshot capture and data uploads.
requests: For sending HTTP requests to upload data to cloud services.
pymongo: For interaction with MongoDB if local storage is required before upload.
PIL (Pillow): For image processing tasks like blurring screenshots.
watchdog: For monitoring file system changes or configuration updates.
2. Amazon Web Services (AWS)
Amazon S3: For storing and managing uploaded screenshots and activity logs.
AWS Lambda: For handling the backend processing of uploads, such as file storage or data transformation.
AWS IAM: For managing permissions and roles required for secure interaction with S3 and Lambda.
Boto3: AWS SDK for Python to interact with S3 for uploading files.
3. FastAPI
Used for creating an API that handles configuration updates from a web application, allowing the agent to fetch new configurations (e.g., interval times, screenshot settings).
4. MongoDB
A NoSQL database used for temporarily storing captured data locally (e.g., activity logs and screenshots) before uploading to cloud storage.
5. React.js
For the front-end of the web application where users can configure the agent settings (e.g., screenshot intervals, whether screenshots should be blurred, etc.).
6. Encryption & Security
PyCryptodome: A library for implementing encryption to ensure that data is securely uploaded to S3.
7. System-level Tools
Time Zone Management: Utilizing Python's tzlocal or pytz libraries for detecting and managing time zone changes.
8. Testing and Debugging Tools
Pytest: For unit testing the different components of the application.
Logging: Using Python's logging module for error handling, activity tracking, and debugging.
9. Deployment & Packaging
PyInstaller: To package the Python script as a standalone executable that can run on users' desktops without requiring them to install Python.
10. Error Handling
Retry Mechanisms: For retrying failed uploads due to connectivity issues.
Queueing: To handle data that couldn’t be uploaded immediately, ensuring it's uploaded once the network is restored.
Application Key Features
Different dashboards for client and admin
Manage user total active time
Manage user total inactive time
Take screenshot manually and automatically
Store screenshots in AWS S3 bucket
Locally store screenshots in queue if network related problem arise
Track Mouse and Keyboard Movements
Gives warning if user become inactive for more than 30 seconds
Track and store different application usage of client on device and showcase on admin portal
Track battery status
Show current time according to location
And some more......
Important Instructions To Run
Step 1- git clone https://github.com/Vivek833855/Python-based-Desktop-Agent-Application-Group-17/tree/main/VinoveProject-main

step 2 ->For Frontend

cd client
npm i
npm start

step 3->For backend

cd server
pip install "all dependencies"
python main.py

ALWAYS STARTS SERVER FIRST
ID , PASSWORD ->
id- client , pass- 1111
id- admin , pass- 0000
Dependencies To Install
Backent Dependencies
1.motor
2.pyautogui
3.requests
4.pymongo
5.pygetwindow
6.fastapi
7.pydantic
Frontend Dependencies
1.axios
2.react-router-dom
Repository Information
Commit History
This repository includes a complete commit history that reflects the development process of the project. All changes and updates made during the development phase are documented in the commit history, providing a detailed record of the project's evolution.

For a more comprehensive understanding of the development process, you can review the commit messages and associated changes.

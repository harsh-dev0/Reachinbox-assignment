ReachInbox Web Application
This project is a functional web application built using React, based on the provided designs and APIs. The application implements various features like user login, data fetching, keyboard shortcuts, custom text editor functionalities, reply functionality, and support for both light and dark modes.

Features
Login Page

Users can log in using the provided design.
After logging in, users are redirected to the onebox screen.
Onebox Screen

Fetch and display data in onebox using API integration.
Implemented API endpoints:
/onebox/list (GET)
/onebox/:thread_id (GET)
/onebox/:thread_id (DELETE)
Keyboard shortcuts:
Press D to delete a thread.
Press R to open the reply box.
Custom Text Editor

Added custom buttons like “SAVE” and “Variables” to the text editor.
Reply Functionality

Clicking on the "Send" button will send a reply using the following API endpoint:
POST /reply/:thread_id
Request body format:
json
Copy code
{
  "from": "email",
  "to": "email",
  "subject": "",
  "body": "<html></html>"
}
Light and Dark Mode

The application supports both light and dark themes, allowing users to switch between modes.
Getting Started
Prerequisites
Node.js (v14.x or later)
npm or yarn
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/your-repository.git
cd your-repository
Install the dependencies:

bash
Copy code
npm install
# or
yarn install
Running the Application
Start the development server:

bash
Copy code
npm start
# or
yarn start
Open your browser and navigate to:

arduino
Copy code
http://localhost:3000
Building for Production
To create an optimized production build:

bash
Copy code
npm run build
# or
yarn build
The production build will be located in the build/ directory.

Deployment
The project can be deployed on platforms like Vercel, Netlify, or any other static site hosting service.

Deployed Link: (Please provide the deployed link here once available)

API Documentation
You can refer to the provided API documentation here for more details on API endpoints and usage.

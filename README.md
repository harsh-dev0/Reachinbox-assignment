# ReachInbox Web Application

This project is a functional web application built using React, based on the provided designs and APIs. The application implements various features like user login, data fetching, keyboard shortcuts, custom text editor functionalities, reply functionality, and support for both light and dark modes.

## Features

1. **Login Page**
   - Users can log in using the provided design.
   - After logging in, users are redirected to the onebox screen.

2. **Onebox Screen**
   - Fetch and display data in onebox using API integration.
   - Implemented API endpoints:
     - `/onebox/list` (GET)
     - `/onebox/:thread_id` (GET)
     - `/onebox/:thread_id` (DELETE)
   - Keyboard shortcuts:
     - Press `D` to delete a thread.
     - Press `R` to open the reply box.

3. **Custom Text Editor**
   - Added custom buttons like “SAVE” and “Variables” to the text editor.

4. **Reply Functionality**
   - Clicking on the "Send" button will send a reply using the following API endpoint:
     - `POST /reply/:thread_id`
     - Request body format:
       ```json
       {
         "from": "email",
         "to": "email",
         "subject": "",
         "body": "<html></html>"
       }
       ```

5. **Light and Dark Mode**
   - The application supports both light and dark themes, allowing users to switch between modes.

## Getting Started

### Prerequisites

- Node.js (v14.x or later)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
   ```

2. Install the dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

### Running the Application

1. Start the development server:

   ```bash
   npm start
   # or
   yarn start
   ```

2. Open your browser and navigate to:

   ```
   http://localhost:3000
   ```

### Building for Production

To create an optimized production build:

```bash
npm run build
# or
yarn build
```

The production build will be located in the `build/` directory.

## Deployment

The project can be deployed on platforms like Vercel, Netlify, or any other static site hosting service.

**Deployed Link**: *(Please provide the deployed link here once available)*

## API Documentation

You can refer to the provided API documentation [here](https://documenter.getpostman.com/view/30630244/2sA2rCTMKr#433eb613-e405-4239-9e2d-f20485b31b27) for more details on API endpoints and usage.

## Contributing

Feel free to fork the project, create a new branch, and submit a pull request for any enhancements or bug fixes.

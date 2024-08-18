# React Firebase Chat Room

This project is a simple chat room application built using React and Firebase. It allows users to sign in with Google, send messages in real-time, and view messages from other users. The application leverages Firebase Authentication, Firestore, and Firebase Analytics.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Screenshots](#screenshots)
- [Setup and Installation](#setup-and-installation)
- [How to Use](#how-to-use)
- [Deployment](#deployment)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [License](#license)

## Features

- **Google Authentication:** Users can sign in using their Google accounts.
- **Real-Time Messaging:** Messages are updated in real-time using Firestore.
- **User-Friendly Interface:** The UI is simple, clean, and easy to use.
- **Community Guidelines:** Clear guidelines are provided to ensure a safe and respectful environment.
- **Responsive Design:** The application is designed to work well on various screen sizes.

## Technologies Used

- **React:** Front-end JavaScript library for building user interfaces.
- **Firebase Authentication:** Manages user authentication via Google.
- **Firestore:** Cloud-hosted NoSQL database that stores chat messages.
- **Firebase Analytics:** Collects usage data to help improve the app.
- **CSS:** Custom styles for the application.

## Screenshots

<img src="./screenshots/Screenshot 2024-08-18 063822.png" width="320px" />

<img src="./screenshots/Screenshot 2024-08-18 064014.png" width="320px" />

## Setup and Installation

To set up and run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/rishi-vakharia/react-firebase-chat-room.git
   cd react-firebase-chat-room
   ```

2. **Install dependencies:**
   Make sure you have Node.js installed. Then run:
   ```bash
   npm install
   ```

3. **Firebase Setup:**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Enable **Google Authentication** in the Firebase Authentication settings.
   - Set up **Firestore** in your Firebase project.
   - Create a `.env` file in the root of your project and add your Firebase configuration:
     ```env
     REACT_APP_API_KEY=your-api-key
     REACT_APP_AUTH_DOMAIN=your-auth-domain
     REACT_APP_PROJECT_ID=your-project-id
     REACT_APP_STORAGE_BUCKET=your-storage-bucket
     REACT_APP_MESSAGING_SENDER_ID=your-messaging-sender-id
     REACT_APP_APP_ID=your-app-id
     REACT_APP_MEASUREMENT_ID=your-measurement-id
     ```

4. **Start the development server:**
   ```bash
   npm start
   ```
   The app will be available at `http://localhost:3000`.

## How to Use

1. **Sign In:**
   - Click on "Sign in with Google" to authenticate yourself.
   
2. **Chat:**
   - Type a message in the input box and press Enter or click the send button (🕊️) to send it.
   - View your message and other users' messages in real-time.

3. **Sign Out:**
   - Click on the "Sign Out" button in the header to log out.

## Deployment

You can deploy the site using the `build` folder and the `serve` command.

1. **Build the project:**

   ```bash
   npm run build
   ```

   This will create a `build` folder with a production-ready version of your app.

2. **Serve the app locally:**
   Install `serve` globally if you haven't already:

   ```bash
   npm install -g serve
   ```

   Then, serve the `build` folder:

   ```bash
   serve -s build
   ```

   Your app will be available at `http://localhost:5000`.

3. **Deploy to a hosting service:**

   - You can deploy the contents of the `build` folder to any static site hosting service, such as GitHub Pages, Vercel, or Netlify.

## Project Structure

```
/src         
  |-- App.css              # CSS file for styling the application
  |-- index.js             # Entry point for React
  |-- App.js			  # Main application component
        |-- ChatRoom.js    # Chat room component handling messages
        |-- ChatMessage.js # Chat message component for displaying individual messages
        |-- SignIn.js      # Sign-in component for Google authentication
        |-- SignOut.js     # Sign-out component for logging out
```

## Future Improvements

- **Add Private Messaging:** Implement private chat rooms or direct messaging between users.
- **Enhanced User Profiles:** Allow users to set display names or profile pictures.
- **Message Reactions:** Enable users to react to messages with emojis.
- **Moderation Tools:** Implement moderation features to enforce community guidelines.


## References

https://www.youtube.com/watch?v=zQyrwxMPm88


# Pinterest Clone

## Overview
This is a full-stack Pinterest clone web application built using modern web technologies. The project is based on a YouTube tutorial that guides you through the development process, focusing on user authentication, image uploads, and interactive UI components.

## Features
- **User Authentication**: Sign up and log in using Google authentication via NextAuth.js and Firebase.
- **Pin Creation**: Upload images or videos, add descriptions, and save them as pins.
- **Pin Display**: View pins in a masonry-style layout for a visually appealing user experience.
- **Pin Details**: Click on a pin to see an enlarged view along with its description and creator information.
- **User Profiles**: Each user has a profile page displaying their created and saved pins.
- **Image Uploads**: Store images securely in Firebase Storage.
- **Data Management**: Store user details and pin information in Firestore.
- **Responsive Design**: Optimized for both desktop and mobile devices using Tailwind CSS.

## Technologies Used
- **Next.js 13**: A React framework with server-side rendering and SEO optimizations.
- **Tailwind CSS**: Utility-first CSS framework for efficient styling.
- **Firebase**:
  - Firestore: Database for storing user and pin data.
  - Firebase Storage: Secure storage for images and videos.
  - Firebase Authentication: Handles user login and authentication.
- **NextAuth.js**: Authentication library for Next.js applications.
- **React Icons**: Collection of ready-to-use icons for UI enhancement.

## Installation & Setup

### Prerequisites
- Node.js and npm installed on your machine
- Firebase account setup
- Google Cloud project for authentication (OAuth credentials)

### Steps to Run the Project Locally
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/pinterest-clone.git
   cd pinterest-clone
   ```
2. **Install Dependencies**
   ```sh
   npm install
   ```
3. **Set Up Firebase**
   - Create a new Firebase project.
   - Enable Firestore and Firebase Storage.
   - Set up Firebase Authentication with Google Sign-In.
   - Retrieve Firebase config credentials.
4. **Set Up Environment Variables**
   Create a `.env.local` file and add the required credentials:
   ```env
   NEXT_PUBLIC_FIREBASE_API_KEY=your-api-key
   NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your-auth-domain
   NEXT_PUBLIC_FIREBASE_PROJECT_ID=your-project-id
   NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your-storage-bucket
   NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your-sender-id
   NEXT_PUBLIC_FIREBASE_APP_ID=your-app-id
   GOOGLE_CLIENT_ID=your-google-client-id
   GOOGLE_CLIENT_SECRET=your-google-client-secret
   NEXTAUTH_URL=http://localhost:3000
   ```
5. **Run the Development Server**
   ```sh
   npm run dev
   ```
   The application should now be running at `http://localhost:3000`.

## Project Structure
```
📦 pinterest-clone
├── 📂 components       # Reusable React components
├── 📂 pages            # Next.js pages (home, login, profile, etc.)
├── 📂 styles           # Tailwind CSS styles
├── 📂 utils            # Helper functions and Firebase configurations
├── .env.local          # Environment variables (not included in repo)
├── next.config.js      # Next.js configuration
├── package.json        # Project dependencies
└── README.md           # Project documentation
```


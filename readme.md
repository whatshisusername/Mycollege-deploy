# MyCollege

MyCollege is a comprehensive web application designed to cater to the essential needs of college students and professors. The platform focuses on two core areas: academics and extracurricular activities. It provides tools for managing courses, events, notifications, and hall tickets, creating a centralized hub for college-related activities.

---

## Tech Stack

- **Frontend**: `React.js`
- **Backend**: `Express.js` 
- **Database**: `MongoDB`  
- **Authentication**: `JWT (JSON Web Tokens)`  
  - Access and refresh tokens for secure authentication and session management.
- **Encryption**:
  - Password encryption using `bcrypt`.  
- **File Handling**:  
  - `Multer` for file uploads.  
  - `Cloudinary` for secure cloud storage of files.  
- **PDF Generation**:  
  - `jspdf` to convert HTML content into PDF for hall tickets.  
- **Secure Storage**:  
  - Used `securelocalstorage` to keep users logged in even after closing the browser.  
- **AI Description Generation**:  
  - `Gemini API` for generating event descriptions.  

---

## Features

### For Students
#### **Profile Management**
- Sign up, log in, and log out.
- Update profile details, including profile picture.

#### **Courses**
- Browse all courses with search filters.
- Join or leave courses.
- View joined courses under the "My Courses" tab.
- Access course details and download notes (available after joining a course).
- View and manage course participants.

#### **Hall Ticket**
- Automatically generated hall ticket for each student.
- View and download hall ticket in PDF format.

#### **Events**
- View events happening today, past events, and future events.
- Access details of all events under "All Events."
- Organizers can add/delete events with AI-generated descriptions, images, and more.

#### **Notifications**
- Receive notifications for updates related to courses and events.

---

### For Professors
#### **Profile Management**
- Create, update, and manage personal profiles.

#### **Courses**
- Browse and manage their courses.
- Add, edit, and delete courses.
- Remove students from courses.
- Upload and manage course notes.

#### **Events**
- View all college events under the "Events" tab.
- Add/delete events for their activities, such as tests or workshops.

#### **Notifications**
- Stay updated with notifications related to courses and events.

---

## Screenshots

### Homepage  
![Homepage Screenshot](link-to-homepage-screenshot)  

### Profile Management  
![Profile Screenshot](link-to-profile-screenshot)  

### Courses  
![Courses Screenshot](link-to-courses-screenshot)  

### Events  
![Events Screenshot](link-to-events-screenshot)  

---

## Deployed Web App

Visit the live application here(open with Microsoft Edge.): [MyCollege Web App](https://mycollege-final-dp.vercel.app/)

---

## Key Practices and Implementation Details

1. **Authentication and Authorization**
   - Implemented JWT for user authentication and role-based access control.
   - Passwords are encrypted using `bcrypt` for enhanced security.
   - Secure tokens stored using `securelocalstorage` to maintain user sessions across browser tabs and closures.

2. **File Handling**
   - Files are uploaded using `multer` and temporarily stored locally.
   - Files are then uploaded to Cloudinary, and the local files are deleted after successful upload.

3. **Environment Variables**
   - Sensitive information (e.g., database credentials, API keys) is stored in an `.env` file for security.

4. **Scalable Backend Architecture**
   - Structured codebase with controllers, models, routes, and middlewares for maintainability and scalability.

5. **Performance and Session Management**
   - Used access tokens and refresh tokens instead of session IDs for improved performance and session security.
   - Securelocalstorage ensures persistent user login without compromising security.

---



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
   - 

---


## Screenshots

### Homepage  
![home](https://github.com/user-attachments/assets/663c3ff1-f11e-41ef-896b-8bc9227b9263)  

### Profile Management  
**  **![login ](https://github.com/user-attachments/assets/8e8b346f-534d-47a4-bcb1-b3eb2e9e90a2)
**  **![ssign](https://github.com/user-attachments/assets/1c2397be-c2b5-4699-a667-8d76287d7263)
**  **![tsign](https://github.com/user-attachments/assets/7fa49e47-59aa-4c1a-a664-350a3892e5e1)
**  **![profile](https://github.com/user-attachments/assets/e5b67448-daf8-403d-a956-4f87187867f2)

![pp](https://github.com/user-attachments/assets/5ab76848-d4c5-47c6-b1a7-4e84410c99ee)

### Courses  
![mycourses](https://github.com/user-attachments/assets/577fe14c-8343-461a-b453-8cb453f2c35b)
![course](https://github.com/user-attachments/assets/4202d8ca-c084-4ff5-ae52-2196c0834a0b)
![coursepage'](https://github.com/user-attachments/assets/8fe37b46-51c4-44d7-a76b-a3a5716bfc3d)
![addcourse](https://github.com/user-attachments/assets/3a4fe68b-e871-4c90-86b9-1039753c18ba)
![tcpage](https://github.com/user-attachments/assets/9f003a58-26ec-4e48-aa3b-8929a3187ec7)


### Events 
![events](https://github.com/user-attachments/assets/0e9163d6-3503-490a-b58c-1cf968b5a8c9)
![addevent](https://github.com/user-attachments/assets/8832f5a0-a924-423c-83fa-af8fa7c7ce13)
![notification](https://github.com/user-attachments/assets/74c8015a-d0c2-4d7b-9156-0b2bbf4f6c24)


---

## Deployed Web App

Visit the live application here(open with Microsoft Edge.): [MyCollege Web App](https://mycollege-final-dp.vercel.app/)

---


# BookMyDoc-Prescripto
BookMyDoc-Prescripto is a robust platform that allows patients to manage medical appointments, doctors to update availability, and administrators to oversee all platform activity efficiently. This Minimum Viable Product (MVP) features three distinct interfaces for users (patients), doctors, and administrators, ensuring seamless management of appointments, payments, and user profiles.

## Live Demo
- **User**: [Prescripto - Live - Frontend](https://bookmydoc-frontend.onrender.com/)
- **Admin Panel**: [Prescripto - Live - admin](https://bookmydoc-admin.onrender.com/)
  
## Table of Contents
- [Installation](#installation)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Usage](#usage)

## Installation

To run the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/axdityax/BookMyDoc-Prescripto
   cd BookMyDoc-Prescripto
   ```

2. **Set up the Backend**:
   - Navigate to the backend directory:
     ```bash
     cd backend
     ```
   - Install the necessary dependencies:
     ```bash
     npm install
     ```
   - In `.env` file in the `backend` directory, add the following environment variables (replace the placeholders with your actual values):
     ```plaintext
     CURRENCY = "INR"
     JWT_SECRET="testxupdate"
     ADMIN_EMAIL = "admin@bookmydoc.com"
     ADMIN_PASSWORD = "admin123"
     MONGODB_URI = ""
     CLOUDINARY_NAME = ""
     CLOUDINARY_API_KEY = ""
     CLOUDINARY_SECRET_KEY = ""
     RAZORPAY_KEY_ID = ""
     RAZORPAY_KEY_SECRET = ""
     STRIPE_SECRET_KEY=""
     ```
   - Start the backend server:
     ```bash
     npm run server
     ```
   - Ensure the backend server is running successfully before proceeding to the frontend.

3. **Set up the Frontend**:
   - Navigate to the frontend directory:
     ```bash
     cd ../frontend
     ```
   - Install the necessary dependencies:
     ```bash
     npm install
     ```
   - Start the frontend application:
     ```bash
     npm run dev
     ```

4. **Set up the Admin**:
   - Navigate to the frontend directory:
     ```bash
     cd ../Admin
     ```
   - Install the necessary dependencies:
     ```bash
     npm install
     ```
   - Start the Admin application:
     ```bash
     npm run dev
     ```

5. **Testing the Application**:
   - Once the backend, frontend, and admin panel are running, test the platform by logging in as a user, doctor, or admin.
   - Make appointments as a user, manage appointments as a doctor, and monitor all activity through the admin dashboard.

## Features

### Admin Dashboard
- **Doctor Management**: Add, view, and manage doctor details.
- **Appointment Management**: View and cancel patient appointments.
- **Analytics**: Monitor platform activity and statistics through the admin dashboard.
  
### Doctor Functionality
- **Login**: Secure login for doctors.
- **Manage Appointments**: View upcoming appointments, cancel or complete appointments.
- **Profile Management**: Update doctor profile and availability status.
- **Dashboard**: Access doctor-specific insights and data.

### User (Patient) Functionality
- **User Registration & Login**: Secure registration and login process.
- **Profile Management**: Users can update their profile details and upload a profile picture.
- **Book Appointments**: Users can search for doctors, book appointments, and view booking history.
- **Payment Integration**: Integrated with Razorpay and Stripe for secure online payments.
- **Track Appointments**: Users can track their appointment status and cancel appointments if necessary.

### Frontend
- **Home Page**: Overview of the platform and its purpose.
- **User Login**: Secure login system with JWT for session management.
- **Submission Process**:
  - Add address, select center, and choose clothes in a stepwise manner.
  - Review submission details before final submission.
- **Track Page**: 
  - Track user submissions.
  - Sort functionality and search by apparel type.
- **FAQ Page**: Answers to common questions.
- **Contact Page**: Contact information for support and inquiries.

## Technologies Used
- **Frontend**: 
  - React.js (for building the user interface)
  - Redux (for state management)
  - Axios (for making API calls)
  - Tailwind CSS (for styling)

- **Backend**: 
  - Node.js (for backend development)
  - Express.js (for building the API)
  - MongoDB (for database management)
  - JWT (for user authentication)

- **Payments**: 
  - Razorpay (payment gateway integration)
  - Stripe (alternative payment gateway)

## Usage
### For Users (Patients):
1. **Register an Account**:  
   Navigate to the user interface and register a new account by providing your name, email, and password.

2. **Login**:  
   After registration, log in with your email and password.
3. **Update Profile**:  
   Access your profile page to update your personal information and upload a profile picture if desired.
4. **Search for Doctors**:  
   Use the search functionality to find doctors based on specialization or availability.
5. **Book an Appointment**:  
   Select a doctor, choose a date and time, and book an appointment. You will be redirected to the payment page.
6. **Make a Payment**:  
   Choose your preferred payment method (Razorpay or Stripe), make the payment, and confirm your appointment.
7. **Track Appointments**:  
   View your upcoming and past appointments in the "Appointments" section. You can also cancel any appointment if necessary.
8. **Logout**:  
   Once done, log out from the system for security.

---

### For Doctors:
1. **Login**:  
   Use your registered credentials to log in to the doctor panel.
2. **Manage Appointments**:  
   View all your upcoming appointments. You can mark them as completed or cancel them if needed.
3. **Update Profile**:  
   Update your profile details including specialization, and availability status. You can also upload a profile picture.
4. **Update Availability**:  
   Toggle your availability status to let users know when you're available for appointments.
5. **Access Dashboard**:  
   View your personalized dashboard to see appointments, analytics, and other key details.
6. **Logout**:  
   Log out of the system when finished for security.
---

### For Admins:
1. **Login**:  
   Access the admin panel by logging in with your admin credentials.
2. **Manage Doctors**:  
   Add new doctors, view the list of all registered doctors, and manage their details.
3. **Manage Appointments**:  
   View all the appointments booked on the platform, including user and doctor details. You can also cancel appointments if necessary.
4. **Analytics Dashboard**:  
   Monitor overall platform activity including doctor performance, user activity, and appointment statistics through the analytics dashboard.
5. **Logout**:  
   Log out of the admin panel after you're done.

# DoctorScheduler

A comprehensive web-based doctor appointment scheduling system built with Node.js, Express, and MongoDB. This application allows patients to book appointments with doctors while providing doctors with tools to manage their schedules and availability.

## 🚀 Features

### For Patients
- **User Registration & Authentication**: Secure signup and login system
- **Doctor Search & Discovery**: Browse available doctors by specialty, location, or name
- **Appointment Booking**: Schedule appointments with preferred doctors
- **Appointment Management**: View, reschedule, or cancel upcoming appointments
- **Medical History**: Access personal appointment history and medical records

### For Doctors
- **Professional Profile Management**: Create and update professional profiles
- **Schedule Management**: Set availability, working hours, and time slots
- **Appointment Overview**: View and manage patient appointments
- **Patient Records**: Access patient information and appointment history

### For Administrators
- **User Management**: Manage patient and doctor accounts
- **System Oversight**: Monitor appointments and system usage
- **Data Analytics**: View scheduling statistics and system metrics

## 🛠 Tech Stack

- **Backend**: Node.js with Express.js framework
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT (JSON Web Tokens)
- **Frontend**: React Js
- **Styling**: Bootstrap for responsive design
- **Session Management**: Express sessions

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (v4.4 or higher)
- [Git](https://git-scm.com/)

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Om-dharra/DoctorScheduler.git
   cd DoctorScheduler
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory and add the following:
   ```env
   PORT=3000
   MONGODB_URI=mongodb://localhost:27017/doctorscheduler
   JWT_SECRET=your_jwt_secret_key
   SESSION_SECRET=your_session_secret_key
   ```

4. **Start MongoDB**
   Make sure your MongoDB service is running on your system.

5. **Run the application**
   ```bash
   npm start
   ```

6. **Access the application**
   Open your browser and navigate to `http://localhost:3000`

## 📁 Project Structure

```
DoctorScheduler/
├── config/
│   └── database.js          # Database configuration
├── controllers/
│   ├── authController.js    # Authentication logic
│   ├── appointmentController.js # Appointment management
│   ├── doctorController.js  # Doctor-related operations
│   └── patientController.js # Patient-related operations
├── middleware/
│   ├── auth.js             # Authentication middleware
│   └── validation.js       # Input validation middleware
├── models/
│   ├── User.js             # User model (patients & doctors)
│   ├── Appointment.js      # Appointment model
│   └── Schedule.js         # Doctor schedule model
├── routes/
│   ├── auth.js             # Authentication routes
│   ├── appointments.js     # Appointment routes
│   ├── doctors.js          # Doctor routes
│   └── patients.js         # Patient routes
├── public/
│   ├── css/                # Stylesheets
│   ├── js/                 # Client-side JavaScript
│   └── images/             # Static images
├── views/
│   ├── layouts/            # Template layouts
│   ├── partials/           # Reusable template components
│   └── pages/              # Main application pages
├── utils/
│   └── helpers.js          # Utility functions
├── app.js                  # Main application file
├── package.json            # Dependencies and scripts
└── README.md              # Project documentation
```

## 🔑 Key Features Breakdown

### Authentication System
- Secure user registration and login
- Role-based access control (Patient, Doctor, Admin)
- JWT token-based authentication
- Password encryption using bcrypt

### Appointment Management
- Real-time availability checking
- Conflict prevention for double bookings
- Automated appointment reminders
- Flexible rescheduling options

### Doctor Profiles
- Comprehensive professional profiles
- Specialty and qualification management
- Availability calendar integration
- Patient review and rating system

### Administrative Dashboard
- User management interface
- Appointment analytics and reporting
- System configuration options
- Data export capabilities

## 🧪 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/profile` - Get user profile

### Appointments
- `GET /api/appointments` - Get user appointments
- `POST /api/appointments` - Create new appointment
- `PUT /api/appointments/:id` - Update appointment
- `DELETE /api/appointments/:id` - Cancel appointment

### Doctors
- `GET /api/doctors` - Get all doctors
- `GET /api/doctors/:id` - Get specific doctor
- `PUT /api/doctors/:id/schedule` - Update doctor schedule
- `GET /api/doctors/:id/availability` - Get doctor availability

## 🚀 Usage

### For Patients
1. Register for a new account or login
2. Browse available doctors by specialty or location
3. Select a doctor and view their available time slots
4. Book an appointment for your preferred time
5. Manage your appointments from the dashboard

### For Doctors
1. Complete your professional profile setup
2. Set your working hours and availability
3. Manage incoming appointment requests
4. View patient information and appointment history
5. Update your schedule as needed

## 🤝 Contributing

We welcome contributions to improve DoctorScheduler! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes and commit**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Development Guidelines
- Follow existing code style and conventions
- Write clear, descriptive commit messages
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

## 🔮 Future Enhancements

- **Real-time Notifications**: WebSocket integration for instant updates
- **Payment Integration**: Online payment processing for appointments
- **Telemedicine Support**: Video consultation capabilities
- **Mobile App**: React Native mobile application
- **AI-Powered Scheduling**: Smart appointment recommendations
- **Multi-language Support**: Internationalization features



## 👥 Authors

- **Om Dharra** - *Initial work* - [Om-dharra](https://github.com/Om-dharra)

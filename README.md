# Disaster Preparedness Education Platform

A comprehensive full-stack application for disaster preparedness education in schools, featuring interactive learning modules, virtual drills, real-time emergency alerts, and comprehensive progress tracking.

## 🌟 Features

### 🎓 Learning Management
- **Interactive Modules**: Comprehensive disaster preparedness content
- **Virtual Drills**: Real-time emergency response simulations
- **Progress Tracking**: Detailed analytics and achievement system
- **Quiz System**: Interactive assessments with immediate feedback

### 🚨 Emergency Management
- **Real-time Alerts**: Instant emergency notifications
- **Emergency Contacts**: Quick access to emergency services
- **Evacuation Points**: Interactive evacuation route mapping
- **Broadcast System**: Mass communication during emergencies

### 👥 User Management
- **Role-based Access**: Student, Teacher, and Admin roles
- **User Profiles**: Comprehensive user management
- **Class Management**: Teacher oversight of student progress
- **Leaderboards**: Gamified learning experience

### 📊 Analytics & Reporting
- **Admin Dashboard**: Comprehensive management tools
- **Progress Analytics**: Detailed performance metrics
- **Class Performance**: Teacher insights into student progress
- **Real-time Statistics**: Live platform usage data

## 🛠️ Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development
- **Tailwind CSS** for styling
- **Radix UI** for accessible components
- **Lucide React** for icons

### Backend
- **Node.js** with Express.js
- **MongoDB** with Mongoose
- **Socket.io** for real-time features
- **JWT** for authentication
- **Express-validator** for input validation

## 🚀 Quick Start

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or cloud)
- npm or yarn

### 1. Clone the Repository

```bash
git clone <repository-url>
cd disaster-preparedness-platform
```

### 2. Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Copy environment file
cp config.env.example config.env

# Edit config.env with your settings
nano config.env

# Seed sample data
npm run seed

# Start the backend server
npm run dev
```

The backend will start on `http://localhost:5000`

### 3. Frontend Setup

```bash
# Navigate to frontend directory (root)
cd ..

# Install dependencies
npm install

# Start the development server
npm run dev
```

The frontend will start on `http://localhost:5173`

## 🔧 Configuration

### Backend Environment Variables

Create `backend/config.env`:

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/disaster-preparedness
JWT_SECRET=your-super-secret-jwt-key
JWT_EXPIRE=7d
FRONTEND_URL=http://localhost:5173
```

### Frontend Configuration

The frontend is configured to connect to the backend API. Update the API base URL in your frontend code if needed.

## 📱 Usage

### Default Login Credentials

```
Admin: admin@disastered.com / admin123
Teacher: teacher@disastered.com / teacher123
Student: alice@disastered.com / student123
Student: bob@disastered.com / student123
```

### Key Features

1. **Dashboard**: View progress, recent activities, and quick actions
2. **Learning Modules**: Access interactive educational content
3. **Virtual Drills**: Practice emergency response procedures
4. **Emergency Center**: Access emergency contacts and alerts
5. **Admin Panel**: Manage users, content, and system settings

## 🎯 Educational Content

### Available Modules
- **Earthquake Safety**: Drop, cover, hold techniques
- **Fire Safety**: Evacuation procedures and prevention
- **Flood Response**: Water safety and evacuation
- **Cyclone Preparedness**: Storm safety measures
- **Landslide Management**: Risk assessment and response
- **Chemical Hazards**: Industrial safety protocols

### Virtual Drills
- **Earthquake Response**: Practice drop, cover, hold
- **Fire Evacuation**: Navigate through smoke-filled corridors
- **Flood Response**: Learn water safety procedures

## 🔐 Security Features

- **JWT Authentication**: Secure user sessions
- **Role-based Access Control**: Granular permissions
- **Input Validation**: Comprehensive request validation
- **Rate Limiting**: API protection against abuse
- **CORS Protection**: Secure cross-origin requests
- **Password Hashing**: bcrypt encryption

## 📊 API Documentation

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user

### Modules
- `GET /api/modules` - Get all modules
- `POST /api/modules/:id/start` - Start module
- `POST /api/modules/:id/complete` - Complete module

### Drills
- `GET /api/drills` - Get all drills
- `POST /api/drills/:id/start` - Start drill
- `POST /api/drills/:id/complete` - Complete drill

### Emergency
- `GET /api/emergency/alerts` - Get alerts
- `POST /api/emergency/broadcast` - Send broadcast
- `GET /api/emergency/contacts` - Get contacts

## 🚀 Deployment

### Local Development
```bash
# Backend
cd backend && npm run dev

# Frontend
npm run dev
```

### Production
```bash
# Backend
cd backend && npm start

# Frontend
npm run build && npm run preview
```

### Docker (Optional)
```bash
# Build and run with Docker Compose
docker-compose up --build
```

## 🧪 Testing

```bash
# Run backend tests
cd backend && npm test

# Run frontend tests
npm test
```

## 📈 Performance

- **Frontend**: Optimized with Vite and React 18
- **Backend**: Express.js with MongoDB for fast queries
- **Real-time**: Socket.io for instant updates
- **Caching**: Efficient data caching strategies

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:

- Create an issue in the repository
- Contact the development team
- Check the documentation

## 🔄 Version History

- **v1.0.0** - Initial release with core features
- **v1.1.0** - Added real-time features
- **v1.2.0** - Enhanced admin dashboard

## 🎓 Educational Impact

This platform helps schools:

- **Improve Safety**: Better disaster preparedness
- **Engage Students**: Interactive learning experience
- **Track Progress**: Monitor learning outcomes
- **Coordinate Response**: Real-time emergency management
- **Build Resilience**: Community-wide safety awareness

## 🌍 Global Reach

Designed for Indian schools but adaptable worldwide:

- **Multi-language Support**: English, Hindi, and regional languages
- **Regional Customization**: Location-specific content
- **Cultural Sensitivity**: Culturally appropriate examples
- **Scalable Architecture**: Supports multiple schools

---

**Built with ❤️ for disaster preparedness education**

*Making schools safer, one lesson at a time.*
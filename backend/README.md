# Tinome Backend

The backend service for Tinome, a collaborative platform for ESI students to find partners for academic projects, homework assignments, and hackathons.

## 🎯 Overview

This backend service provides the necessary APIs and data management for the Tinome platform, handling user authentication, project management, team formation, and real-time collaboration features.

## 🛠️ Tech Stack

- Node.js - JavaScript runtime
- Express.js - Web framework
- MongoDB - Database
- Docker - Containerization
- JWT - Authentication
- Socket.IO - Real-time communication

## 📋 Requirements

Please ensure you have the following installed:

- Node.js v20.10.0 or higher
- Git v2.43.0 or higher
- Docker v24.0.6 or higher
- Docker Desktop v4.25.2 or higher
- MongoDB Shell v2.1.0 or higher

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/abderrahimlaribi/tinome-hack.git
cd tinome-hack/backend
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```
Edit the `.env` file with your configuration.

## 🏃‍♂️ Running the Application

### Development Mode

1. Start MongoDB using Docker:
```bash
docker-compose up -d
```

2. Run the development server:
```bash
npm run dev
```

The server will be available at `http://localhost:3000`

### Production Mode

```bash
npm start
```

## 📚 API Documentation

The API documentation is available at `/api-docs` when running the server.

### Main Endpoints

- `/api/auth` - Authentication endpoints
- `/api/users` - User management
- `/api/projects` - Project management
- `/api/teams` - Team formation
- `/api/hackathons` - Hackathon management

## 🧪 Testing

Run the test suite:

```bash
npm test
```

## 🔒 Security

- JWT-based authentication
- Password hashing with bcrypt
- CORS configuration
- Rate limiting
- Input validation
- Security headers

## 📦 Database Schema

The MongoDB database includes collections for:
- Users
- Projects
- Teams
- Hackathons
- Messages
- Notifications

## 🔄 API Versioning

The API follows semantic versioning. Current version: v1

## 🐳 Docker Support

Build and run with Docker:

```bash
docker build -t tinome-backend .
docker run -p 3000:3000 tinome-backend
```

## 📝 Environment Variables

Required environment variables:
- `PORT` - Server port
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - JWT secret key
- `NODE_ENV` - Environment (development/production)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Team

Tinome is developed by and for ESI students. Join us in making collaboration easier for the ESI community!

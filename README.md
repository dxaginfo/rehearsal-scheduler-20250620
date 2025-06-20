# 🎵 Rehearsal Scheduler

A comprehensive web application for bands to schedule rehearsals, track attendance, and manage setlists.

## 🎸 Features

- **Smart Scheduling**: Find optimal rehearsal times based on band member availability
- **Calendar Integration**: Sync with Google, Apple, and Microsoft calendars
- **Attendance Tracking**: Monitor attendance and participation
- **Setlist Management**: Create and share rehearsal setlists
- **Venue Management**: Store and share rehearsal locations
- **Real-time Updates**: Instant notifications for schedule changes
- **Mobile Responsive**: Works on all devices

## 🚀 Tech Stack

- **Frontend**: React.js with TypeScript, Redux Toolkit, Material-UI
- **Backend**: Node.js, Express.js, Socket.io
- **Database**: PostgreSQL with Prisma ORM
- **Caching**: Redis
- **DevOps**: Docker, Kubernetes, GitHub Actions, AWS

## 📋 Prerequisites

- Node.js 18+
- Docker and Docker Compose
- PostgreSQL 14+
- Redis 6+

## 🛠️ Setup Instructions

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/dxaginfo/rehearsal-scheduler-20250620.git
   cd rehearsal-scheduler-20250620
   ```

2. Install dependencies:
   ```bash
   # Install frontend dependencies
   cd frontend
   npm install
   
   # Install backend dependencies
   cd ../backend
   npm install
   ```

3. Set up environment variables:
   ```bash
   # Copy environment variables template
   cp .env.example .env
   
   # Edit .env file with your configuration
   ```

4. Set up the database:
   ```bash
   # Using Docker
   docker-compose up -d postgres redis
   
   # Run migrations
   cd backend
   npx prisma migrate dev
   ```

5. Start the development servers:
   ```bash
   # Start backend server
   cd backend
   npm run dev
   
   # In another terminal, start frontend server
   cd frontend
   npm start
   ```

6. Access the application:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:4000
   - API Documentation: http://localhost:4000/api-docs

### Docker Deployment

1. Build and run with Docker Compose:
   ```bash
   docker-compose up -d
   ```

2. Access the application at http://localhost:3000

## 🧪 Running Tests

```bash
# Run backend tests
cd backend
npm test

# Run frontend tests
cd frontend
npm test
```

## 📚 Documentation

- [API Documentation](./docs/api.md)
- [Architecture Overview](./docs/architecture.md)
- [Database Schema](./docs/database.md)
- [Deployment Guide](./docs/deployment.md)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
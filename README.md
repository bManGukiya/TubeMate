# YouTube Clone - Enterprise Level Project

A full-stack YouTube clone built with Django backend and React frontend with Tailwind CSS.

## 🚀 Features

### Core Features
- **Video Upload & Streaming**: Upload, process, and stream videos
- **User Authentication**: Secure user registration and login
- **Video Management**: Create, edit, delete videos with metadata
- **Comments System**: Real-time comments with nested replies
- **Like/Dislike System**: Interactive video engagement
- **User Profiles**: Customizable user profiles and channels
- **Search & Discovery**: Advanced search with filters
- **Responsive Design**: Mobile-first responsive design
- **Real-time Updates**: WebSocket integration for live features

### Advanced Features
- **Video Processing**: Automatic thumbnail generation
- **Recommendation Engine**: AI-powered video recommendations
- **Analytics Dashboard**: Video performance metrics
- **Playlist Management**: Create and manage video playlists
- **Subscription System**: Subscribe to channels
- **Notification System**: Real-time notifications
- **Admin Panel**: Comprehensive admin interface

## 🏗️ Architecture

```
youtube-clone/
├── backend/                 # Django REST API
│   ├── core/               # Core Django settings
│   ├── apps/               # Django applications
│   ├── media/              # Uploaded files
│   └── requirements.txt    # Python dependencies
├── frontend/               # React application
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── services/       # API services
│   │   ├── utils/          # Utility functions
│   │   └── styles/         # Tailwind CSS styles
│   ├── public/             # Static assets
│   └── package.json        # Node.js dependencies
├── docker/                 # Docker configuration
├── docs/                   # Documentation
└── scripts/                # Deployment scripts
```

## 🛠️ Tech Stack

### Backend
- **Django 4.2+**: Web framework
- **Django REST Framework**: API development
- **PostgreSQL**: Primary database
- **Redis**: Caching and session storage
- **Celery**: Background task processing
- **FFmpeg**: Video processing
- **JWT**: Authentication
- **WebSocket**: Real-time features

### Frontend
- **React 18**: UI framework
- **TypeScript**: Type safety
- **Tailwind CSS**: Styling
- **React Router**: Navigation
- **React Query**: Data fetching
- **Zustand**: State management
- **Axios**: HTTP client
- **Socket.io**: Real-time communication

## 📦 Installation

### Prerequisites
- Python 3.11+
- Node.js 18+
- PostgreSQL
- Redis
- FFmpeg

### Backend Setup
```bash
# Clone the repository
git clone <repository-url>
cd youtube-clone

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
cd backend
pip install -r requirements.txt

# Setup environment variables
cp .env.example .env
# Edit .env with your configuration

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Start development server
python manage.py runserver
```

### Frontend Setup
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Start development server
npm start
```

## 🚀 Quick Start with Docker

```bash
# Build and run with Docker Compose
docker-compose up --build
```

## 📚 API Documentation

The API documentation is available at `/api/docs/` when the backend server is running.

## 🧪 Testing

### Backend Tests
```bash
cd backend
python manage.py test
```

### Frontend Tests
```bash
cd frontend
npm test
```

## 📊 Environment Variables

### Backend (.env)
```env
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgresql://user:password@localhost:5432/youtube_clone
REDIS_URL=redis://localhost:6379
AWS_ACCESS_KEY_ID=your-aws-key
AWS_SECRET_ACCESS_KEY=your-aws-secret
AWS_STORAGE_BUCKET_NAME=your-bucket-name
```

### Frontend (.env)
```env
REACT_APP_API_URL=http://localhost:8000/api
REACT_APP_WS_URL=ws://localhost:8000/ws
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License.

## 🆘 Support

For support, email support@youtube-clone.com or create an issue in the repository. 
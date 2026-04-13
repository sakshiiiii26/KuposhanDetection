# Predictive AI Malnutrition Assessment Backend

A Flask API for malnutrition assessment and user management.

## API Endpoints

### Test
- `GET /api/test` - Test if server is running

### User Management
- `POST /api/user/register` - Register a new user
- `GET /api/user/<user_id>` - Get user details

### Assessment
- `POST /api/assessment/create` - Create new assessment
- `GET /api/assessment/all/<user_id>` - Get all assessments for user
- `GET /api/dashboard/<user_id>` - Get dashboard data

## Local Development

1. Create virtual environment:
```bash
python -m venv venv
```

2. Activate virtual environment:
```bash
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the application:
```bash
python app.py
```

## Deployment

### Heroku Deployment

1. Install Heroku CLI
2. Login to Heroku: `heroku login`
3. Create app: `heroku create your-app-name`
4. Push to Heroku: `git push heroku main`

### Railway Deployment

1. Go to railway.app
2. Connect your GitHub repository
3. Deploy automatically

### Other Platforms

The app can be deployed to any platform supporting Python/Flask:
- AWS EC2
- DigitalOcean
- Render
- Fly.io

## Environment Variables

- `PORT` - Port to run the server (default: 5000)
- `DEBUG` - Debug mode (default: False)
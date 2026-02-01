
## ⚙️ Backend API Documentation

### Authentication
All API requests require authentication via JWT:
```bash
Authorization: Bearer <your_jwt_token>
```

### Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /auth/login | User authentication |
| GET | /users/me | Current user profile |
| GET | /games | List active games |
| POST | /games/:id/score | Submit score |

### Database Schema
- Users table with wallet addresses
- Games table with metadata
- Scores table for leaderboards
- Sessions for auth management

### Running Locally
```bash
# Install dependencies
npm install

# Run migrations
npm run db:migrate

# Start server
npm run dev
```

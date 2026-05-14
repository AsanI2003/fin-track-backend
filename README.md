---

### fin-track-backend
This README focuses on your backend engineering skills, API structure, and data security of FinTrack 

```markdown
# Fin-Track Backend

The robust API powering the Fin-Track ecosystem. This service handles authentication, financial transactions, and subscription logic with a focus on data integrity and security.

## 🛠️ Tech Stack
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB (Mongoose ODM)
- **Security**: JWT (JSON Web Tokens) & Bcrypt
- **Environment**: Dotenv

## Key Backend Features
- **RESTful API Design**: Clean and predictable endpoints for financial data.
- **AI Integration**: FinTrack AI chatbot using Groq AI
- **JWT Authentication**: Secure user sessions and protected route middleware.
- **Aggregation Pipelines**: Efficient MongoDB queries for calculating monthly summaries and trends.
- **Validation**: Strict schema validation to ensure data consistency.

## API Endpoints (Quick View)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/auth/register` | User registration |
| `POST` | `/api/auth/login` | User login |
| `GET` | `/api/transactions` | Fetch all user transactions |
| `POST` | `/api/transactions` | Create a new record |
| `GET` | `/api/summary` | Get balance and spending analytics |
| `POST` | `/api/ai` | Ask questions from chatbot |

## Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/AsanI2003/fin-track-backend.git](https://github.com/AsanI2003/fin-track-backend.git)
   cd fin-track-backend
Install dependencies:

Bash
npm install
Configure Environment:
Create a .env file in the root:

Code snippet
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secure_secret_key
Start the server:

Bash
npm run start # Production
npm run dev   # Development with Nodemon
Architecture

src/
├── controllers/  # Request handling logic
├── models/       # Mongoose schemas (User, Transaction, Subscription)
├── routes/       # API route definitions
├── middleware/   # Auth and error handling middleware
└── config/       # Database and server configuration

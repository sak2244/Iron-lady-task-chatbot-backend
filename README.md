# Iron Lady AI Career Guide Backend

An Express.js backend service for the Iron Lady women-focused career transformation platform. This service provides AI-powered career guidance using Google's Gemini API.

## Features

- **AI Career Advisor**: Uses Google Gemini 2.5 Flash model to provide personalized career recommendations
- **Program Recommendations**: Suggests the best Iron Lady programs based on user background
- **CORS Enabled**: Supports cross-origin requests for frontend integration
- **Environment Configuration**: Secure API key management using environment variables

## Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Google Gemini API key

## Installation

1. Clone or navigate to the project directory:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory:
   ```
   GEMINI_API_KEY=AIzaSyD7aiQmIHhJvJDK2tB9O1Oz9Yz0A1fgoao
   ```

## Usage

Start the server:

```bash
npm start
```

The server will run on the default port (typically 3000 or as configured).

## API Endpoints

### POST /chat

Sends a user message to the AI Career Advisor and receives personalized career guidance.

**Request:**

```json
{
  "message": "I have 5 years of marketing experience and want to transition to tech"
}
```

**Response:**

```json
{
  "response": "AI-generated career advice and program recommendations..."
}
```

## Dependencies

- **express**: Web framework for Node.js
- **cors**: Cross-Origin Resource Sharing middleware
- **dotenv**: Environment variable management
- **@google/generative-ai**: Google Gemini API client library

## Project Structure

```
backend/
├── index.js         # Main application file
├── package.json     # Project dependencies and scripts
└── README.md        # This file
```

## Environment Variables

```
 GEMINI_API_KEY=AIzaSyD7aiQmIHhJvJDK2tB9O1Oz9Yz0A1fgoao
```

## License

ISC

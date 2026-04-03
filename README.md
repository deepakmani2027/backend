# InventoryPro Backend API

FastAPI-based backend for InventoryPro chatbot system.

## Setup

### Local Development

```bash
# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set environment variables
export SUPABASE_URL=https://grkfoepzoqhloxanexmb.supabase.co
export SUPABASE_SERVICE_KEY=your_service_key
export OPENROUTER_API_KEY=your_api_key

# Run server
python server.py
```

Server runs on `http://localhost:8001`

## API Endpoints

- `GET /api/health` - Health check
- `POST /api/chat` - Chat endpoint with real inventory data

## Environment Variables

- `SUPABASE_URL` - Supabase project URL
- `SUPABASE_SERVICE_KEY` - Supabase service role key  
- `OPENROUTER_API_KEY` - OpenRouter API key for LLM

## Deployment on Railway

```bash
# Push to GitHub
git push origin main

# Railway will auto-deploy
# Set environment variables in Railway dashboard
# Backend URL will be provided
```

## Features

- Real-time inventory data from Supabase
- AI-powered chat using OpenRouter API
- Low stock alerts
- Recent sales information
- Session management

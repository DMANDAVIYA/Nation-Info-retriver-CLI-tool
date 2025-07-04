# DIplotools - Dhruvil (internal tool) ALPHA PHASE — Setup Guide

This guide will help you set up and run the internal tool that uses Google Gemini 2.0 Flash AI to answer questions about any country.

---

## Prerequisites
- **Node.js** (v18 or higher)
- **Gemini API Key** from Google AI Studio

## Getting Your Gemini API Key
1. Go to [Google AI Studio](https://aistudio.google.com/)
2. Sign in with your Google account
3. Click on "Get API key" or go to the API keys section
4. Create a new API key
5. Copy the API key (it starts with "AI")

## Environment Setup
1. In the `inputproj` folder, create a file named `.env`
2. Add your Gemini API key to the file:
   ```env
   GEMINI_API_KEY=your_actual_api_key_here
   ```
   Replace `your_actual_api_key_here` with your real Gemini API key.

## Installation
1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the development server:
   ```bash
   npm run dev
   ```
3. Open your browser to the URL shown (typically `http://localhost:5173`)

## How to Use
1. **Select a Country** from the dropdown
2. **Ask a Question** about the country (e.g., culture, history, economy, etc.)
3. **Click Get Information**
4. **View the AI-powered response** in JSON format below the form

## Example Questions
- "Tell me about the culture and traditions"
- "What is the history of this country?"
- "Describe the economy and major industries"
- "What are the main tourist attractions?"
- "Explain the political system and government structure"

## Troubleshooting
- **"Gemini API key not configured"**: Make sure you've created the `.env` file with your API key
- **"Failed to generate response"**: Check your internet connection and API key validity
- **Port already in use**: Try running `npm run dev -- --port 3001` to use a different port

## Features
- 🌍 Country dropdown with 195+ countries
- 🤖 AI-powered answers using Gemini 2.0 Flash
- 📝 Real-time JSON response display
- 🚦 Error handling and loading states
- 💻 Modern, responsive UI
- 🟦 TypeScript support

---

For internal use only. Not for public distribution. 
# AI Email Writer - Frontend

This is the frontend for the AI-powered Email Reply Generator. It is built using React and Material-UI to provide a simple interface for generating AI-powered email replies.

## Features
- User-friendly interface for generating email replies
- Allows users to specify the tone of the response
- Uses Axios to send requests to the backend
- Material-UI for modern styling

## Technologies Used
- React
- Material-UI (@mui/material)
- Axios

## Installation

### Prerequisites
- Node.js installed
- Backend API running ([Backend Repository](https://github.com/JohnUfo/ai-email-writer.git))

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/JohnUfo/ai-email-writer-front.git
   cd ai-email-writer-front
   ```
2. Install dependencies:
   ```sh
   npm install
   npm install @mui/material @emotion/react @emotion/styled
   npm install axios
   ```
3. Start the frontend:
   ```sh
   npm run dev
   ```
4. The frontend will be available at:
   ```sh
   http://localhost:5173
   ```

## How It Works [click here](https://scribehow.com/shared/Generate_and_Copy_a_Professional_Email_Reply__LMBAtNRpQz-XcuAeDWHQLQ).
1. Enter the original email content in the text area.
2. Select an optional tone (Professional, Casual, Friendly).
3. Click "Generate Reply" to generate a response.
4. The AI-generated reply will appear below.
5. Copy the generated reply to the clipboard using the "Copy to Clipboard" button.

## API Integration
- The frontend sends a `POST` request to the backend at:
  ```sh
  http://localhost:8080/api/email/generate
  ```
- The request body:
  ```json
  {
    "emailContent": "Hello, can we reschedule our meeting?",
    "tone": "professional"
  }
  ```
- The response:
  ```json
  "Sure, let me know a convenient time for you."
  ```

## Related Projects
- [Backend Repository](https://github.com/JohnUfo/ai-email-writer.git) (Required to run the frontend)
- [Chrome Extension](https://github.com/JohnUfo/ai-email-writer-extension.git) (For AI-powered email replies within Gmail)


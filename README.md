# Nabi - A Love Letter Web App

A beautiful interactive web application for sharing heartfelt letters. Built with Node.js and Express.

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm

### Installation

1. Clone the repository
```bash
git clone <your-repo-url>
cd nabi
```

2. Install dependencies
```bash
npm install
```

3. Start the server
```bash
npm start
```

The application will be available at `http://localhost:3000`

## Deployment to Render

### Quick Deploy (Recommended)

1. Push your code to GitHub
2. Go to [Render.com](https://render.com)
3. Click "New" → "Web Service"
4. Connect your GitHub repository
5. Render will automatically detect the `render.yaml` configuration
6. Click "Create Web Service"

Your app will be live in a few minutes!

### Manual Configuration (if needed)

If automatic detection doesn't work:
- **Build Command**: `npm install`
- **Start Command**: `npm start`  
- **Node Version**: 18 or higher

## Project Structure

```
nabi/
├── public/
│   ├── index.html          # Main HTML file with all styles and scripts
│   └── download (1).gif    # Hug animation (if used)
├── server.js               # Express server
├── package.json            # Dependencies and scripts
├── render.yaml             # Render deployment config
└── README.md              # This file
```

## Features

- Interactive letter cards for different emotions
- Beautiful animations and particle effects
- Typewriter effect for letter content
- Flower bloom animation
- Music/Spotify integration
- Hug button with overlay
- Fully responsive design

## Customization

Edit the letter content in `public/index.html`:

```javascript
const LETTERS = {
  happy: {
    icon: '۶ৎ',
    title: 'A Letter to Make You Happy',
    lines: [
      'Your custom letter text here...',
      // Add more lines as needed
    ]
  },
  // ... other letters
};
```

## Environment Variables

Currently, no environment variables are required. The app runs on port 3000 by default, or uses the `PORT` environment variable if set.

## License

MIT
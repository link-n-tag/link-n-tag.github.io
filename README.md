# Link Tag 🔗

A simple and beautiful web application to store and organize your favorite weblinks. All data is stored locally in your browser using localStorage.

## Features

- ✨ Modern, responsive dark-themed UI
- 📝 Add, edit, and delete links
- 🔍 Search functionality to find links quickly
- 🏷️ Tag support for organizing links
- 💾 Local storage - all data saved in your browser
- 🚀 No backend required - works entirely in the browser

## Tech Stack

- **Frontend**: React
- **Storage**: Browser localStorage
- **Styling**: CSS3 with dark theme

## Installation

1. **Install dependencies:**
   ```bash
   npm run install-client
   ```

## Running the Application

### Development Mode

Start the React development server:
```bash
npm start
```

The application will open at `http://localhost:3000`

### Production Build

Build the app for production:
```bash
npm run build
```

The built files will be in the `client/build` directory and can be served by any static file server.

## Usage

1. Click "Add New Link" to create a new bookmark
2. Fill in the title and URL (required fields)
3. Optionally add a description and tags
4. Use the search bar to filter your links
5. Click the edit icon (✏️) to modify a link
6. Click the delete icon (🗑️) to remove a link

All your links are automatically saved to your browser's localStorage and will persist between sessions.

## Data Storage

All links are stored locally in your browser using localStorage. This means:
- Your data never leaves your computer
- No server or database required
- Data persists between browser sessions
- Each browser profile has its own separate link collection

## License

MIT

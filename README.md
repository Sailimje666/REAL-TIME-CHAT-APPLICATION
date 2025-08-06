# Real-time Chat Application

A modern, responsive real-time chat application built with **React.js** and **WebSockets** using **Socket.io**.

## 🚀 Features

- **Real-time Messaging**: Instant message delivery using WebSockets
- **User Authentication**: Simple username-based login system
- **Message History**: View previous messages when joining the chat
- **Typing Indicators**: See when other users are typing
- **Online User List**: View all connected users with their status
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Modern UI**: Beautiful gradient design with smooth animations
- **System Messages**: Automatic notifications for user join/leave events
- **Message Timestamps**: See when each message was sent
- **Character Counter**: Track message length (500 character limit)

## 🛠️ Tech Stack

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **Socket.io** - Real-time WebSocket library
- **CORS** - Cross-origin resource sharing
- **UUID** - Unique identifier generation

### Frontend
- **React.js** - UI library
- **Socket.io-client** - WebSocket client
- **CSS3** - Styling with modern features
- **Responsive Design** - Mobile-first approach

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- npm (v6 or higher)

### Setup Instructions

1. **Clone or navigate to the project directory**
   ```bash
   cd task 2
   ```

2. **Install server dependencies**
   ```bash
   npm install
   ```

3. **Install client dependencies**
   ```bash
   cd client
   npm install
   cd ..
   ```

4. **Start the development servers**
   ```bash
   # Start both server and client simultaneously
   npm run dev
   
   # Or start them separately:
   # Terminal 1 - Start server
   npm run server
   
   # Terminal 2 - Start client
   npm run client
   ```

5. **Open your browser**
   - Server runs on: `http://localhost:5000`
   - Client runs on: `http://localhost:3000`
   - Open `http://localhost:3000` in your browser

## 🎯 How to Use

1. **Join the Chat**
   - Enter your username in the login screen
   - Click "Join Chat" or press Enter

2. **Send Messages**
   - Type your message in the input field
   - Press Enter or click the send button
   - Messages support up to 500 characters

3. **View Online Users**
   - Click the "Users" button in the header
   - See all connected users with their join times

4. **Real-time Features**
   - See typing indicators when others are typing
   - Get notified when users join or leave
   - Messages appear instantly for all users

## 📱 Responsive Design

The application is fully responsive and works on:
- **Desktop**: Full-featured interface with sidebar
- **Tablet**: Optimized layout for medium screens
- **Mobile**: Touch-friendly interface with collapsible elements

## 🔧 Available Scripts

```bash
# Install all dependencies (server + client)
npm run install-all

# Start both server and client in development mode
npm run dev

# Start only the server
npm run server

# Start only the client
npm run client

# Build the client for production
npm run build

# Start production server
npm start
```

## 🌐 API Endpoints

- `GET /api/health` - Server health check
- `GET /api/users` - Get list of online users

## 🔌 WebSocket Events

### Client to Server
- `user_join` - User joins the chat
- `send_message` - Send a new message
- `typing` - Typing indicator

### Server to Client
- `user_connected` - User successfully connected
- `message` - New message received
- `user_list_update` - Online users list updated
- `user_typing` - Typing indicator from other users

## 🎨 Design Features

- **Gradient Backgrounds**: Modern purple-blue gradients
- **Smooth Animations**: Fade-in effects and hover transitions
- **Chat Bubbles**: Different styles for own vs other messages
- **System Messages**: Centered notifications with icons
- **User Avatars**: Color-coded circles with initials
- **Online Indicators**: Pulsing green dots for active users

## 🔒 Security Features

- Input validation and sanitization
- Message length limits
- Username validation
- CORS configuration for secure communication

## 🚀 Deployment

### Production Build
```bash
# Build the React app
npm run build

# Start production server
npm start
```

### Environment Variables
- `PORT` - Server port (default: 5000)
- `NODE_ENV` - Environment mode (development/production)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License.

## 🐛 Troubleshooting

### Common Issues

1. **Port already in use**
   - Change the port in `server/index.js`
   - Or kill the process using the port

2. **WebSocket connection failed**
   - Ensure the server is running on port 5000
   - Check firewall settings
   - Verify CORS configuration

3. **Client won't start**
   - Ensure all dependencies are installed
   - Check Node.js version compatibility
   - Clear npm cache if needed

### Support
If you encounter any issues, please check:
- Node.js version (should be 14+)
- npm version (should be 6+)
- All dependencies are properly installed
- No other services are using the required ports

---

**Enjoy chatting! 💬✨** 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Real-Time Chat Application</title>
</head>
<body>

<h1>💬 Real-Time Chat Application</h1>

<p>A full-stack <strong>real-time chat application</strong> built with <strong>React, Node.js, Express, MongoDB, and Socket.IO</strong>. It supports secure authentication, individual and group conversations, real-time messaging, profile customization, emoji support, and file sharing through a clean and responsive interface.</p>

<hr>

<h2>✨ Features</h2>
<ul>
<li>🔐 <strong>JWT Authentication</strong> — Secure login and signup flow</li>
<li>💬 <strong>Real-Time Messaging</strong> — Powered by Socket.IO</li>
<li>👤 <strong>Individual Chats</strong> — Private one-to-one conversations</li>
<li>👥 <strong>Group Chats</strong> — Create channels and group conversations</li>
<li>📎 <strong>File Uploads & Downloads</strong> — Share files in conversations</li>
<li>🖼️ <strong>Profile Setup</strong> — Customize profile information and avatar</li>
<li>😀 <strong>Emoji Support</strong> — Integrated emoji picker</li>
<li>⚡ <strong>State Management</strong> — Zustand</li>
<li>🕒 <strong>Message Timestamps</strong> — Moment.js</li>
<li>🎨 <strong>Modern UI</strong> — ShadCN UI and React Icons</li>
<li>📱 <strong>Responsive Design</strong> — Works across different screen sizes</li>
</ul>

<h2>🛠️ Tech Stack</h2>
<h3>Frontend</h3>
<ul>
<li>React</li><li>Vite</li><li>Zustand</li><li>Axios</li><li>Socket.IO Client</li>
<li>Emoji Picker React</li><li>React Icons</li><li>ShadCN UI</li>
</ul>

<h3>Backend</h3>
<ul>
<li>Node.js</li><li>Express.js</li><li>MongoDB</li><li>Mongoose</li>
<li>Socket.IO</li><li>JWT / JSON Web Token</li><li>Bcrypt</li>
<li>Cookie Parser</li><li>CORS</li><li>Dotenv</li>
</ul>

<h2>📁 Project Structure</h2>
<pre>
chat/
├── 📁 client
│   ├── 📁 public
│   │   ├── 🖼️ contact.png
│   │   └── 🖼️ download.png
│   ├── 📁 src
│   │   ├── 📁 assets
│   │   ├── 📁 components
│   │   │   ├── 📁 ui
│   │   │   └── 📄 ContactList.jsx
│   │   ├── 📁 context
│   │   │   └── 📄 SocketContext.jsx
│   │   ├── 📁 lib
│   │   ├── 📁 pages
│   │   │   ├── 📁 auth
│   │   │   ├── 📁 chat
│   │   │   └── 📁 profile
│   │   ├── 📁 store
│   │   │   └── 📁 slices
│   │   │       ├── 📄 auth-slice.js
│   │   │       └── 📄 chat-slice.js
│   │   ├── 📁 utils
│   │   ├── 🎨 App.css
│   │   ├── 📄 App.jsx
│   │   ├── 🎨 index.css
│   │   └── 📄 main.jsx
│   ├── ⚙️ .gitignore
│   ├── ⚙️ components.json
│   ├── 📄 eslint.config.js
│   ├── 🌐 index.html
│   ├── ⚙️ jsconfig.json
│   ├── 📦 package.json
│   └── ⚙️ vite.config.js
│
├── 📁 server
│   ├── 📁 controllers
│   │   ├── 📄 AuthController.js
│   │   ├── 📄 ChannelController.js
│   │   ├── 📄 ContactsController.js
│   │   └── 📄 MessagesController.js
│   ├── 📁 middlewares
│   │   └── 📄 AuthMiddleware.js
│   ├── 📁 models
│   │   ├── 📄 ChannelModel.js
│   │   ├── 📄 MessagesModel.js
│   │   └── 📄 UserModel.js
│   ├── 📁 routes
│   │   ├── 📄 AuthRoutes.js
│   │   ├── 📄 ChannelRoutes.js
│   │   ├── 📄 ContactRoutes.js
│   │   └── 📄 MessagesRoutes.js
│   ├── 📁 uploads
│   │   ├── 📁 files
│   │   └── 📁 profiles
│   ├── ⚙️ .gitignore
│   ├── 📄 index.js
│   ├── 📦 package.json
│   └── 📄 socket.js
│
├── ⚙️ .gitignore
└── 📝 README.md
</pre>

<h2>🚀 Getting Started</h2>

<h3>1. Clone the Repository</h3>
<pre><code>git clone &lt;your-repository-url&gt;
cd chat</code></pre>

<h3>2. Install Frontend Dependencies</h3>
<pre><code>cd client
npm install</code></pre>

<h3>3. Install Backend Dependencies</h3>
<pre><code>cd ../server
npm install</code></pre>

<h3>4. Configure Environment Variables</h3>
<p>Create a <code>.env</code> file inside the <code>server</code> directory:</p>
<pre><code>PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret</code></pre>

<h3>5. Start the Backend</h3>
<pre><code>cd server
npm run dev</code></pre>

<h3>6. Start the Frontend</h3>
<pre><code>cd client
npm run dev</code></pre>

<h2>🔄 Application Flow</h2>
<pre>
User
 │
 ▼
React Frontend
 │
 ├── Authentication
 ├── Contact Management
 ├── Chat Interface
 ├── Profile Management
 └── File Sharing
 │
 ▼
Express REST API
 │
 ├── Controllers
 ├── Routes
 ├── Authentication Middleware
 └── MongoDB / Mongoose
 │
 ▼
Socket.IO
 │
 └── Real-Time Messages
</pre>

<h2>🔐 Authentication</h2>
<ul>
<li>User registration and login</li>
<li>Password hashing with Bcrypt</li>
<li>JWT-based authentication</li>
<li>Protected backend routes</li>
<li>Authentication middleware</li>
</ul>

<h2>💬 Chat System</h2>
<h3>Private Messaging</h3>
<ul><li>Start individual conversations</li><li>Send messages in real time</li><li>Share files</li><li>Use emojis</li><li>View message timestamps</li></ul>

<h3>Group Messaging</h3>
<ul><li>Create channels</li><li>Select multiple members</li><li>Participate in group conversations</li><li>Send real-time messages</li><li>Share files within groups</li></ul>

<h2>📎 File Sharing</h2>
<p>Files and profile images are stored under the server upload directories.</p>
<pre>
server/
└── uploads/
    ├── files/
    └── profiles/
</pre>

<h2>🎨 UI Components</h2>
<p>The frontend uses reusable ShadCN UI components including Avatar, Badge, Button, Dialog, Input, Tabs, Tooltip, Scroll Area, Command, Multiple Select, and Sonner notifications.</p>

<h2>⚡ State Management</h2>
<pre>
store/
├── index.js
└── slices/
    ├── auth-slice.js
    └── chat-slice.js
</pre>

<p>Zustand keeps authentication and chat state organized across the application.</p>

<h2>🔌 Real-Time Communication</h2>
<p><strong>Socket.IO</strong> handles real-time private and group messaging.</p>
<pre>
Client
  │
  │ Socket.IO
  ▼
Socket Server
  │
  ├── Private Messages
  ├── Group Messages
  └── Real-Time Updates
</pre>

<p>Frontend socket management: <code>client/src/context/SocketContext.jsx</code></p>
<p>Backend socket configuration: <code>server/socket.js</code></p>

<h2>📱 Responsive Design</h2>
<p>Designed for desktop, laptop, tablet, and mobile screens.</p>

<h2>🔮 Future Improvements</h2>
<ul>
<li>🔔 Push notifications</li>
<li>🟢 Online/offline status</li>
<li>✍️ Typing indicators</li>
<li>✅ Message delivery and read status</li>
<li>🔍 Advanced message search</li>
<li>🎤 Voice messages</li>
<li>📹 Voice/video calling</li>
<li>🗑️ Message editing and deletion</li>
</ul>

<hr>

<h2>👨‍💻 Author</h2>
<p><strong>Zohaib</strong></p>
<p>Built with ❤️ using the MERN stack and Socket.IO.</p>
<p>⭐ If you like this project, consider giving the repository a star on GitHub.</p>

</body>
</html>

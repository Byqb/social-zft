# social-zft

You will have to create migrations for this project so every time the application runs, it creates the specific tables to make the project work properly.

For this, you must focus on a folder structure similar to this one:

```console
student$ tree .
backend
├── pkg
│   ├── db
│   │   ├── migrations
│   │   │   └── sqlite
│   │   │       ├── 000001_create_users_table.down.sql
│   │   │       ├── 000001_create_users_table.up.sql
│   │   │       ├── 000002_create_posts_table.down.sql
│   │   │       └── 000002_create_posts_table.up.sql
│   │   └── sqlite
│   |       └── sqlite.go
|   |
|   └── ...other_pkgs.go
|
└── server.go
```

```console
📦 social-network-project
 ├── 📂 backend
 │    ├── 📂 controllers
 │    │    ├── authController.js  ✅ Implement JWT authentication (Login, Signup, Logout)
 │    │    ├── postController.js  ✅ CRUD operations for posts
 │    │    ├── userController.js  ✅ Manage user profiles and settings
 │    │    ├── chatController.js  ✅ WebSockets for real-time chat
 │    │    ├── notificationController.js ✅ Handle notifications
 │    ├── 📂 models
 │    │    ├── User.js  ✅ Define user schema (name, email, password, profile, etc.)
 │    │    ├── Post.js  ✅ Post schema (content, media, timestamps, author)
 │    │    ├── Chat.js  ✅ Chat schema (sender, receiver, messages)
 │    │    ├── Notification.js ✅ Notification schema
 │    ├── 📂 routes
 │    │    ├── authRoutes.js  ✅ Define authentication routes
 │    │    ├── userRoutes.js  ✅ Define user profile and settings routes
 │    │    ├── postRoutes.js  ✅ Define post CRUD routes
 │    │    ├── chatRoutes.js  ✅ Define chat-related routes
 │    ├── 📂 middleware
 │    │    ├── authMiddleware.js ✅ Protect routes with authentication
 │    │    ├── errorHandler.js ✅ Centralized error handling
 │    ├── 📂 config
 │    │    ├── db.js ✅ Database connection
 │    │    ├── env.js ✅ Load environment variables
 │    ├── server.js ✅ Main server file (Express setup)
 │    ├── package.json ✅ Dependencies and scripts
 │    ├── .env ✅ Environment variables (DO NOT COMMIT)
 │
 ├── 📂 frontend
 │    ├── 📂 components
 │    │    ├── Header.js ✅ Navigation bar
 │    │    ├── Post.js ✅ Single post component
 │    │    ├── Chat.js ✅ Chat UI component
 │    │    ├── Profile.js ✅ Profile page component
 │    ├── 📂 pages
 │    │    ├── Home.js ✅ Display news feed
 │    │    ├── Profile.js ✅ User profile page
 │    │    ├── Chat.js ✅ Chat system page
 │    │    ├── Login.js ✅ User login page
 │    │    ├── Register.js ✅ User registration page
 │    ├── 📂 assets
 │    │    ├── images/ ✅ Profile pictures, post images
 │    │    ├── icons/ ✅ Icons for UI
 │    ├── 📂 utils
 │    │    ├── api.js ✅ Handles API requests
 │    │    ├── auth.js ✅ Manage authentication tokens
 │    ├── App.js ✅ Main frontend component
 │    ├── index.js ✅ Entry point for frontend
 │    ├── package.json ✅ Dependencies and scripts
 │
 ├── 📂 database
 │    ├── schema.sql ✅ Database schema for PostgreSQL/MySQL
 │    ├── migrations/ ✅ Migration files
 │    ├── seeders/ ✅ Test data for development
 │
 ├── 📂 docs
 │    ├── API_Documentation.md ✅ API reference
 │    ├── Setup_Guide.md ✅ How to set up the project
 │    ├── Troubleshooting.md ✅ Common issues and fixes
 │
 ├── README.md ✅ Project overview and setup guide
 ├── .gitignore ✅ Files to ignore in Git
 ├── docker-compose.yml ✅ Docker setup for backend, frontend, and database

```

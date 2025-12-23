# Plumelive

Welcome to **Plumelive** – your creative writing platform designed to empower authors, storytellers, and creative minds. Whether you're writing books, novels, mangas, crafting citations, or sharing stories, Plumelive provides the tools and community you need to bring your literary visions to life.

## 🌟 Features

- **Multi-Format Writing Support**: Write books, novels, mangas, short stories, and more
- **Rich Text Editing**: Powerful editor with formatting options tailored for creative writing
- **Citation Management**: Easily manage and organize citations and references
- **Collaborative Tools**: Share and collaborate with other writers
- **Community Engagement**: Connect with a vibrant community of writers and readers
- **Cloud Storage**: Secure cloud backup for all your creative works
- **Export Options**: Export your works in multiple formats (PDF, EPUB, DOCX, etc.)
- **Version Control**: Keep track of document revisions and history

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Node.js** (v16.0 or higher)
- **npm** (v7.0 or higher) or **yarn** (v1.22 or higher)
- **Git**
- **MongoDB** (v4.4 or higher) or MongoDB Atlas account for cloud database

### Installation

Follow these steps to set up Plumelive locally:

#### 1. Clone the Repository

```bash
git clone https://github.com/snoopyx15/plumelive.git
cd plumelive
```

#### 2. Install Dependencies

Using npm:
```bash
npm install
```

Or using yarn:
```bash
yarn install
```

#### 3. Environment Setup

Create a `.env` file in the root directory and configure the following variables:

```env
# Server Configuration
PORT=5000
NODE_ENV=development

# Database Configuration
MONGODB_URI=mongodb://localhost:27017/plumelive
# Or use MongoDB Atlas:
# MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/plumelive

# JWT Configuration
JWT_SECRET=your_jwt_secret_key_here
JWT_EXPIRE=7d

# Email Configuration (optional)
SMTP_HOST=your_smtp_host
SMTP_PORT=587
SMTP_USER=your_email@example.com
SMTP_PASS=your_email_password

# API Configuration
API_URL=http://localhost:5000/api
CLIENT_URL=http://localhost:3000

# File Upload Configuration
MAX_FILE_SIZE=52428800
UPLOAD_PATH=./uploads
```

#### 4. Database Setup

If using MongoDB locally, start your MongoDB service:

```bash
# macOS with Homebrew
brew services start mongodb-community

# Linux
sudo systemctl start mongod

# Windows
net start MongoDB
```

#### 5. Run the Application

**Development Mode:**

```bash
npm run dev
```

Or with yarn:
```bash
yarn dev
```

**Production Mode:**

```bash
npm run build
npm start
```

The application should now be running at `http://localhost:3000` (frontend) and `http://localhost:5000` (backend API).

### Project Structure

```
plumelive/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/         # Page components
│   │   ├── styles/        # CSS files
│   │   └── App.js
│   └── package.json
├── server/                 # Backend Node.js application
│   ├── routes/            # API routes
│   ├── models/            # Database models
│   ├── controllers/       # Request handlers
│   ├── middleware/        # Custom middleware
│   └── server.js
├── .env                    # Environment variables (create this)
├── .gitignore
├── package.json
└── README.md
```

## 📝 Usage

### Creating Your First Story

1. Sign up or log in to your Plumelive account
2. Click "New Project" to start a new writing project
3. Choose your project type (Novel, Short Story, Manga, etc.)
4. Begin writing using our rich text editor
5. Save your work (auto-save is enabled)
6. Publish or share with the community when ready

### Managing Citations

1. Navigate to the Citations section
2. Add citations using various formats (APA, MLA, Chicago, etc.)
3. Insert citations directly into your documents
4. Generate a bibliography automatically

## 🔧 Available Scripts

In the root directory, you can run:

### `npm run dev`
Runs both frontend and backend in development mode

### `npm run build`
Builds the production version of the application

### `npm start`
Starts the application in production mode

### `npm test`
Runs the test suite

### `npm run lint`
Checks code quality and style

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

1. **Fork** the repository
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Make your changes** and commit them: `git commit -m 'Add some feature'`
4. **Push to the branch**: `git push origin feature/your-feature-name`
5. **Create a Pull Request** with a clear description of your changes

Please ensure your code follows our coding standards and includes appropriate tests.

## 🐛 Reporting Issues

Found a bug or have a suggestion? Please [open an issue](https://github.com/snoopyx15/plumelive/issues) on GitHub. Include:

- A clear description of the issue
- Steps to reproduce (if applicable)
- Expected vs. actual behavior
- Screenshots or error messages

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💬 Support

For support, questions, or feedback:

- **Discord**: [Join our community server](#)
- **Email**: support@plumelive.com
- **Twitter**: [@plumelive](#)
- **Issues**: [GitHub Issues](https://github.com/snoopyx15/plumelive/issues)

## 🎯 Roadmap

- [ ] Advanced formatting options for manga
- [ ] AI-powered writing suggestions
- [ ] Real-time collaboration features
- [ ] Mobile app for iOS and Android
- [ ] Translation tools for multilingual content
- [ ] Advanced analytics for author metrics

## ✨ Acknowledgments

- Thanks to all our contributors and community members
- Special thanks to the open-source libraries and tools that make Plumelive possible

---

**Happy Writing! 📚✍️**

*Plumelive - Where Stories Come to Life*

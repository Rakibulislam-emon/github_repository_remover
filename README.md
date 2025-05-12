# GitHub Repo Remover

![GitHub Repo Remover Banner](https://github.com/Rakibulislam-emon/github_repo_remover_react/raw/main/client/public/banner.png)

A modern web application that helps developers clean up and manage their GitHub repositories with an intuitive interface.

## 🌟 Live Demo

Visit the live application: [GitHub Repo Remover](https://github-repo-remover.vercel.app)

## ✨ Features

- **GitHub OAuth Integration**: Secure authentication with GitHub
- **Repository Management**: View, sort, and filter your GitHub repositories
- **Batch Operations**: Select and delete multiple repositories at once
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Real-time Updates**: UI updates instantly after operations

## 🛠️ Tech Stack

### Frontend
- **React 19**: Latest version of React for building the UI
- **Vite**: Next-generation frontend tooling
- **Tailwind CSS**: Utility-first CSS framework
- **React Router**: Client-side routing
- **Axios**: Promise-based HTTP client
- **React Icons**: Popular icon library

### Backend
- **Node.js**: JavaScript runtime
- **Express**: Web application framework
- **GitHub API**: For repository management
- **OAuth 2.0**: For secure authentication

## 📸 Screenshots

<div align="center">
  <img src="https://github.com/Rakibulislam-emon/github_repo_remover_react/raw/main/screenshots/home.png" alt="Home Page" width="45%">
  <img src="https://github.com/Rakibulislam-emon/github_repo_remover_react/raw/main/screenshots/repos.png" alt="Repositories Page" width="45%">
</div>

## 🚀 Getting Started

### Prerequisites

- Node.js 18.x or higher
- npm or yarn
- GitHub account
- GitHub OAuth App credentials

### Installation and Setup

#### 1. Clone the repository
```bash
git clone https://github.com/Rakibulislam-emon/github_repo_remover_react.git
cd github_repo_remover_react
```

#### 2. Frontend Setup
```bash
cd client
npm install
```

Create a `.env` file in the client directory:
```
VITE_API_URL=http://localhost:5000
```

Start the development server:
```bash
npm run dev
```

#### 3. Backend Setup
```bash
cd ../server
npm install
```

Create a `.env` file in the server directory:
```
PORT=5000
GITHUB_CLIENT_ID=your_github_client_id
GITHUB_CLIENT_SECRET=your_github_client_secret
GITHUB_CALLBACK_URL=http://localhost:5000/auth/github/callback
CLIENT_URL=http://localhost:5173
```

Start the server:
```bash
npm run dev
```

#### 4. GitHub OAuth Setup

1. Go to [GitHub Developer Settings](https://github.com/settings/developers)
2. Click "New OAuth App"
3. Fill in the application details:
   - Application name: GitHub Repo Remover
   - Homepage URL: http://localhost:5173
   - Authorization callback URL: http://localhost:5000/auth/github/callback
4. Register the application and note your Client ID and Client Secret

## 📁 Project Structure

```
github_repo_remover_react/
├── client/                 # Frontend React application
│   ├── public/             # Static files
│   ├── src/                # Source files
│   │   ├── components/     # React components
│   │   │   ├── auth/       # Authentication components
│   │   │   ├── layout/     # Layout components
│   │   │   ├── repos/      # Repository management components
│   │   │   └── router/     # Routing configuration
│   │   ├── assets/         # Images, fonts, etc.
│   │   ├── App.jsx         # Main application component
│   │   └── main.jsx        # Entry point
│   ├── index.html          # HTML template
│   └── vite.config.js      # Vite configuration
│
├── server/                 # Backend Node.js application
│   ├── config/             # Configuration files
│   ├── controllers/        # Request handlers
│   ├── routes/             # API routes
│   ├── utils/              # Utility functions
│   └── index.js            # Entry point
│
└── README.md               # Project documentation
```

## 🔒 Security

- GitHub tokens are not stored in the database
- CORS is configured to only allow requests from the client application
- Sensitive information is stored in environment variables
- Input validation is performed on all endpoints

## 🚢 Deployment

The application is deployed using:
- **Frontend**: [Vercel](https://vercel.com)
- **Backend**: [Vercel](https://vercel.com)

## 👨‍💻 About the Developer

GitHub Repo Remover is a personal project developed by Rakibul Islam. As a developer, I understand the importance of maintaining a clean and organized GitHub profile. I created this tool to make developers' lives easier, including my own.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [GitHub API](https://docs.github.com/en/rest) for providing the API
- [React Icons](https://react-icons.github.io/react-icons/) for the icon library
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework

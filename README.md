# Page Prism - Intuit Front End A4A

## Project Overview

Page Prism is a web application designed to help designers and developers collect and organize visual inspirations for their projects.

## Key Features

- Create and manage design inspiration projects
- Capture screenshots of websites and save them as inspirations
- Organize inspirations within projects
- View and edit project and inspiration details

## Technology Stack

- React 18
- TypeScript
- Vite
- CSS Modules
- React Router
- IndexedDB (via idb library)

## Prerequisites

Before you begin, ensure you have the following installed on your development machine:

1. **Node.js** (version 18.20.2)
   - Download and install from [nodejs.org](https://nodejs.org/)
   - Verify installation: `node --version`

2. **npm** (usually comes with Node.js)
   - Verify installation: `npm --version`

3. **Git**
   - Download and install from [git-scm.com](https://git-scm.com/)
   - Verify installation: `git --version`

3. **Docker**
   - Download and install from [docker.com](https://www.docker.com/)
   - Verify installation: `docker --version`

## Getting Started (web App)

1. Fork the repository:
   - Visit the GitHub repository
   - Click the "Fork" button in the top-right corner to create your own copy of the repository

2. Clone your forked repository:
   ```
   git clone https://github.com/your-username/page-prism.git
   cd page-prism
   ```

3. Install dependencies:
   ```
   npm install
   ```

4. Start the development server:
   ```
   npm run dev
   ```

5. Open your browser and visit `http://localhost:5173` to view the application.

6. Run tests:
   ```
   npm test
   ```

   This will run all the tests in the project using Jest.

7. Run tests in watch mode (for development):
   ```
   npm test -- --watch
   ```

   This will run Jest in watch mode, which will re-run tests when files change.

## Getting Started (genAI)

1. Pull and run docker image
   - `docker pull ollama/ollama`
   - `docker run -it -v ~/ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama`
   - `docker exec -it ollama ollama run tinyllama`

2. Test API server
   - `curl -v --location 'http://localhost:11434/api/generate' --header 'Content-Type: application/json' --data '{"model": "tinyllama","prompt": "why is the sky blue?", "stream": true}'`

## Project Structure

- `/src`: Source code
  - `/components`: Reusable React components
  - `/layouts`: Layout components
  - `/pages`: Page components
  - `/services`: API and data services
  - `/utils`: Utility functions
  - `/models`: TypeScript interfaces and types
  - `/hooks`: Custom React hooks

## Additional Notes

- The project uses IndexedDB for local storage, simulating a backend database
- API calls can be mocked with artificial latency to simulate network requests

## Additional Setup

- **VS Code Extensions** (optional but recommended):
  - ESLint
  - Prettier

- **Environment Setup**:
  - This project uses Node.js version 18.20.2. To ensure you're using the correct version, you can use a version manager like `nvm` (Node Version Manager):
    ```
    nvm use
    ```
  - If you don't have `nvm` installed, you can get it from [here](https://github.com/nvm-sh/nvm).

- **Editor Configuration**:
  - The project includes a `.prettierrc` file for consistent code formatting. Make sure your editor is set up to use Prettier for formatting.


### Run with Gitpod

This app can also be run in Gitpod. We recommend running using Gitpod to build and run this app on the browser. To run this app in Gitpod you will need -
- Github account
- Gitpod Classic account

Click on the below link to open this repository in Gitpod

   [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Intuit-A4A/page-prism)

- Select the IDE of your choice. We recommend `VSCode IDE in browser`
- Standard Configuration
- Click `Continue`

![Screenshot 2024-10-18 at 10 49 59 AM](https://github.com/user-attachments/assets/cf97589f-e84b-48e3-b691-2248c437d884)  

# My Template Project

This is a simple React template project powered by Vite and styled with Tailwind CSS. It serves as a foundation for other projects and includes a basic structure to get started quickly.

## Project Overview

This template project was created by **Mathys Rioux** aka **mstjr**, a web developer. The project includes a minimal setup with React and Tailwind CSS, and a simple UI to indicate that this is a template project.

### Features

- **Vite**: A fast build tool that provides a modern development environment.
- **React**: A JavaScript library for building user interfaces.
- **Tailwind CSS**: A utility-first CSS framework for rapid UI development.
- **Minimal Structure**: Basic HTML and CSS structure to kickstart your projects.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (which includes npm)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mstjr/my-template-project.git
   ```

3. **Navigate to the project directory:**

   ```bash
   cd my-template-project
   ```

4. **Install dependencies:**

   ```bash
   npm install
   ```

### Setting Up Vite with Tailwind CSS

If you want to understand how the project was set up, you can refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs/guides/vite). The basic steps followed were:

1. **Install Vite:**

   ```bash
   npm create vite@latest my-template-project --template react
   cd my-template-project
   ```

2. **Install Tailwind CSS:**

   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   ```

3. **Configure Tailwind to remove unused styles in production:**

   Update `tailwind.config.js` with the following:

   ```javascript
   module.exports = {
     content: [
       "./index.html",
       "./src/**/*.{js,ts,jsx,tsx}",
     ],
     theme: {
       extend: {},
     },
     plugins: [],
   }
   ```

4. **Include Tailwind in your CSS:**

   Add the following to `src/index.css`:

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

### Running the Project

To start the development server, run:

```bash
npm run dev
```

This will open the project in your default web browser. Any changes you make to the source files will automatically refresh the browser.

### Building for Production

To build the project for production, run:

```bash
npm run build
```

This will generate optimized files in the `dist` folder.

### Project Structure

```plaintext
my-template-project/
│
├── src/
│   ├── App.jsx         # Main React component
│   ├── main.jsx        # Entry point for the React app
│   └── index.css       # Tailwind CSS configuration
│
├── public/             # Public assets like index.html
│
├── tailwind.config.js  # Tailwind CSS configuration file
├── vite.config.js      # Vite configuration file
├── package.json        # Project dependencies and scripts
├── README.md           # Project documentation
└── .gitignore          # Files and directories to ignore in Git
```

### Customization

Feel free to customize the project as per your needs. You can modify the existing components or add new ones to build out your application.

Happy coding !

If you have any questions or suggestions, feel free to reach out!

---

Happy coding!

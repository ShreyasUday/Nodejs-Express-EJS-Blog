# Node.js, Express.js, and EJS Blog Website

This is a simple blog website built with Node.js, Express.js for the backend, and EJS (Embedded JavaScript) as the templating engine. It allows users to publish blog posts, which are saved locally in a `posts.json` file.

## Features

* **Create Posts:** Users can write and publish new blog posts.
* **View Posts:** All published posts are displayed.
* **Persistent Storage (Local):** Posts are saved to a `posts.json` file on the server.

---

---

## Project Structure


You are absolutely right! My apologies again. The "Project Structure" in your README.md is not rendering as intended on GitHub.

The issue is that I missed a detail in the specific way the directory tree was formatted; it's using characters like │ and ├── that need to be within a plain text code block to preserve their alignment. When not in a code block, Markdown processors interpret spaces and these characters differently, causing it to look "messed up."

Here's how to fix it:

1. Edit Your README.md File Again 📝
You need to wrap the entire "Project Structure" content with triple backticks (```) to explicitly tell Markdown to render it as a code block.

Open your README.md file locally and make this change:

Locate this section:

Markdown

---

## Project Structure

.
├── public/
│   ├── images/
│   │   └── notepad.png
│   ├── styles/
│   │   └── main.css
├── views/
│   ├── partials/
│   │   ├── footer.ejs
│   │   └── header.ejs
│   ├── about.ejs
│   ├── blog.ejs
│   ├── contact.ejs
│   ├── index.ejs
│   └── saves.ejs
├── index.js          // Main application file
├── package.json      // Project dependencies and scripts
├── posts.json        // Stores blog post data (ignored by Git, but structure shown for clarity)
└── .gitignore        // Specifies files/folders to be ignored by Git
And change it to this:

Markdown

---

## Project Structure

.
├── public/
│   ├── images/
│   │   └── notepad.png
│   ├── styles/
│   │   └── main.css
├── views/
│   ├── partials/
│   │   ├── footer.ejs
│   │   └── header.ejs
│   ├── about.ejs
│   ├── blog.ejs
│   ├── contact.ejs
│   ├── index.ejs
│   └── saves.ejs
├── index.js          // Main application file
├── package.json      // Project dependencies and scripts
├── posts.json        // Stores blog post data (ignored by Git, but structure shown for clarity)
└── .gitignore        // Specifies files/folders to be ignored by Git

## How to Make It Work on Your System

Follow these steps to get the blog website up and running on your local machine:

### Prerequisites

Before you begin, ensure you have the following installed:

* **Node.js**: [Download and Install Node.js](https://nodejs.org/en/download/) (Includes npm - Node Package Manager)

### Installation

1.  **Clone the Repository:**
    Open your terminal or command prompt and clone the repository to your local machine:

    ```bash
    git clone https://github.com/ShreyasUday/Nodejs-Express-EJS-Blog.git
    ```

2.  **Navigate to the Project Directory:**
    ```bash
    cd Nodejs-Express-EJS-Blog
    ```

3.  **Install Dependencies:**
    Install all the required Node.js packages using npm:

    ```bash
    npm install
    ```

4.  **Create `posts.json` (Optional but Recommended):**
    This project uses `posts.json` to store blog data. Since it's ignored by Git, you'll need to create an empty one for the application to work correctly initially.

    Create a file named `posts.json` in the root of your project with the following content:
    ```json
    []
    ```
    This initializes an empty array for your posts.

---

### Running the Application

1.  **Start the Server:**
    Once dependencies are installed, you can start the Node.js server:

    ```bash
    node index.js
    ```
    You should see a message in your terminal indicating that the server is running (e.g., "Server started on port 3000" or whatever port you configured in `index.js`).

2.  **Access the Application:**
    Open your web browser and go to:

    ```
    http://localhost:3000
    ```
    (Adjust the port if your `index.js` uses a different one.)

    You should now see the blog website running locally!

---

## Contributing

If you'd like to contribute, please fork the repository and submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

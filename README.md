# Todo App

A simple Todo application built with Node.js, Express, MongoDB, and EJS.

## Features

- Add tasks to your to-do list.
- View all tasks in a styled interface.
- Edit or remove tasks (future implementation).

## Prerequisites

- [Node.js](https://nodejs.org/) installed on your system.
- A MongoDB database. This app uses MongoDB Atlas, but you can use a local MongoDB instance as well.

## Installation

1. Clone the repository or download the source code.
2. Navigate to the project directory.
3. Install dependencies:

   ```sh
   npm install
   ```

4. Create a `.env` file in the root directory and add your MongoDB connection string:

   ```env
   DB_CONNECT=mongodb+srv://<username>:<password>@cluster0.tklra.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
   ```

   Replace `<username>` and `<password>` with your MongoDB credentials.

## Usage

1. Start the server:

   ```sh
   npm start
   ```

2. Open your browser and navigate to `http://localhost:3000`.

## Project Structure

```
.env
index.js
mongodbinfo.txt
package.json
models/
    TodoTask.js
public/
    stylesheets/
        style.css
views/
    todo.ejs
```

- `index.js`: Main server file.
- `models/TodoTask.js`: Mongoose schema for the Todo tasks.
- `public/stylesheets/style.css`: CSS for styling the app.
- `views/todo.ejs`: EJS template for rendering the Todo list.

## Dependencies

- [Express](https://expressjs.com/) - Web framework for Node.js.
- [Mongoose](https://mongoosejs.com/) - MongoDB object modeling tool.
- [EJS](https://ejs.co/) - Embedded JavaScript templating.
- [dotenv](https://github.com/motdotla/dotenv) - Loads environment variables from `.env` file.
- [Nodemon](https://nodemon.io/) - Development tool for automatically restarting the server.

## License

This project is licensed under the MIT License.

Here's the `README.md` file for your MERN project:

```markdown
# MERN Stack with MySQL Server

This project implements a MERN stack application to add anonymous comments. The backend uses Node.js with TypeScript, Express, and MySQL for the database. The MySQL server is containerized and should be launched using Docker. The frontend, located in the `client` folder, was created using the `create-react-app` command and includes a separate `README.md` file with additional instructions.

## Getting Started

### Prerequisites

- Node.js and npm
- Docker (to run the MySQL server)
- TypeScript (installed globally or locally)

### Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/bhuvinsingla/MERN-Project.git
   cd MERN-Project
   ```

2. **Install Dependencies**
   Navigate to both the root directory and the `client` folder, and install the required dependencies:
   ```bash
   npm install
   cd client
   npm install
   cd ..
   ```

3. **Set Up the Environment**
   Create a `.env` file in the root directory with the following configuration:
   ```env
   DB_HOST=<your-database-host>
   DB_USER=<your-database-user>
   DB_PASSWORD=<your-database-password>
   DB_NAME=<your-database-name>
   PORT=4000
   ```

4. **Start the MySQL Server with Docker**
   ```bash
   docker run --name mysql-server -e MYSQL_ROOT_PASSWORD=<your-password> -e MYSQL_DATABASE=<your-database> -p 3306:3306 -d mysql:latest
   ```

5. **Run Migrations**
   If your project includes database migration scripts, ensure to execute them before starting the application.

## Available Scripts

In the project directory, you can run:

### `npm run dev`

Starts the application in development mode.  
This uses the `concurrently` package to watch TypeScript files and start the backend with `nodemon`.

```bash
npm run dev
```

- Backend URL: [http://localhost:4000](http://localhost:4000)

### `npm run test`

Currently, this script outputs an error indicating no tests are specified.

### `npm run build`

Builds the TypeScript backend code into JavaScript in the `build` folder.

```bash
npm run build
```

## Frontend Setup

The frontend resides in the `client` folder. Refer to the `README.md` file in the `client` directory for further instructions.

## Deployment

To deploy this application, ensure you:

1. Build the frontend and serve the static files.
2. Deploy the backend server with proper configurations.
3. Configure the MySQL database for the production environment.

## Contributing

Feel free to fork this repository and submit pull requests for enhancements and bug fixes.

## License

This project is licensed under the [MIT License](LICENSE).
```

This file includes a comprehensive setup guide, script explanations, and deployment instructions. Let me know if you want to add or modify anything!

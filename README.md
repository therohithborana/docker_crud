# Simple CRUD App with MongoDB and Mongo Express

## Overview
This is a simple CRUD (Create, Read, Update, Delete) application built with:
- **Node.js** for the backend.
- **MongoDB** for the database.
- **Mongo Express** for database management.
- **Docker** for containerization.

The application allows you to perform basic CRUD operations on items stored in a MongoDB database.

## Features
- **Create**: Add new items with a name and description.
- **Read**: View all items or a single item by ID.
- **Update**: Edit existing items.
- **Delete**: Remove items from the database.

## Prerequisites
- Docker
- Docker Compose

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/therohithborana/docker_crud.git
   ```

3. Navigate to the project directory:
   ```bash
   cd docker_crud
   ```
      or run the command
   ```bash
   curl -o mongodb.yaml https://raw.githubusercontent.com/therohithborana/docker_crud/main/mongodb.yaml
``
4. Start the application using Docker Compose:
   ```bash
   docker-compose -f mongodb.yaml up -d
   ```
5. Access the application:
   - **Node.js App**: [http://localhost:3000](http://localhost:3000)
   - **Mongo Express**: [http://localhost:8081](http://localhost:8081)

## How to Stop
To stop the application, run:
```bash
docker-compose -f mongodb.yaml down
```

## Project Structure
```
docker_crud/
├── server.js
├── package.json
├── public/
│   ├── index.html
│   └── styles.css
├── Dockerfile
├── mongodb.yaml
├── .dockerignore
└── README.md
```

## Docker Hub
The Node.js app image is available on Docker Hub:
```bash
docker pull therohithborana/crud
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. 

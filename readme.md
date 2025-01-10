
---

# Node.js, PostgreSQL, and Redis Docker Setup

This setup provides a containerized environment for a Node.js application, PostgreSQL database, and Redis. Follow the steps below to configure and start the environment.

---

## **Environment Variables**

Before starting, configure the following environment variables in your `.env` file or export them in your terminal:

```env
DB_USER=USER       # Replace 'USER' with your PostgreSQL username
DB_PASSWORD=PASSWORD   # Replace 'PASSWORD' with your PostgreSQL password
DB_NAME=DATABASE   # Replace 'DATABASE' with your PostgreSQL database name
```

---

## **Usage**

1. **Build and Start Containers**  
   Run the following command to build and start the containers:  

   ```bash
   docker-compose up --build
   ```

   This command will:
   - Build the Docker images for Node.js, PostgreSQL, and Redis.
   - Start the containers with the configurations provided in the `docker-compose.yml` file.
   - Initialize the PostgreSQL container with the specified `DB_USER`, `DB_PASSWORD`, and `DB_NAME` provided in the environment variables.

2. **Verify Setup**  
   Once the containers are running:
   - The Node.js application will be accessible at its configured port.
   - PostgreSQL and Redis will be available for use within the Docker network.

---

## **Features**
- PostgreSQL is preconfigured with the specified user, password, and database.
- Redis is available for caching or session management.
- Node.js is ready for application development with database and caching support.

---
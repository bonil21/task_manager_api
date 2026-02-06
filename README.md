Task Manager API 


Clone and navigate – Clone the GitHub repository and enter the project folder containing Symfony files (bin, config, src, .env).

Start Docker – Make sure Docker Desktop is running, then launch the MySQL container (task_manager_db) on port 3307.

Install dependencies – Run Composer to install PHP packages, including Symfony and API Platform.

Configure database – Verify the DATABASE_URL in .env (user: root, password: root, database: task_manager_api, port: 3307).

Set up tables – Execute Doctrine migrations to create the database schema.

Run Symfony server – Start the server at [(http://localhost:8000](http://127.0.0.1:8000).

Access the API – [http://localhost:8000/api](http://127.0.0.1:8000/api)
 to view documentation and test endpoints.

Basic operations –

POST /api/tasks → create a new task

PATCH /api/tasks/{id} → update a task

Set isCompleted=true → mark a task as completed

Verify database – Inspect tables using any MySQL client or Symfony commands.

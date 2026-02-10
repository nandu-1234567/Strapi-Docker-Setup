<!DOCTYPE html>
<html>
<head>
  <title>TASK-3 Dockerized Strapi Setup</title>
</head>
<body>

<h1>TASK-3: Dockerized Strapi with PostgreSQL and Nginx</h1>

<h2>Step 1: Install Required Tools</h2>
<ol>
  <li>Install Docker Desktop</li>
  <li>Install Git</li>
  <li>Install Node.js (for creating Strapi app)</li>
</ol>

<h2>Step 2: Create Project Directory</h2>
<ol>
  <li>Create a main project folder</li>
  <li>Inside it, create folders for nginx and Strapi</li>
</ol>

<h2>Step 3: Create User-Defined Docker Network</h2>
<ol>
  <li>Create a Docker network named <b>strapi-net</b></li>
  <li>Verify that the network is created successfully</li>
</ol>

<h2>Step 4: Create Strapi Application</h2>
<ol>
  <li>Create a new Strapi application inside the project</li>
  <li>Ensure Strapi runs on port 1337</li>
</ol>

<h2>Step 5: Configure PostgreSQL Container</h2>
<ol>
  <li>Set PostgreSQL username</li>
  <li>Set PostgreSQL password</li>
  <li>Set PostgreSQL database name</li>
  <li>Attach PostgreSQL container to strapi-net</li>
</ol>

<h2>Step 6: Configure Strapi to Use PostgreSQL</h2>
<ol>
  <li>Set database client as PostgreSQL</li>
  <li>Set database host as postgres service name</li>
  <li>Set database port to 5432</li>
  <li>Provide database name, username, and password</li>
  <li>Attach Strapi container to strapi-net</li>
</ol>

<h2>Step 7: Configure Nginx Reverse Proxy</h2>
<ol>
  <li>Create nginx configuration file</li>
  <li>Configure Nginx to listen on port 80</li>
  <li>Proxy requests from localhost to Strapi on port 1337</li>
  <li>Attach Nginx container to strapi-net</li>
</ol>

<h2>Step 8: Docker Compose Setup</h2>
<ol>
  <li>Define PostgreSQL service</li>
  <li>Define Strapi service</li>
  <li>Define Nginx service</li>
  <li>Ensure all services use the same Docker network</li>
</ol>

<h2>Step 9: Start Containers</h2>
<ol>
  <li>Run Docker Compose to start all containers</li>
  <li>Verify all containers are running</li>
</ol>

<h2>Step 10: Access Strapi Admin Panel</h2>
<ol>
  <li>Open browser</li>
  <li>Access <b>http://localhost/admin</b></li>
  <li>Confirm Strapi Admin Dashboard loads successfully</li>
</ol>





</body>
</html>

# compose-exercise-drupal

## Assignment: Write a Docker Compose File to Deploy Drupal

The goal of this assignment is to develop a `compose.yml` file from scratch to deploy a Drupal application and its database, ensuring that all components work seamlessly together. This will test your understanding of Docker Compose syntax, service orchestration, and the interaction between services.

## Instructions

1. **Understand the Requirements**
   - You need to deploy a Drupal website using Docker Compose.
   - The setup requires:
     - A Drupal service that runs on Apache.
     - A PostgreSQL database service to store Drupal's data.
   - The Drupal container should:
     - Expose port `8083` on the host machine.
     - Use volumes to persist modules, themes, profiles, and site-specific data.
   - The PostgreSQL container should:
     - Have a secure password set via an environment variable.
   - Both services should restart automatically in case of failure.

2. **Write the Compose File**
   - Create a `compose.yml` file that meets the above requirements.

3. **Test Your Setup**
   - Run the services by executing:
     ```bash
     docker compose up
     ```
   - Ensure that:
     - Drupal is accessible in your browser at `http://localhost:8083`.
     - There are no errors during container startup.
     - The Drupal setup screen loads, indicating a connection to the database.

# WordPress + Bedrock + Docker

A nice local dev env using [WordPress](https://wordpress.org/), [Roots/Bedrock](https://roots.io/bedrock/) and [Docker](https://www.docker.com/).  
Making it easy to version control and maintain your next wp theme or plugin.

You need [Docker Desktop](https://www.docker.com/get-started) and [Composer](https://getcomposer.org/download/) installed to use this setup.

### Getting started

1. Rename the container names in `docker-compose.yml` to your needs.

2. Go to the bedrock folder and make a copy of `.env.example`, name it `.env` and enter your credentials. You can keep most of what's in there already.

3. Run `composer update` in the bedrock folder.  
   **Note:** If you are not using ACF Pro, simply remove this dependency from `composer.json`, both under "repositories" and under "require".

4. Open a new tab in your terminal at the root of the project and start the local dev env: `docker compose up`

5. Install WordPress by going to http://localhost:8080

6. Open a new tab in your terminal and shut down: `docker compose down`

### End points

Login page: [http://localhost:8080/wp/wp-login.php](http://localhost:8080/wp/wp-login.php)

Wp admin: [http://localhost:8080/wp/wp-admin/](http://localhost:8080/wp/wp-admin/)

### Credits

❤️ Big thanks to [@Jitesoft](https://github.com/jitesoft) for their contribution with the Docker part of this setup.

# dockerpress

This is a simple local development environment for WordPress using Docker Compose. It consists of two services, a MySQL database and a WordPress web server.

## Requirements

- Docker Engine
- Docker Compose

## Usage

1. Clone this repository to your local machine
2. Navigate to the cloned directory
3. Start the environment with `docker-compose up -d`
4. Access the WordPress site at `http://localhost:8000`

## Configuration

The environment can be configured by modifying the `docker-compose.yml` file. The following configuration options are available:

### Database

The `db` service is responsible for the MySQL database. It can be configured with the following environment variables:

- `MYSQL_ROOT_PASSWORD`: The root password for the MySQL server
- `MYSQL_DATABASE`: The name of the WordPress database
- `MYSQL_USER`: The username for the WordPress database
- `MYSQL_PASSWORD`: The password for the WordPress database

### WordPress

The `wordpress` service is responsible for the WordPress web server. It can be configured with the following environment variables:

- `WORDPRESS_DB_HOST`: The hostname of the MySQL server
- `WORDPRESS_DB_USER`: The username for the WordPress database
- `WORDPRESS_DB_PASSWORD`: The password for the WordPress database
- `WORDPRESS_DB_NAME`: The name of the WordPress database

## Contributing

If you find a bug or have an idea for a new feature, please open an issue or pull request on the [GitHub repository](https://github.com/vorniches/dockerpress).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

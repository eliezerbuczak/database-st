# Database

## Installation

### Requirements

- Docker
- Docker Compose
- Git
- Linux (recommended Ubuntu 20.04 or higher)

### Installation

1. Clone the repository

```bash
git clone <repository-url>
```

2. Go to the project directory

```bash
cd <project-directory>
```

3. Configure the docker-compose.yml file

```bash
sudo nano docker-compose.yml
```

4. Run the docker-compose.yml file

```bash
sudo docker-compose up -d
```

### Usage

1. Open DataGrip or any other database management tool

2. Connect to the database

- Host: `localhost` or ip address
- Port: `3306` (default) or port specified in docker-compose.yml file
- User: `root` (default) or user specified in docker-compose.yml file
- Password: `root` (default) or password specified in docker-compose.yml file

3. Aceess the database

- Database: `database` (default) or database specified in docker-compose.yml file

4. Create a new table

```sql
CREATE TABLE `table` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(255) NOT NULL,
  `password` varchar(255) NOT NULL,
    PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;
```


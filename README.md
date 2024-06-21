# Distributed System Project : Movie Booking App

This project is a ticket booking system where users can book tickets for movies. The application fetches movie, theater, and show information from an external API and stores it in a MySQL database. It utilizes Python, Django, Docker, JavaScript, HTML, CSS, and MySQL for implementation.

## Aim

- **Client Server Communication**: Implemented using RPC and Socket programming
- **Multi Threading**: Implemented Multi-threading by using thread pool executer. Celery to integrate with multi-threading for task scheduling and execution.
- **Clock Synchronization**: Implemented clock sychronization using lamport's clock
- **Data Consistency**: Implemented semaphores, mutex locks for consistency
- **Data Replication**: Designed Master slave architecture for replication purpose across multiple containers.
- **Election Algorithm**: Used Bully Algorithm for the election process of the master.
- **Load Balancing**: Used Nginx and Docker for load balancing & deployment

## Features

- **Ticket Booking**: Users can browse available movies, select showtimes, and book tickets.
- **API Integration**: Movie, theater, and show information is fetched from an external API.
- **Data Storage**: Information retrieved from the API is stored in a MySQL database.
- **Concurrency Handling**: Mutexes, locks, and semaphores are implemented to ensure data consistency, especially in scenarios with multiple concurrent requests.
- **Containerization**: Docker is used for containerization, enabling easy deployment and running multiple instances of the application.
- **Web Interface**: A user-friendly web interface is provided for users to interact with the system.

## Technologies Used

- **Python**: Backend development and logic implementation.
- **Django**: Web framework for building the application.
- **Docker**: Containerization for easy deployment and scalability.
- **JavaScript, HTML, CSS**: Frontend development for the web interface.
- **MySQL**: Database for storing movie, theater, and booking information.
- **Nginx**: Web server for serving static files and reverse proxying to Django.

## Setup Instructions

1. Clone the repository:

    ```
    git clone https://github.com/your_username/bookmyshow.git
    ```

2. Navigate to the project directory:

    ```
    cd bookmyshow
    ```

3. Build and run Docker containers:

    ```
    docker-compose up --build
    ```

4. Access the application via a web browser at `http://localhost:8000`.

Commands to run:
1) docker compose build
2) docker compose up -d
3) docker ps

To stop project:

docker stop $(docker ps -a -q)

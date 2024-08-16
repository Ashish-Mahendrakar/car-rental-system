# Car Rental System

This project is a simple console-based Car Rental System written in C++. It connects to a MySQL database to manage car rentals, check availability, and update rental statuses. 

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Introduction

The Car Rental System allows users to view available cars and rent them if they are not already booked. The system is designed to be simple and easy to use, with a minimal interface and a focus on core functionality.

## Features

- Display available cars from the MySQL database.
- Rent a car by selecting its serial number.
- Update car availability status in the database.
- Handle multiple car entries in the database.
- Error handling for database operations.

## Installation

### Prerequisites

- **C++ Compiler**: Ensure you have a C++ compiler like GCC or MSVC installed.
- **MySQL Server**: A running instance of MySQL Server.
- **MySQL Connector/C++**: The MySQL Connector/C++ library for C++ database access.

### Steps

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/car-rental-system.git
    cd car-rental-system
    ```

2. **Set up MySQL Database**:
    - Create a database named `mydb`.
    - Create a table `cars` with the following structure:

    ```sql
    CREATE TABLE cars (
        Serial INT PRIMARY KEY,
        Brand VARCHAR(50),
        Model VARCHAR(50),
        Rent INT,
        Avail BOOLEAN
    );
    ```

    - Update the `DB`, `USER`, `PW`, and `HOST` variables in the source code to match your MySQL setup.



## Usage

- Once the program is running, it will display all available cars from the database.
- You can select a car to rent by entering its serial number.
- The system will check the availability and update the database accordingly.
- You can exit the program by selecting the exit option.


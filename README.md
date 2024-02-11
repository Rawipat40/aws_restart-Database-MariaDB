# AWS EC2 and MariaDB Setup and Usage

This guide provides an overview of setting up and using AWS EC2 (Elastic Compute Cloud) instances with MariaDB, along with insights into performing various database operations.

## Prerequisites

- Access to an AWS account
- Basic understanding of AWS EC2 and MariaDB concepts
- Familiarity with the Linux command line

## Setup

1. **Launch an AWS EC2 Instance:**

    Launch a new EC2 instance with your desired specifications, such as instance type, operating system (e.g., Amazon Linux), and security group settings.

2. **Install and Configure MariaDB:**

    Connect to your EC2 instance via SSH and install MariaDB using the package manager appropriate for your Linux distribution (e.g., `yum` for Amazon Linux).

## Usage

1. **Create a Database and Tables:**

    Use the MySQL client (`mysql`) to connect to the MariaDB server and create databases and tables as needed. For example:

    ```sql
    CREATE DATABASE my_database;
    USE my_database;

    CREATE TABLE users (
        id INT AUTO_INCREMENT PRIMARY KEY,
        username VARCHAR(50) NOT NULL,
        email VARCHAR(100) NOT NULL
    );
    ```

2. **Update Data:**

    Modify existing data in the tables using the `UPDATE` statement. For example:

    ```sql
    UPDATE users SET email='new_email@example.com' WHERE id=1;
    ```

3. **Delete Data:**

    Remove records from tables using the `DELETE` statement. For example:

    ```sql
    DELETE FROM users WHERE id=1;
    ```

4. **Query Tables:**

    Retrieve data from tables using the `SELECT` statement. For example:

    ```sql
    SELECT * FROM users;
    ```

5. **Inner Join Tables:**

    Perform inner joins between tables to retrieve related data. For example:

    ```sql
    SELECT users.username, orders.order_id
    FROM users
    INNER JOIN orders ON users.id = orders.user_id;
    ```

## What I Have Learned

Through setting up and using AWS EC2 with MariaDB, I have learned the following:

- **EC2 Instance Management:**
  - Provisioning and configuring EC2 instances, including security group settings and instance types.

- **MariaDB Installation and Configuration:**
  - Configuring remote access to MariaDB.

- **Database Operations:**
  - Creating databases and tables using SQL commands.
  - Updating, deleting, and querying data in MariaDB tables.
  - Performing inner joins to retrieve data from related tables.

- **Remote Server Administration:**
  - Managing an EC2 instance remotely via SSH.
  - Executing SQL commands and managing databases using the MySQL client.

## Conclusion

By leveraging AWS EC2 instances with MariaDB, you can create scalable and flexible database solutions in the cloud. Understanding the setup and usage of these technologies, along with database operations, provides valuable insights into cloud-based database management and administration.

For more advanced configurations and optimizations, refer to the AWS and MariaDB documentation, and explore additional features and services available in the AWS ecosystem.

##

![MariaDB1](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/f5a4b167-50bc-4ce5-b0f9-ee9879a8babb)

![MariaDB2](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/eaf885a7-5a50-4d7b-92c8-284e7ae2f594)

![MariaDB3](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/37564f1c-5bf2-47f8-be48-41883a1eb874)

![MariaDB4](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/202e5ad2-c57b-45be-aac2-ad238bc2512b)

![MariaDB5](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/02e189c5-f8d5-4368-b311-34c4f0072fe7)

![MariaDB6](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/f94308f8-0323-4276-8f20-f870075b4d4b)

![MariaDB7](https://github.com/Rawipat40/aws_restart-Database-MariaDB/assets/141838218/b5ef943d-714a-4fe1-b455-c8eb47f805da)





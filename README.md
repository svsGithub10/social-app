# KodBook

KodBook is a social media application designed to connect users through posts, comments, and interactions. This README provides an overview of the project, instructions for setting up the development environment, and details on configuring the database.

## Features

- **User Registration and Authentication**: Secure sign-up and login functionalities.
- **Post Creation**: Users can create and share posts with text and images.
- **Commenting**: Engage with posts through comments.
- **User Profiles**: View and edit personal profiles.
- **Follow System**: Follow other users to see their posts in your feed.

## Technologies Used

- **Backend**: Spring Boot
- **Frontend**: HTML, CSS
- **Database**: MySQL

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Database
- Maven

### Installation

1. **Clone the Repository**:

   ```bash
   git clone http://github.com/svsGithub10/social-app.git
   cd social-app
   ```

2. **Configure the Database**:

   - Create a new MySQL database:

     ```sql
     CREATE DATABASE kodbook_db;
     ```

   - Update `src/main/resources/application.properties` with your database credentials:

     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/kodbook_db
     spring.datasource.username="your_username"
     spring.datasource.password="your_password"
     spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
     spring.jpa.hibernate.ddl-auto=update
     ```

     Ensure that the `spring.jpa.hibernate.ddl-auto` property is set to `update` to automatically synchronize the database schema with the entity models.

3. **Build and Run the Application**:

   - Use Maven to build the project:

     ```bash
     mvn clean install
     ```

   - Run the application:

     ```bash
     mvn spring-boot:run
     ```

     The application should now be running on `http://localhost:8080/`.

## Contributing

We welcome contributions to enhance KodBook. To contribute:

1. Fork the repository.
2. Create a new branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Make your changes and commit them:

   ```bash
   git commit -m 'Add some feature'
   ```

4. Push to the branch:

   ```bash
   git push origin feature/your-feature-name
   ```

5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For more information, visit the [KodBook repository](http://github.com/svsGithub10/social-app).

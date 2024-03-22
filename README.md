# GritAcademy API

This project is a Java Spring Boot API that provides fictional data about students and courses for the GritAcademy. The API allows users to retrieve information about students, courses, and associations between them.

## Technologies Used
- Java
- Spring Boot
- MySQL
- JPA (Java Persistence API)
- Lombok
- RESTful API principles

## Getting Started

### Prerequisites
- Java Development Kit (JDK)
- Maven
- MySQL

### Installation
1. Clone this repository.
2. Set up MySQL database and configure connection properties in `application.properties`.
3. Build and run the project using Maven.

## API Endpoints

The API provides the following endpoints:

- `GET /api/students/all`: Retrieve all students.
- `GET /api/students/allAssociations`: Retrieve all associations between students and courses.
- `GET /api/students/searchCoursesByStudentId?id={studentId}`: Search courses by student ID.
- `GET /api/students/by-fname?fName={firstName}`: Get students by first name.
- `GET /api/students/by-lname?lName={lastName}`: Get students by last name.
- `GET /api/students/by-town?town={townName}`: Get students by town.
- `POST /api/students`: Add a new student.
- `DELETE /api/students/deleteStudentById?id={studentId}`: Delete a student by ID.
- `POST /api/students/addStudentToCourse?studentId={studentId}&courseId={courseId}`: Add a student to a course.
- `DELETE /api/students/removeStudentFromCourse?studentId={studentId}&courseId={courseId}`: Remove a student from a course.

- `GET /api/courses/all`: Retrieve all courses.
- `GET /api/courses/searchStudentsByCourseId?id={courseId}`: Search students by course ID.
- `GET /api/courses/by-name-keyword?keyword={keyword}`: Get courses by keyword in name.
- `GET /api/courses/by-description-keyword?keyword={keyword}`: Get courses by keyword in description.
- `POST /api/courses`: Add a new course.
- `DELETE /api/courses/deleteCourseById?id={courseId}`: Delete a course by ID.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request.



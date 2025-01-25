EpitomeHub E-commerce Website

Overview

This is a complete e-commerce platform developed to provide functionality similar to popular platforms like Flipkart and Amazon. It includes backend services, frontend design, Docker configuration, CI/CD pipelines, and deployment scripts for cloud environments.

Features

User Account Management:

Registration, Login, and Forgot Password functionalities.

Secure authentication using JWT.

Product Management:

Product showcase with search and filter options.

Detailed product pages with descriptions, images, and reviews.

Shopping Cart & Orders:

Add/remove items from the cart.

Checkout process with address and payment options.

Order history and status tracking.

Customer Reviews:

Review and rating system for products.

Responsive UI:

Mobile and desktop-friendly design using React and Bootstrap.

Technology Stack

Frontend: React, TypeScript, Bootstrap

Backend: Spring Boot Microservices

Database: MySQL (or MongoDB)

Containerization: Docker and Docker Compose

Deployment: AWS (ECS, RDS, and Load Balancer)

CI/CD: GitHub Actions

Project Structure

shoppingcart/
├── backend/           # Spring Boot backend services
├── frontend/          # React frontend application
├── .github/workflows/ # CI/CD pipeline configuration
├── docker-compose.yml # Docker Compose for local and cloud deployments
└── README.md          # Project documentation

Setup Instructions

Backend

Navigate to the backend directory:

cd backend

Build the backend project:

mvn clean package

Run the application:

java -jar target/ecommerce.jar

Frontend

Navigate to the frontend directory:

cd frontend

Install dependencies:

npm install

Start the application:

npm start

Docker

Build and run the entire application with Docker:

docker-compose up --build

Deployment

AWS RDS:

Set up a MySQL instance for the backend.

Update application.properties with RDS credentials.

AWS ECS:

Push Docker images to a container registry (e.g., Docker Hub).

Deploy the images to ECS using the provided deployment script.

CI/CD:

GitHub Actions pipeline automates build, test, and deployment steps.

Contributing

Fork the repository.

Create a feature branch:

git checkout -b feature-branch

Commit your changes:

git commit -m 'Add new feature'

Push the branch:

git push origin feature-branch

Create a pull request.

License

This project is licensed under the MIT License.

Contact

For any inquiries, reach out to EpitomeHub.
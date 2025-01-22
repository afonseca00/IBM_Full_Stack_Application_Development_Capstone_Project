# IBM_Full_Stack_Application_Development_Capstone_Project

# Fullstack Developer Capstone Project - Dealerships Review Portal

## Overview

This project is the final capstone for the **Fullstack Software Developer** certification course. The goal of this project is to develop a web application for a national car dealership with branches across the United States, enabling users to view dealership information and leave reviews for each branch. This project leverages various technologies, including **Django**, **React**, **Node.js**, **MongoDB**, **Docker**, and **IBM Cloud**.

### Project Background

A market survey conducted by the car dealership company revealed a strong interest from customers in a centralized platform where they could view reviews of dealerships nationwide. The goal is to provide transparency and increase customer trust in the dealership network by enabling users to read reviews and submit their own.

### Key Features

- **Anonymous Users**: View dealership details and reviews.
- **Authorized Users**: Log in, submit reviews, and view reviews for each dealership.
- **Admin Users**: Manage dealership information, including adding car makes, models, and other attributes.
- **Sentiment Analysis**: Analyze the sentiment of customer reviews using an IBM Cloud-based sentiment analyzer service.

## Technologies Used

- **Django**: Backend web framework to manage dealership data, user authentication, and reviews.
- **React**: Frontend framework for building dynamic user interfaces.
- **Node.js**: Server to handle dealership and review data with MongoDB.
- **MongoDB**: Database used to store dealership and review data.
- **Docker**: Containerization technology for packaging the application and services.
- **IBM Cloud Code Engine**: Cloud platform to deploy the sentiment analysis service.
- **CI/CD**: Continuous Integration and Continuous Deployment pipeline for efficient code management and delivery.

## Architecture

The solution architecture consists of the following components:

1. **Dealerships Website (Django)**:
   - Microservices for managing dealerships, car models, reviews, and user authentication.
   - Interaction with a MongoDB database through a proxy service.

2. **Dealerships and Reviews Service (Node.js/Express)**:
   - Microservice to handle CRUD operations for dealers and reviews.
   - Hosted in a Docker container for easy deployment.

3. **Sentiment Analyzer (IBM Cloud Code Engine)**:
   - Analyzes the sentiment of review text (positive, negative, or neutral).

4. **Database**:
   - **SQLite** for storing car make and model data in Django.
   - **MongoDB** for storing dealer and review data in the Node.js service.

## User Stories

### Anonymous Users
- View the **Contact Us** and **About Us** pages.
- View a list of dealerships across the United States, with the ability to filter by state.
- View reviews for each dealership.

### Authorized Users
- In addition to anonymous features, authorized users can:
  - Submit reviews for any dealership.
  - Submit a review which will appear at the top of the list of reviews on the dealership detail page.

### Admin Users
- Log into the admin interface to manage dealership data.
- Add new makes, models, and other attributes for dealerships.

## Installation Instructions

1. **Clone the repository**:

   ```bash
   git clone https://github.com/afonseca00/IBM_Full_Stack_Application_Development_Capstone_Project.git
   cd fullstack_developer_capstone

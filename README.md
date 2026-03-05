# Culinary Recipes Management System

## Overview

This project is a backend web application developed for managing culinary recipes.  
The system allows storing, retrieving and managing recipes together with their ingredients and preparation instructions.

The application is built using Java and Spring Boot, following a layered architecture and exposing REST APIs that allow interaction with the recipe database.

In addition to basic recipe management, the system includes a feature that helps users discover recipes based on the ingredients they already have available.

---

## Technologies Used

- Java
- Spring Boot
- Spring Web
- Spring Data JPA (Hibernate)
- Maven
- H2 Database
- REST API

---

## Architecture

The application follows a standard Spring Boot layered architecture:

**Controller Layer**  
Handles HTTP requests and exposes REST API endpoints.

**Service Layer**  
Contains the business logic for managing recipes and processing ingredient-based searches.

**Repository Layer**  
Manages database interaction using JPA repositories.

**Database Layer**  
Stores recipes, ingredients and related culinary data.

---

## Features

The system provides functionality for managing recipes and culinary data, including:

- Creating new recipes
- Retrieving recipe information
- Updating existing recipes
- Deleting recipes
- Managing recipe ingredients
- Searching recipes based on available ingredients

---

## Ingredient-Based Recipe Search

One of the main features of the system allows users to search for recipes based on the ingredients they already have at home.

The user provides a list of available ingredients, and the system compares them with the ingredients required for each recipe stored in the database.

Recipes are then ranked based on the number of matching ingredients.  
The recipes that share the highest number of common ingredients with the user's input are returned first, helping users quickly identify meals they can prepare with minimal additional ingredients.

This feature demonstrates basic recommendation logic and ingredient matching.

---

# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system that separates an application into two main parts that work together. In this project, the two tiers are the Web/Application Tier, which runs Nextcloud, and the Database Tier, which uses MariaDB to store the application's data.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the application that users access through a web browser. In this project, Nextcloud serves as the web application and handles HTTP requests from users. It provides the interface for accessing and managing files in the private cloud storage system.

## The Database Tier

The Database Tier is responsible for storing and managing persistent information needed by the application. MariaDB is used in this project as the database for Nextcloud. It stores information such as user accounts, configuration information, and file metadata.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container has a specific responsibility, so the application and database can be updated, restarted, or managed separately without putting everything inside one container.


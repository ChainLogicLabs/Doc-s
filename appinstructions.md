# Data Aggregator API User Guide

## Introduction

The Data Aggregator API is a crucial component of the Trust and Verification System. It facilitates the aggregation of data from various trusted sources, supporting the creation of a robust and reliable data bank. This user guide outlines the functionalities and usage of the Data Aggregator API.

## Table of Contents

1. [API Endpoints](#1-api-endpoints)
    - 1.1 [Welcome Endpoint](#11-welcome-endpoint)
    - 1.2 [News Endpoint](#12-news-endpoint)
    - 1.3 [Specific Newspaper Endpoint](#13-specific-newspaper-endpoint)
2. [Usage](#2-usage)
    - 2.1 [Retrieve Data](#21-retrieve-data)
    - 2.2 [Retrieve Specific Newspaper Data](#22-retrieve-specific-newspaper-data)

## 1. API Endpoints

### 1.1 Welcome Endpoint

- **Endpoint:** `/data`
- **Method:** `GET`
- **Description:** Returns a welcome message indicating successful API connection.

### 1.2 News Endpoint

- **Endpoint:** `/news`
- **Method:** `GET`
- **Description:** Retrieves aggregated news articles from multiple newspapers.

### 1.3 Specific Newspaper Endpoint

- **Endpoint:** `/news/:newspaperId`
- **Method:** `GET`
- **Parameters:** `newspaperId` (string) - Name of the specific newspaper
- **Description:** Retrieves aggregated news articles from a specific newspaper.

## 2. Usage

### 2.1 Retrieve Data

1. Make a GET request to the `/news` endpoint to retrieve aggregated news articles from all newspapers.

2. Optionally, specify a newspaper by making a GET request to `/news/:newspaperId` with the desired `newspaperId`.

### 2.2 Retrieve Specific Newspaper Data

1. Make a GET request to `/news/:newspaperId`, replacing `:newspaperId` with the name of the specific newspaper (e.g., `/news/MoneyLion`).

2. Receive aggregated news articles from the specified newspaper.

Note: Regularly check for updates or changes in API endpoints and parameters.

The Data Aggregator API serves as a reliable source for aggregated news articles, providing users with up-to-date and verified information for making informed decisions.
## SPRINT 4

### Introduction to API 
- **Application Architecture**
- **What is an API**
- **Architectural Solutions**:
  - REST
- **HTTP**:
  - Request and Response Structure
- **JSON**

### API Testing with Postman
- **Basic Features**
- **API Testing**
- **Dynamic URL in Postman**
- **cURL and Generating Request for cURL**
- **Database and API**
- **Bug Reporting for API**
- **API Logs**
- **API Documentation**:
  - Swagger
  - Apidoc

### API Test Design
- **Positive Tests**
- **Negative Tests**
- **Equivalence Classes**
- **Boundary Values**
- **API Validation**
- **API Testing Checklist**



# Urban.Grocers API - Testing New Features

This repository contains the testing details and reports for the new functionality added to the Urban.Grocers API. The focus is on back-end testing of features related to kit management and delivery services.

## Overview

A new version of the Urban.Grocers API has been released for testing, featuring the following key functionalities:

- **Kit Management**: Ability to add products to a kit via the endpoint:
  - **POST** `/api/v1/kits/{id}/products`
  - Limitation: The length of the resulting product list (not the cumulative quantities of each product) cannot exceed 30. A `400 Bad Request` will be returned if this limit is exceeded.

- **Delivery Services (Order and Go)**: Check the availability and cost of delivery using the endpoint:
  - **POST** `/order-and-go/v1/delivery`
  - Refer to the "Couriers" section of the apiDoc for delivery price calculation requirements.

## Testing Tasks

### 1. Requirement Analysis
- Study the API documentation (apiDoc) to understand the details of the new functionality and the back-end requirements.

### 2. Test Design
- Create a detailed checklist of functionalities to be tested. The checklist was developed and shared in a [Google Spreadsheet](#).
- The checklist includes test cases such as:
  - Adding products to kits with different list sizes.
  - Verifying availability and correct price calculation in the "Order and Go" service.

### 3. Testing in Postman
- The API was tested using **Postman** to ensure the new features work as expected.
- Expected behavior in response to various inputs and scenarios was validated.

### 4. Bug Reporting
- If any bugs are identified during testing, reports are created in **Jira**, detailing the reproduction steps, expected behavior, and actual behavior.

### 5. Test Report
- A final test report will be compiled for the development team, providing insights into the status of the tested features, any failures, and recommendations.


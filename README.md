# Lecturer Claim Register

This is a small ASP.NET Core MVC application for managing lecturer claim drafts. It allows users to view existing claims and add new claims. The claims are stored in an in-memory list, so no database is used.

## MVC

**Model:**  
The `Claim` model stores the claim details such as the lecturer name, module code, hours worked, hourly rate, month and status. It also calculates the total amount.

**View:**  
The Razor Views display the claims and provide a form where a new claim can be entered.

**Controller:**  
The controllers handle the requests from the user, add claims to the list and display the correct pages. There is also an API controller for returning the claims as JSON.

## ASP.NET Core Features

Two features used in this project are:

- **Razor Tag Helpers** – used for the form fields and validation messages.
- **API Controllers** – used to create the `/api/claims` GET endpoint.

## API

The API can be tested using:

```text
GET /api/claims

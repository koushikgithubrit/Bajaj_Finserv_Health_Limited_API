# Bajaj_Finserv_Health_Limited_API


This project implements a REST API for the Chitkara Full Stack Question Paper using Node.js and Express.

## Features
- POST /bfhl endpoint that processes an array and returns:
  - Status
  - User ID
  - Email ID
  - College Roll Number
  - Array for even numbers
  - Array for odd numbers
  - Array for alphabets (converted to uppercase)
  - Array for special characters
  - Sum of numbers (as string)
  - Concatenation of all alphabetical characters in reverse order with alternating caps

## How to Run Locally

1. Install dependencies:
   bash
   npm install
   
2. Start the server:
   bash
   node index.js
   
3. The server will run on http://localhost:5000 by default.

## Example Request

POST /bfhl
json
{
  "data": ["a", "1", "334", "4", "R", "$"]
}


## Example Response
json
{
  "is_success": true,
  "user_id": "john_doe_17091999",
  "email": "john@xyz.com",
  "roll_number": "ABCD123",
  "odd_numbers": ["1"],
  "even_numbers": ["334", "4"],
  "alphabets": ["A", "R"],
  "special_characters": ["$"],
  "sum": "339",
  "concat_string": "Ra"
}


## Deployment
I have deployed this project to onrender.
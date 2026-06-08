# URL Shortener

## Overview
This project is a URL Shortener application built using Node.js, Express.js, and MongoDB. It allows users to convert long URLs into short and easy-to-share links. The application also tracks the number of visits made through each shortened URL.

## Features
* Generate short URLs from long URLs
* Redirect users to the original URL
* Store URL data in MongoDB
* Track visit history and click counts
* REST API support for URL creation and retrieval

## Tech Stack
* Node.js
* Express.js
* MongoDB
* Mongoose
* ShortID

## How It Works
1. User submits a long URL.
2. The server generates a unique short ID.
3. The original URL and short ID are stored in MongoDB.
4. When the short URL is accessed, the user is redirected to the original URL.
5. The visit is recorded in the database for analytics.

## API Endpoints
### Create Short URL
POST /url
Request:
{
"url": "https://example.com"
}

### Redirect to Original URL
GET /:shortId

## Author
Arushi Sharma

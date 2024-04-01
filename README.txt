URL Shortener Project

Introduction
This URL Shortener project is a Node.js-based application designed to shorten long URLs to more manageable versions. It features JWT authentication to ensure that each user can only access analytics for URLs they've submitted.


Features
URL Shortening: Users can submit a long URL and receive a shortened version for easier sharing.
User Authentication: Secure access using JWT (JSON Web Tokens) to ensure users can only access their own URLs and analytics.
Analytics Tracking: Tracks the number of visits for each shortened URL, accessible only by the user who created the URL.


How It Works
User Authentication: Users must authenticate to access the service. Upon authentication, they receive a JWT, granting them access to their URLs and analytics.

Shortening a URL: Authenticated users can create a short version of a long URL through a POST request. The service generates a unique identifier for each URL, associates it with the user, and returns the shortened version.

Redirecting: Accessing a shortened URL via a GET request redirects the user to the original URL and increments a visit counter.

User-Specific Analytics: Authenticated users can view the total number of visits for their shortened URLs through a GET request, ensuring privacy and security of data.


http://localhost:8001/signup
http://localhost:8001/login
http://localhost:8001/url
http://localhost:8001/
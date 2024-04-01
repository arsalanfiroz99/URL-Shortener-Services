# URL Shortener Service

## Introduction

The URL Shortener Service is a Node.js application designed to simplify long URLs into shortened links, with added features like JWT-based user authentication for secure access to personalized analytics of each shortened URL.

## Key Features

- **URL Shortening**: Easily convert long URLs to shortened links for ease of sharing.
- **Secure User Authentication**: Utilize JWT authentication to ensure secure access to the application.
- **Personalized Analytics**: Access detailed analytics for your shortened URLs, tracking the total number of visits.

## Technologies Used

- Node.js
- Express
- MongoDB
- JWT for Authentication

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Node.js
- npm (Node Package Manager)
- MongoDB

### Installation

1. **Clone the repository**
   
   Use the following command to clone the project repository to your local machine:

   ```
   git clone https://github.com/<your-username>/URL_Shortener.git
   ```

   Replace `<your-username>` with your GitHub username or the organization/user under which the repository is hosted.

2. **Navigate to the project directory**

   ```
   cd URL_Shortener
   ```

3. **Install dependencies**

   Run the following command to install the necessary Node.js packages for the project:

   ```
   npm install
   ```

### Running the Application

1. **Start the server**

   ```
   node index.js
   ```

   This command will start the Node.js server, and the application will begin listening for incoming requests.

2. **Accessing the application**

   With the server running, you can access the URL Shortener Service through your web browser or API client at the designated port (default is usually 3000).

## Usage

- **Shortening a URL**: Send a `POST` request to `/URL` with the original URL to receive a shortened link.
- **Accessing a Shortened URL**: Use a `GET` request with the short link to be redirected to the original URL.
- **Viewing Analytics**: Authenticated users can send a `GET` request to `/URL/analytics/:id` to view the click count for their shortened URLs.

## Contributing

Contributions to the URL Shortener Service are welcome! Please feel free to fork the repository, make improvements, and submit pull requests.

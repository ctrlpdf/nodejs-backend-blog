# nodejs-backend-blog

This project is a backend service for a blog, built with Node.js.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for testing purposes.

### Prerequisites

The following items need to be installed for this software:

- Docker
- Node.js
- npm or yarn

### Installing

Follow these steps to set up a development environment:

1. Clone the repo: `git clone <repo_url>`
2. Start docker
3. Execute docker-compose: `docker-compose up -d`
4. Install dependencies: `npm install` or `yarn install`
5. Start the server: `npm start` or `yarn start`

## Built With

- [Docker](https://www.docker.com/) - A platform to develop, ship, and run applications
- [Node.js](https://nodejs.org/) - JavaScript runtime environment
- [Express.js](https://expressjs.com/) - Minimalist web application framework
- [MongoDB](https://www.mongodb.com/) - Database

## Authentication

This project uses [JWT (JSON Web Tokens)](https://jwt.io/) for authentication. JWT is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

To implement JWT authentication:

1. When the user logs in, the server generates a JWT token for the user.
2. The server sends this token to the client.
3. The client stores this token and includes it in the header with every request.
4. The server verifies this token and if it's valid, allows access to the requested resources.

This method ensures secure transmission of information and prevents unauthorized access.

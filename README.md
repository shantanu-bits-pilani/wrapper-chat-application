# AS3 Chat Application

## Overview
The AS3 Chat Application is a microservices-based chat application. It consists of multiple services including authentication, user management, chat messaging, and an API gateway.

## Services
- **Auth Service**: Handles user authentication and authorization.
- **User Service**: Manages user profiles and friend requests.
- **Chat Service**: Manages messaging between users.
- **Gateway Service**: Acts as an API gateway, forwarding requests to the appropriate microservices.
- **Frontend**: A React-based user interface for the chat application.

## Directory Structure
```
AS3-Chat-Application/ 
├── auth-service/ 
│ ├── src/
│ │ └── app.py
│ └── README.md 
├── chat-service/
│ ├── src/
│ │ └── app.py 
│ └── README.md 
├── user-service/
│ ├── src/
│ │ └── app.py 
│ └── README.md 
├── gateway-service/
│ ├── src/
│ │ └── app.py 
│ └── README.md 
├── frontend/ 
│ ├── public/
│ │ └── index.html
│ ├── src/
│ │ └── App.js
│ │ ├── Components/
│ │ │ ├── ChatWindow/
│ │ │ │ └──ChatWindow.js
│ │ │ ├── FriendsList/
│ │ │ │ └──FriendsList.js
│ │ │ ├── HomePage/
│ │ │ │ └──HomePage.js
│ │ │ ├── Login/
│ │ │ │ └──Login.js
│ │ │ ├── Signup/
│ │ │ │ └──Signup.js
│ │ │ └── UserList/
│ │ └── └──UserList.js
│ ├── package.json
│ ├── Dockerfile
│ └── README.md 
├── docker-compose.yml 
└── README.md
```

## Cloning the Repository
To clone the repository, use the following command:
```bash
git clone https://gitlab.com/your-username/AS3-Chat-Application.git
cd AS3-Chat-Application
```

### Adding GitLab Submodules
If your project uses GitLab submodules, add them using the following commands:
```bash
git submodule add https://gitlab.com/your-username/auth-service.git auth-service
git submodule add https://gitlab.com/your-username/chat-service.git chat-service
git submodule add https://gitlab.com/your-username/user-service.git user-service
git submodule add https://gitlab.com/your-username/gateway-service.git gateway-service
git submodule add https://gitlab.com/your-username/frontend.git frontend
git submodule update --init --recursive
```

### Working with Docker
To build and run the services using Docker, use the following commands:
Building the Docker Images

```bash
docker-compose build
```

Running the Docker Containers

```bash
docker-compose up
```

Stopping the Docker Containers

```bash
docker-compose down
```

### Starting the frontend Repository
To start the frontend repository, navigate to the `frontend` directory and run the following commands:
```bash
cd frontend
npm install
```

### Start the Development Server
```bash
npm start watch
```

## Services Details

### Auth Service

Handles user authentication and authorization. For more details, refer to the auth-service/README.md.  

### User Service
Manages user profiles and friend requests. For more details, refer to the user-service/README.md.  

### Chat Service
Manages messaging between users. For more details, refer to the chat-service/README.md.  

### Gateway Service
Acts as an API gateway, forwarding requests to the appropriate microservices. For more details, refer to the gateway-service/README.md.  

### Frontend
A React-based user interface for the chat application. For more details, refer to the frontend/README.md.  

### Dependencies

- Docker
- Docker Compose
- Node.js and npm (for the frontend)

## License
This project is licensed under the MIT License.
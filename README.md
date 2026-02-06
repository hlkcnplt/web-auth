# Web Auth

A full-stack authentication application featuring a modern React frontend and three interchangeable backend implementations. This project demonstrates how to implement the same authentication logic across different backend technologies.

## 🏗 Project Structure

The project is organized as a monorepo with the following components:

| Component            | Directory         | Stack                    | Description                                       |
| -------------------- | ----------------- | ------------------------ | ------------------------------------------------- |
| **Frontend**         | `/frontend`       | React, Vite, TailwindCSS | The user interface for the application.           |
| **Backend (Node)**   | `/backend-node`   | Node.js, Express, Prisma | Backend implementation using Node.js environment. |
| **Backend (.NET)**   | `/backend-dotnet` | .NET 9, ASP.NET Core     | Backend implementation using C# and .NET.         |
| **Backend (Spring)** | `/backend-spring` | Java, Spring Boot        | Backend implementation using Java ecosystems.     |

## 🚀 Getting Started

### Prerequisites

- Node.js (for Frontend and Node backend)
- Java JDK 17+ (for Spring backend)
- .NET SDK (for .NET backend)
- Docker (for Database)

### Database Setup

The project uses PostgreSQL for the database. A `docker-compose.yml` file is provided to spin up the database quickly.

```bash
# Start the database
docker-compose up -d
```

### Running the Application

#### 1. Frontend

```bash
cd frontend
npm install
npm run dev
```

#### 2. Backends (Choose one)

**Node.js:**

```bash
cd backend-node
npm install
npx prisma generate
npm run dev
```

**Spring Boot:**

```bash
cd backend-spring
./mvnw spring-boot:run
```

**.NET:**

```bash
cd backend-dotnet
dotnet run
```

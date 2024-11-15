# Monsters_API

Basic API using Node, SQL, and PostgreSQL.

## Description

Monsters_API is a project designed to demonstrate the creation of a basic API utilizing Node.js, SQL, and PostgreSQL. The primary goal is to provide a simple yet effective example of how to build and interact with an API using these technologies.

## Repository Structure

The repository is primarily composed of JavaScript (93.5%) and Shell scripts (6.5%). Here is an overview of the main files and directories:

- **src/**: Contains the source code for the API.
- **tests/**: Includes test cases for the API endpoints.
- **scripts/**: Shell scripts used for various setup and maintenance tasks.

## Getting Started

### Prerequisites

- Node.js
- PostgreSQL

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/GantalaAvinash/Monsters_API.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Monsters_API
   ```
3. Install dependencies:
   ```sh
   npm install
   ```

### Setup

1. Configure the PostgreSQL database by setting up the necessary tables and seeding initial data.
2. Update the database configuration in the `config` directory.

### Running the API

Start the server:
```sh
npm start
```

The API will be available at `http://localhost:3000`.

## Usage

### Endpoints

- `GET /monsters`: Retrieve a list of monsters.
- `POST /monsters`: Add a new monster.
- `PUT /monsters/:id`: Update a monster's details.
- `DELETE /monsters/:id`: Delete a monster.

### Examples

Retrieve a list of monsters:
```sh
curl -X GET http://localhost:3000/monsters
```

Add a new monster:
```sh
curl -X POST http://localhost:3000/monsters -d '{"name": "Dragon", "type": "Fire"}' -H "Content-Type: application/json"
```

## License

This project is licensed under the MIT License.

---
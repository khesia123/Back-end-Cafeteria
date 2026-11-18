# Bookstore Category API — Academic Project

An academic Node.js backend developed for the Web Programming 3 (PW3) course. The current source code exposes CRUD operations for book categories using Express, Sequelize, and MySQL.

## Technology stack

- Node.js
- Express
- Sequelize ORM
- MySQL / mysql2
- Nodemon

## Main implementation

The API entry point is located at `Back-end Cafeteria/PW3/Cafeteria/index.js`.

### Category routes

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/listarCategoriaItens` | List categories |
| GET | `/listarCategoriaItens/:id` | Find a category by primary key |
| POST | `/inserirCategoriaItens` | Create a category |
| PUT | `/alterarCategoriaItens` | Update a category |
| DELETE | `/excluirCategoriaItens/:id` | Delete a category |

## Run locally

1. Install Node.js and MySQL.
2. Create the local database expected by the application: `cafeteria_tbl`.
3. Review the connection settings in `Back-end Cafeteria/PW3/Cafeteria/database/database.js` and adapt them to your local environment.
4. Install dependencies from the project directory containing `package.json`:

```bash
npm install
```

5. Start the API from the `Cafeteria` directory:

```bash
node index.js
```

The API listens on port `3000`.

## Notes

This repository preserves an academic exercise and is not production-ready. The database connection is configured in code for local development. A production implementation would need environment-based configuration, validation, authentication, authorization, and improved error handling.

# REST API

Build a RESTful API for a resource with full CRUD operations.

## Requirements

### Endpoints
Create a REST API for a resource (e.g., books, tasks, products):

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/items | List all items |
| GET | /api/items/:id | Get single item |
| POST | /api/items | Create new item |
| PUT | /api/items/:id | Update item |
| DELETE | /api/items/:id | Delete item |

### Technical Requirements
- Use Express.js with TypeScript
- Input validation on POST/PUT
- Proper error handling with status codes
- In-memory storage (array) is fine for this project
- Return JSON responses

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the dev server:
   ```bash
   npm run dev
   ```

## Suggested Structure

```
src/
├── routes/
│   └── items.ts
├── controllers/
│   └── itemController.ts
├── middleware/
│   ├── errorHandler.ts
│   └── validateItem.ts
├── types/
│   └── item.ts
└── index.ts
```

## Tips

- Start with GET endpoints, then add POST, PUT, DELETE
- Use Thunder Client or Postman to test your API
- Return appropriate HTTP status codes (200, 201, 400, 404, etc.)
- Add request logging middleware

## Bonus Challenges

- Add pagination to GET /items
- Implement search/filter query parameters
- Add rate limiting
- Write API documentation with Swagger

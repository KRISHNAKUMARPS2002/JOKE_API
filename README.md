# JOKE_API

## Description
JOKE_API is an Express.js application that provides endpoints to manage jokes. Users can perform CRUD operations (Create, Read, Update, Delete) on jokes through HTTP requests.

## Installation
1. Clone the repository: `git clone https://github.com/KRISHNAKUMARPS2002/JOKE_API.git`
2. Navigate to the project directory: `cd JOKE_API`
3. Install dependencies: `npm install`
4. Start the server: `npm start`

## Usage
### Endpoints
1. **GET /random**: Retrieves a random joke.
2. **GET /jokes/:id**: Retrieves a specific joke by ID.
3. **GET /filter?type=**: Filters jokes by type.
4. **POST /jokes**: Adds a new joke.
   - Request Body: `{ "text": "Your joke text", "type": "Joke type" }`
5. **PUT /jokes/:id**: Updates a joke by ID.
   - Request Body: `{ "text": "Updated joke text", "type": "Updated joke type" }`
6. **PATCH /jokes/:id**: Partially updates a joke by ID.
   - Request Body: `{ "text": "Updated joke text" }` (Optional: `"type": "Updated joke type"`)
7. **DELETE /jokes/:id**: Deletes a specific joke by ID.
8. **DELETE /all?key=**: Deletes all jokes (requires master key authorization).

### Authorization
For deleting all jokes, use the master key as a query parameter: `DELETE /all?key=your-master-key`

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a new Pull Request.



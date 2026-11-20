# Project 2 — Student Portal with Login and Protected Routes

## Folder structure

```text
Project_2_Student_Portal_Login_API/
├── file/
│   ├── A2.js
│   ├── package.json
│   ├── .env.example
│   └── .gitignore
├── outputs/
└── README.md
```

## Setup

1. Install Node.js and make sure MongoDB is running, or create a MongoDB Atlas database.
2. Open a terminal inside the `file` folder.
3. Run `npm install`.
4. Copy `.env.example` to `.env` and set your own MongoDB connection string.
5. For Project 2, also set a long private `JWT_SECRET`.
6. Start the API with `npm start` (or `node A2.js`).

The server uses port 3000 by default.

## API endpoints

- `POST /register — register a student or admin`
- `POST /login — login and receive a JWT`
- `GET /profile — view logged-in user's profile`
- `GET /students — admin-only list of students`

## Sample request body

Use this JSON with the relevant POST endpoint:

```json
{
  "name": "Demo Student",
  "email": "student@example.com",
  "password": "student123",
  "role": "student"
}
```

## Testing

Use Postman or Thunder Client. Save your real request/response screenshots in `outputs/`.
For database evidence, open MongoDB Compass and capture the relevant collection after inserting data.

Do not upload your `.env` file or fabricated screenshots.

## GitHub submission

Create a separate **Public** GitHub repository for this project. Upload the contents of this folder, including the `file`, `outputs`, and `README.md` items. Add your screenshots before final submission.

# 📚 FastAPI CRUD Evolution

This project demonstrates a step-by-step evolution of a CRUD API built using **FastAPI**, starting with an in-memory Python list and later transitioning to database-backed operations.

The API manages a collection of books and supports basic CRUD operations.

---

## 🚀 Features

- Built using **FastAPI**
- Modular project structure
- Clean separation of concerns with routes, schemas, and mock data
- Implements the following CRUD endpoints:

| Method | Endpoint          | Description                   |
| ------ | ----------------- | ----------------------------- |
| GET    | `/books`          | Retrieve all books            |
| POST   | `/books`          | Create a new book             |
| GET    | `/book/{book_id}` | Retrieve a book by ID         |
| PATCH  | `/book/{book_id}` | Update an existing book by ID |
| DELETE | `/book/{book_id}` | Delete a book by ID           |

---

## 📁 Folder Structure

```
fastapi-crud-evolution/
├── env/ # Optional virtual environment directory (excluded from Git)
├── main.py # Entry point to run the FastAPI app
├── requirements.txt # Dependencies
└── src/
└── init.py
└── books/
├── init.py
├── routes.py # All book-related route definitions
├── schemas.py # Pydantic models for request/response validation
└── book_data.py # In-memory list of book records
```

---

## 🛠️ Installation & Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/fastapi-crud-evolution.git
   cd fastapi-crud-evolution
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate # On Windows: env\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the application:
   ```bash
   uvicorn main:app --reload
   ```
5. Visit the interactive API docs at:

   - Swagger UI: http://localhost:8000/docs

   - ReDoc: http://localhost:8000/redoc

---

🔄 Evolution Roadmap

✅ Stage 1: CRUD using in-memory Python list

⏳ Stage 2: Integrate SQLite or PostgreSQL via SQLAlchemy

🔐 Stage 3: Add authentication & authorization

📦 Stage 4: Add dependency injection & testing

---

📝 License

This project is open-source and available under the MIT License.

---

🙌 Contributing

Feel free to fork the repo and open PRs to enhance or refactor the project!

---

Would you like me to also provide a `requirements.txt` file and sample `main.py` content for this stage?

# 🚀 Snap Feed — Full-Stack Media \& Social Feed Application

**Snap Feed** is a full-stack media-sharing and social feed web application built with an asynchronous **FastAPI** backend and an interactive **Streamlit** frontend. Users can securely register, log in, upload images and videos to the cloud via **ImageKit**, and browse or manage posts in real time.

\---

## ✨ Features

* **User Authentication \& Security:** Full registration, login, and JWT (JSON Web Token) authentication powered by `fastapi-users`.
* **Protected Endpoints:** Ownership-based route protection ensuring only authenticated users can upload media and delete their own posts.
* **Cloud Media Uploads:** Seamless image and video uploads, optimization, and CDN delivery via **ImageKit** (`imagekitio`).
* **Asynchronous REST API:** High-performance `GET`, `POST`, and `DELETE` endpoints with Pydantic schema validation and custom HTTP exception handling.
* **Async Database Layer:** Non-blocking database operations using **SQLAlchemy (Async)** with SQLite (`test.db`).
* **Interactive Frontend:** Clean, dark-themed user interface built with **Streamlit** (`frontend.py`).
* **Modern Python Tooling:** Fast dependency resolution and virtual environment management using **uv**.

\---

## 🛠️ Tech Stack

|Layer|Technology|
|-|-|
|**Backend Framework**|FastAPI, Uvicorn|
|**Frontend UI**|Streamlit|
|**Authentication**|`fastapi-users`, JWT Bearer Tokens|
|**Database \& ORM**|SQLite, SQLAlchemy (Async)|
|**Media Storage**|ImageKit SDK (`imagekitio`)|
|**Validation**|Pydantic|
|**Package Manager**|`uv`|

\---

## 📂 Project Structure

```text
Fast-API project/
├── app/
│   ├── app.py          # FastAPI routes, CRUD endpoints, and middleware
│   ├── db.py           # Async database engine, session, and ORM models
│   ├── frontend.py     # Streamlit UI application
│   ├── image.py        # ImageKit SDK configuration and upload helpers
│   ├── schema.py       # Pydantic request/response schemas
│   └── users.py        # User authentication, JWT strategy, and fastapi-users setup
├── .env                # Environment variables (API keys, secrets)
├── .gitignore
├── .python-version
├── main.py             # Application entry point
├── pyproject.toml      # Project dependencies and metadata
├── uv.lock             # Locked dependency tree
└── README.md
```


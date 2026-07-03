# meenylink 🔗 https://meenylink.netlify.app/

A full-stack URL shortening service that converts long URLs into short, shareable links.

## Tech Stack
- **Backend:** FastAPI, SQLAlchemy, PostgreSQL
- **Frontend:** HTML, CSS, Vanilla JavaScript
- **Deployed on:** Render (backend), Netlify (frontend)

## Features
- Generate short URLs with random slugs
- Custom slug support
- Collision detection for duplicate slugs
- Persistent storage via PostgreSQL
- Instant redirect to original URL on short link visit

## Running Locally

**Backend:**
```bash
git clone https://github.com/heyimmitt/url_shortener
cd url_shortener/backend
python3 -m venv myvenv
source myvenv/bin/activate
pip install -r requirements.txt
```

Create a `.env` file in `backend/`:
```
DATABASE_URL=postgresql://youruser:yourpassword@localhost/urlshortener
```

```bash
uvicorn main:app --reload
```

**Frontend:**

Open `frontend/index.html` with Live Server or any static file server.

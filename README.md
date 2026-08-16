# 🌐 Chauka — Public Marketing Site

The marketing site for Chauka (Real-Time Restaurant Engine): landing page, demo/signup lead capture, terms & privacy. This is a standalone project, separate from the license-gated restaurant system (`restaurant-os`).

## Run

```bash
npm install
npm start        # http://localhost:8080
```

| Endpoint | Purpose |
|----------|---------|
| `GET /` | Landing page |
| `POST /api/demo` | Book a demo (name, email, restaurant, date, phone?, message?) |
| `POST /api/signup` | Start a free trial (name, email, restaurant, phone?, teamSize?) |

Leads are stored in `data/leads.json` (committed).

## Deploy

Point a Render web service (or any Node host) at this repo:

- Build: `npm install`
- Start: `node server.js`
- Health check: `/health`

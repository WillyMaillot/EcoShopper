# EcoShopper

EcoShopper is an early stage project focused on providing environmentally friendly shopping recommendations. This repository currently acts as a placeholder for future development.

## Free vs. Premium Features

The initial release of EcoShopper will provide a free tier that allows users to search for and bookmark sustainable products. A premium subscription is planned that will unlock additional capabilities such as personalized analytics, priority support, and an ad‑free experience.

### Ad Integration Plans

The service is exploring the possibility of displaying advertisements from sustainable brands in the free tier. Any ads will be non‑intrusive and clearly labeled to maintain transparency with our users.

## Deploying the Backend

For development, the backend can be launched with a command such as:

```bash
uvicorn app:app --reload
```

A production deployment might use `gunicorn` with `uvicorn` workers:

```bash
gunicorn app:app -k uvicorn.workers.UvicornWorker
```

These commands assume an ASGI application named `app` is available.

## Serving the Frontend

When a frontend is ready, build the static files and serve them using a simple HTTP server. For example:

```bash
npm install
npm run build
npx serve -s build
```

This will host the compiled frontend on the default port.

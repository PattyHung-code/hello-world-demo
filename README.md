# hello-world-demo

A minimal FastAPI web server that serves a single `Hello World` page.

## Run locally

```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

Then open <http://127.0.0.1:8000/>.

## Run on GitHub Actions for review

This repo includes a workflow at `.github/workflows/webserver-review.yml` that starts the FastAPI server and captures the rendered homepage.

1. Push your branch to GitHub.
2. Open the **Actions** tab and run **Webserver Review** (or let it run on push/PR).
3. Download the `webserver-output` artifact to review:
   - `response.html` (captured homepage)
   - `server.log` (Uvicorn logs)


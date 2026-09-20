# Jetstream2 Intro — standalone Read the Docs project

A standalone five-minute talk introducing Jetstream2 to interactive-dashboard
builders (Plotly Dash), prepared for TACCSTER. Each page is one slide with
suggested speaker notes. No dependency on — or changes to — the main
training documentation.

## Build locally

```bash
python -m venv venv
venv/bin/pip install -r requirements.txt
venv/bin/python -m sphinx -b dirhtml . _build
# open _build/index.html in a browser
```

## Publish to Read the Docs

1. Push this folder to a GitHub or GitLab repo — the repo name becomes your
   subdomain (e.g. repo `jetstream2-dash-intro` →
   `https://jetstream2-dash-intro.readthedocs.io/`).
2. Log in at https://readthedocs.org → **Add project** → select the repo.
3. That's it — `.readthedocs.yaml` configures the build automatically.

# Development installation

Quick notes to myself how to install the project and run it locally.

## How to install

```bash
poetry install
cp env.example .env
```

## How to run tests

You can run tests offline or online. Offline tests fail when you try to download a new translation that is not in the cache. Set the configuration option in the `.env` file.

```python
PYTEST_OFFLINE=true
```

The run the tests

```bash
poetry run pytest
```

## How to run the API server

```bash
poetry run uvicorn linguee_api.api:app
```

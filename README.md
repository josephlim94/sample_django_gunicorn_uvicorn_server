# sample_django_gunicorn_uvicorn_server
Sample project

# How to run
1. Install poetry.
2. Enter repo, do `poetry install`
3. Start local server by doing `gunicorn sample_django_gunicorn_uvicorn_server.asgi:application --worker-class=uvicorn.workers.UvicornWorker --bind=localhost:8000`

# Sample curl command that would cause it to crash
`curl http://localhost:8000/static/uvicorn_bug/orderan_masuk_bc_313.mp3 -i -H "Range: bytes=0-50" -o test2.mp3`

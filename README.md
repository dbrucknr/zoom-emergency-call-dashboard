# To start application (Non-Docker):

1. `source env/bin/activate`
2. `pip install -r requirements.txt`
3. From the server directory: `uvicorn src.main:app`
- If you want to enable auto-reload, type: `uvicorn src.main:app --reload`

## To see application routes:

- http://localhost:8000/docs

# To start application (Docker):

1. Verify Docker is installed:
- `docker -v`
- `docker-compose -v`

[Install Docker](install) if you need it.

2. Build the image: `docker-compose build`
3. Run in [detached mode](https://docs.docker.com/engine/reference/run/#detached--d): `docker-compose up -d`
4. Check project: `http://localhost:8004/ping`

To tear down project: `docker-compose down`


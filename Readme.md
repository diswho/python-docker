# Initial

`python -m venv venv`

`python -m pip install --upgrade pip`

`pip install pipreqs`

`pipreqs . --force`

`pip install "uvicorn[standard]"`

`pip freeze > requirements.txt`

`pip install -r requirements.txt`

# Run

`uvicorn app.main:app --reload`

`uvicorn sql_app.main:app --reload`

## Handle JWT tokens

`openssl rand -hex 32`

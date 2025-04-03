# DF Wallet User Service

Developers Foundry Wallet User Service

&nbsp;
[![Version: v1.0.0](https://img.shields.io/badge/api-v1.0.0-blue?style=flat&logo=money)](CHANGELOG.md)
[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

---

## OpenAPI/Swagger Documentation

The Swagger documentation for the application is hosted on [Render](https://df-user-service.onrender.com/api/docs) along with the application server.

## Setup

- Clone the repository

  ```bash
  git clone https://github.com/Developer-s-Foundry/user-service.git user-service
  cd user-service
  ```

- Setup UV. \
  [Click to Install UV](https://docs.astral.sh/uv/getting-started/installation/)

- Synchronize the package requirements

  ```bash
  uv sync
  ```

- Setup environment variables \
  You can use .env file in the root directory to configure the variables \
  _See the example in [ENV Example](.env.example)_

- Run migrations

  ```bash
  uv run manage.py migrate --database pg
  ```

- Run the server locally on port 8000

  ```bash
  uv run manage.py runserver 8000
  ```

.PHONY: install dev lint test migrate

install:
	uv sync

dev:
	uv run uvicorn app.main:app --reload --port 8000

lint:
	uv run ruff check .
	uv run ruff format .

test:
	uv run pytest

migrate:
	uv run alembic upgrade head

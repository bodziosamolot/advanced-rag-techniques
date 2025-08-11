# If there is requirements.txt but no pyproject.toml

- pyproject.toml is the native uv dependencies file
- it is incompatible with requirements.txt which is just a flat dependencies file
- to create a pyproject.toml based on requirements.txt:

```
uv init
uv add $(cat requirements.txt)
```
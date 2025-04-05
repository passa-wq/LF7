# Python REST example

Der Beispielcode [rest.py](https://github.com/johannesloetzsch/LF7/blob/main/src/examples/rest/python/rest.py) nutzt die Bibliothek [FastAPI](https://fastapi.tiangolo.com/) um eine REST-API mit Swagger UI bereitzustellen.

## Usage

```
git clone https://github.com/johannesloetzsch/LF7.git
cd src/examples/rest/python
```

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

python rest.py
```

[http://localhost:8000/index.html](http://localhost:8000/index.html)

## Development

To run a devserver with automatic reloading when code changed, use:
```
uvicorn rest:app --reload
```

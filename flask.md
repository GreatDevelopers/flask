#### On MS Windows:

```bash
mkdir myproject
cd myproject
python -m venv env
env\Scripts\activate
pip install Flask
type nul > hello.py
(env) C:\Users\GNE3\myproject>set FLASK_ENV=development
(env) C:\Users\GNE3\myproject>set FLASK_APP=hello.py
(env) C:\Users\GNE3\myproject>flask run
```

#### Contdnt of hello.py

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"
```

Open in brower http://127.0.0.1:5000

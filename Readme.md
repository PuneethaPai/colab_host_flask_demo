## [Colab Host](https://github.com/PuneethaPai/colab_host) Demo: Flask App with Gunicorn

## Install Colab Host:

```bash
$ pip install colab_host
```

## Use Colab Host to run your Flask App:

```python
from colab_host import FlaskApp

FlaskApp(
    port=3000,
    app="main:app",
    git_url="https://github.com/PuneethaPai/colab_host_flask_demo",
    requirements_file="requirements.txt"
)
```

## Testing Flask App:

```bash
$ pip install -r requirements.txt
$ gunicorn --bind 0.0.0.0:1000 main:app
```

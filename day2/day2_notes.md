# Day 2 - Docker: Dockerfile + Building Custom Images

## Theory
- A Dockerfile is a set of instructions to build your own Docker image
- You define exactly what goes into your container — OS, dependencies, code
- Build once, run anywhere

## Dockerfile Instructions

| Command | What it does |
|---------|-------------|
| `FROM ubuntu:22.04` | Base image to start from (always first line) |
| `RUN apt update` | Execute command during build |
| `COPY src dest` | Copy files from your machine INTO image |
| `ADD src dest` | Like COPY but also handles URLs and tar files |
| `WORKDIR /app` | Set working directory for following commands |
| `ENV KEY=value` | Set environment variable |
| `EXPOSE 8080` | Document which port the container uses |
| `CMD ["python3","app.py"]` | Default command when container starts (can override) |
| `ENTRYPOINT ["python3"]` | Fixed command (cannot override, args appended) |
| `USER appuser` | Switch to non-root user (security best practice) |

## Files Created Today

### `day2/app.py`
```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return 'Hello from Docker! DevOps is awesome.'

@app.route('/health')
def health():
    return {'status': 'healthy', 'app': 'my-flask-app'}

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
```

### `day2/requirements.txt`

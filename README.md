# Hello World API

Microserviço simples em FastAPI que expõe um endpoint `/hello-world`.

## Executando localmente com Docker

### Build da imagem

```bash
docker build -t hello-world .
```

### Executar o container

```bash
docker run -p 8000:8000 hello-world
```

### Testar o endpoint

```bash
curl http://localhost:8000/hello-world
```

Resposta esperada:

```json
{"message": "hello world"}
```

## Executando sem Docker

```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

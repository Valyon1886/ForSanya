FROM python:3.8-slim

ENV  \
    #python
    PYTHONFAULTHANDLER=1 \
    PYTHONUNBUFFERED=1 \
    PYTHONHASHSEED=random \
    PYTHONDONTWRITEBYTECODE=1

RUN apt-get update \
    && pip install requests

WORKDIR /pr9
COPY . .

CMD ["python", "client.py"]

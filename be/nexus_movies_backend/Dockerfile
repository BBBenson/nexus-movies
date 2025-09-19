FROM python:3.11-slim

WORKDIR /usr/src/nexus_movies_backend

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# RUN apt-get update && apt-get install -y \
#     build-essential \
#     libpq-dev \
#     curl \
#     && rm -rf /var/lib/apt/lists/*  
# RUN curl -sSL https://install.python-poetry.org | python3 -
# ENV PATH="/root/.local/bin:$PATH"

RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install -r requirements.txt

COPY . .

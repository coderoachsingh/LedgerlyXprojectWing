

<img src="https://github.com/user-attachments/assets/1f7fa88b-1991-4129-a5f2-d93b26f9c341" width="1000" />



<h1 align="center">Ledgerly</h1>
<br>

An open source, self hostable expense tracking platform built with NextJS, Python
<br>
and AWS for the Lambda functions and S3 object storage.
<br>
Manage and gain insights from your expenses.
<br>
# PROJECT ARCHITECTURE (CLOUD)

<img src="https://github.com/user-attachments/assets/373d6857-c452-44d3-90f6-090236fa53bf" width="600" />
<br>

## Project Structure

```
.
├── README.md
├── assets
│   ├── arch.png
│   ├── banner.png
│   ├── er.png
│   ├── goaccess.png
│   ├── grafana.png
│   ├── inboundrules.png
│   └── lambda-uri.png
├── docker-compose.yml
├── monitoring
│   ├── grafana
│   │   └── datasources.yml
│   └── prometheus
│       └── prometheus.yaml
└── services
    ├── backend
    │   ├── Dockerfile
    │   ├── app
    │   │   ├── __init__.py
    │   │   ├── app.py
    │   │   ├── core
    │   │   │   ├── __init__.py
    │   │   │   ├── config.py
    │   │   │   ├── db.py
    │   │   │   └── utils.py
    │   │   ├── db
    │   │   │   ├── __init__.py
    │   │   │   └── models.py
    │   │   ├── main.py
    │   │   └── routers
    │   │       ├── __init__.py
    │   │       ├── auth.py
    │   │       ├── deps.py
    │   │       └── receipts.py
    │   ├── pyproject.toml
    │   └── uv.lock
    ├── ledgerly.sql
    └── receipt-ocr
        ├── Dockerfile
        └── app.py

```
<br>

### Tech Stack
![NextJs](https://img.shields.io/badge/Nextjs-black?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-blue?style=for-the-badge&logo=python&logoColor=white)
![Uvicorn](https://img.shields.io/badge/uvicorn-E6526F.svg?style=for-the-badge&logo=gunicorn&logoColor=white)
![EC2](https://img.shields.io/badge/ec2-orange?style=for-the-badge&logo=amazon-ec2&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![ECR](https://img.shields.io/badge/ecr-f06611.svg?style=for-the-badge&logo=square&logoColor=white)
![S3](https://img.shields.io/badge/S3-darkgreen?style=for-the-badge&logo=amazon-s3&logoColor=white)
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=for-the-badge&logo=aws-lambda&logoColor=white)
![Gemini](https://img.shields.io/badge/gemini-8E75B2?style=for-the-badge&logo=google%20gemini&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)

## Working
-A picture of the bill is uploded to the S3 bucket. 
<br>
-lambda function is triggered and it scan and get the total amount from the bill.
<br>
-The expense data is stored in PostgreSQL database.



 





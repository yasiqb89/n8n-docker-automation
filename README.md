# 🧠 n8n Docker Automation Setup

This project contains a complete, ready-to-use setup for running [n8n](https://n8n.io/) in Docker using Docker Compose with PostgreSQL and custom environment variables.

## 📦 Features

- ✅ Easy setup via `docker-compose`
- 🔐 Secure with basic auth and encryption key
- 🗃️ PostgreSQL for persistent database storage
- 📁 Volume for saving workflows and credentials
- 🌍 Customizable via `.env` file

## 🚀 Getting Started

### 1. Clone this repository

```bash
git clone https://github.com/yasiqb89/n8n-docker-automation.git
cd n8n-docker-automation
```

### 2. Set environment variables

Create your `.env` file:

```bash
cp .env.example .env
```

Then update the `.env` file with your custom values (e.g., password, encryption key, timezone, etc.).

### 3. Start n8n

```bash
docker compose up -d
```

n8n will be available at:  
📍 `http://localhost:5678`

Login using the credentials you defined in `.env`.

### 4. Stop the setup

```bash
docker compose down
```

## 📂 Project Structure

```
n8n-docker-automation/
├── .env.example           # Template for environment variables
├── .gitignore
├── docker-compose.yml     # Docker Compose config
└── README.md              # Project documentation
```

## 🛡️ Security Tips

- Use a **strong `N8N_ENCRYPTION_KEY`**
- Set a **secure admin password**
- Avoid exposing ports directly in production

## 📌 License

This project is licensed under the MIT License.

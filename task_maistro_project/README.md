# Task Maistro Project

This sub-project is an isolated copy of the module 6 deployment example. It contains the necessary scripts and configuration files to run the `task_maistro` graph locally or to package it for deployment.

## Contents
- `task_maistro.py` – main LangGraph script defining the task management assistant.
- `configuration.py` – dataclass for configuring user ID and other settings via environment variables or the LangGraph SDK.
- `langgraph.json` – configuration file allowing LangGraph Studio to load the graph.
- `requirements.txt` – Python dependencies specific to this project.
- `docker-compose-example.yml` – example stack for running the service with Redis and Postgres.

## Quick Start

1. **Install dependencies**
   ```bash
   python3 -m venv env
   source env/bin/activate
   pip install -r requirements.txt
   ```

2. **Run the graph in LangGraph Studio**
   ```bash
   langgraph dev
   ```
   Studio will print a local URL where you can interact with the `task_maistro` graph.

3. **Deploy with Docker (optional)**
   Use `docker-compose-example.yml` as a starting point for running the service with Redis and Postgres.


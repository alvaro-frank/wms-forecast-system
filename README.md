# 📈 AI-Powered WMS Forecasting System

An end-to-end ecosystem designed to optimize warehouse operations through advanced demand and metric forecasting. This system trains predictive Machine Learning models and serves them via a robust API for seamless integration into existing Warehouse Management Systems (WMS).

---

## 🛰️ System Architecture

This project is organized into specialized repositories, linked here as **Git Submodules** to maintain a clean separation of concerns between data science and software engineering:

| Component | Description | Tech Stack | Repository |
|-----------|-------------|------------|------------|
| **AI Training** | Data processing, feature engineering, and training of forecasting models. | Python, Pandas, Scikit-Learn | [Explore](https://github.com/alvaro-frank/wms-forecast) |
| **Backend API** | High-performance inference service exposing models for consumption. | Python, FastAPI, Docker | [Explore](https://github.com/alvaro-frank/wms-forecast-backend) |
| **Frontend UI** | *[Planned]* Interactive dashboard for forecast visualization and metrics. | React / Next.js | [TBD] |

---

## 🛠️ Key Features

- **Data-Driven Insights**: Machine learning models tailored to capture seasonality, trends, and specific warehouse operations data.
- **Decoupled Architecture**: Clear separation between the experimental data science pipeline (training) and the production infrastructure (backend).
- **Scalable Inference**: Models are deployed behind a fast, RESTful API, ready to handle requests from external WMS platforms or dashboards.
- **Containerized Ecosystem**: Designed to be easily spun up using Docker, ensuring consistency across development and production environments.

---

## ⚡ Quick Start

To clone the complete ecosystem and run the backend service:

1. **Clone the Master Repository with Submodules**:
```bash
git clone --recurse-submodules [https://github.com/alvaro-frank/wms-forecast-master.git](https://github.com/alvaro-frank/wms-forecast-master.git)
cd wms-forecast-master
```

2. **Launch via Docker Compose**:
```bash
docker-compose up --build
```

3. **Access API Documentation**:

Once running, visit `http://localhost:8000/docs` to test the prediction endpoints via the Swagger UI.

Developed by Álvaro Franco - [LinkedIn](https://www.linkedin.com/in/alvaro-jose-franco/) | [GitHub](https://github.com/alvaro-frank)

# Trend Detector AI

## Overview

Trend Detector AI is a sophisticated system designed to monitor social media platforms like Twitter, Instagram, and TikTok in real-time to detect emerging trends and viral memes before they become mainstream. The system leverages advanced natural language processing, image analysis, and machine learning techniques to identify and score potential trends, providing early insights into what might go viral.

## Features

- **Real-Time Data Ingestion**: Streams data from Twitter, Instagram, and TikTok APIs
- **Distributed Processing**: Uses Apache Kafka for distributed data streaming and Apache Spark for distributed processing
- **Advanced Preprocessing**: Cleans and processes text, images, and metadata using state-of-the-art models like BERT and CLIP
- **Dynamic Clustering**: Groups posts into evolving topics using HDBSCAN and UMAP
- **Anomaly Detection**: Identifies unusual growth or engagement patterns
- **Scoring and Alerts**: Scores clusters and generates notifications for potential trends
- **Web Dashboard**: Displays detected trends in an interactive dashboard

## Architecture

The system is divided into several key components:

1. **Data Ingestion**: Handles real-time data streaming from APIs
2. **Preprocessing**: Cleans and processes text, images, and metadata
3. **Feature Engineering**: Converts raw data into embeddings and relevant features
4. **Clustering and Topic Modeling**: Groups posts into evolving topics
5. **Anomaly Detection**: Identifies unusual growth or engagement patterns
6. **Scoring and Alerts**: Scores clusters and generates notifications
7. **Web Dashboard**: Displays detected trends

## Tools and Libraries

- **Language Processing**: Transformers by Hugging Face, spaCy
- **Data Streaming**: Python SDKs for platform APIs, Apache Kafka
- **Clustering**: HDBSCAN, sklearn, UMAP
- **Anomaly Detection**: Time-series models, statistical metrics
- **Backend**: FastAPI
- **Database**: PostgreSQL
- **Dashboard**: Streamlit
- **Distributed Computing**: Docker, Kubernetes

## Installation

### Prerequisites

- Python 3.9+
- CUDA-compatible GPU (recommended for transformer models)
- Docker 24.0+ (for containerization)
- Kubernetes 1.28+ (optional, for orchestration)
- Apache Kafka 3.6+
- PostgreSQL 15+

#### Python Package Requirements
- NumPy (>=2.1.0)
- Pandas (>=2.2.0)
- scikit-learn (>=1.4.0)
- spaCy (>=3.7.2)
- Transformers (>=4.37.0)
- PyTorch (>=2.2.0)
- FastAPI (>=0.109.0)
- Streamlit (>=1.31.0)
- HDBSCAN (>=0.8.33)
- UMAP (>=0.5.5)
- Kafka-Python (>=2.0.2)

#### Hardware Requirements (Per Server)
- Minimum 64GB RAM (Recommended: 128GB+ for production)
- High-performance CPU (Minimum 16 cores, 32 threads)
- CUDA-compatible GPU with 16GB+ VRAM for transformer models
- 500GB+ SSD storage (Recommended: 1TB+ for extended data retention)
- High-bandwidth network connection (10Gbps recommended)

#### Cluster Requirements (Production)
- Minimum 3 server nodes for high availability
- Load balancer for distributed processing
- Dedicated database server with 128GB+ RAM
- Separate servers for:
  - Data ingestion and preprocessing
  - Model inference and clustering
  - Database and storage
  - Dashboard and API serving

#### Additional Requirements
- Robust internet connection with redundancy
- API keys with enterprise-level rate limits for:
  - X (Twitter) Enterprise API
  - Instagram Graph API
  - TikTok Business API
- Kafka cluster with multiple brokers
- PostgreSQL with partitioning and replication setup
- At least 16GB RAM
- 50GB+ available disk space
- API keys for X (Twitter), Instagram, and TikTok

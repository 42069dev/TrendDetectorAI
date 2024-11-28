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


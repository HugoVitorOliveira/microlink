# 🌐 Microlink Project Overview

## 🏗️ System Design

### ✅ Functional Requirements
- 🔗 Shorten long URLs into short links.  
- ↪️ Redirect short links to their original URLs.  
- 📊 Track metrics: clicks per link, by city/state/country, by hour/day/month, etc.  
- 🧑‍💼 Manage users and permissions, automatically delete links after 5 hours for anonymous users.  

### ⚙️ Non-Functional Requirements
- ⚡ High availability and performance.  
- 📈 Horizontal scalability to support many users simultaneously.  
- 🧰 Secure storage and redirection of URLs.  

### 🧱 Architecture
- **Frontend**: User interface to create and manage URLs.  
- **Backend**: API responsible for URL generation and redirection.  
- **Database**:  
  - 🗄️ Relational: **PostgreSQL** for metadata and user management.  
  - 📂 Non-relational: **MongoDB** for storing shortened links.  

### 🔄 General Flow
1. The client sends a long URL to the backend.  
2. The backend generates a unique hash (shortened SHA-256).  
3. The short URL is saved along with the original URL and metadata.  
4. Redirects are handled by the backend with caching support.  

---

## 💻 Technologies

### 🧠 Backend
- 🖥️ **Quarkus** – Lightweight and performant microservices framework.  

### 🗃️ Database
- 🛢️ **PostgreSQL**  
- 📘 **MongoDB**  

### 🧑‍🎨 Frontend
- 🅰️ **Angular** – Intuitive and responsive user interface.  

### ⚙️ DevOps
- 🐋 **Docker** – Containerization of services.  
- 📦 **Kubernetes** – Container orchestration.  
- 🔁 **GitHub Actions** – Continuous integration and delivery (CI/CD).  

### 📡 Monitoring
- 📊 **Prometheus + Grafana** – Metrics collection and visualization.  
- 🪵 **Elastic Stack (ELK)** – Log monitoring and analysis.  

## 📄 Others
- 🧾 Report generation using **Jasper Reports**.  

---

## 🧩 Methodology

### 📌 Planning
- 🎯 Define use cases and requirements.  
- 🗺️ Create flow and architecture diagrams.  

### 👨‍💻 Implementation
- 🧱 Break the system into microservices.  
- 🧼 Apply best practices like **SOLID** and **Clean Code**.  

### 🧪 Testing
- 🔍 Write unit and integration tests.  
- 🧰 Load testing with tools like **JMeter** or **Postman Collections**.  

### 🔁 Iteration
- 💡 Continuous improvement based on user feedback.  
- 🌐 Scale as traffic increases.  

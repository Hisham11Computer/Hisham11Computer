<!-- ============ HEADER ============ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=200&section=header&text=Hisham%20Emad&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=Data%20Engineer%20%7C%20Real-Time%20CDC%20%26%20Lakehouse%20Pipelines&descSize=20&descAlignY=60" alt="Hisham Emad">
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&color=2C9CDB&center=true&vCenter=true&width=700&lines=Building+real-time+CDC+pipelines;Kafka+%C2%B7+Debezium+%C2%B7+Spark+%C2%B7+Delta+Lake;Bronze+%E2%86%92+Silver+%E2%86%92+Gold+lakehouses;Fast+SQL%3A+indexing+%26+query+tuning" alt="Typing animation">
  </a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hisham-el-rifai-82ba55378/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:hishammm77717@gmail.com"><img src="https://img.shields.io/badge/Email-Contact%20Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Open%20to-Data%20Engineering%20Roles-2ea44f?style=for-the-badge" alt="Open to work">
</p>

---

## 👋 About Me

I build data pipelines and data platforms end to end: capturing changes from transactional databases, streaming them through Kafka, processing them in a Bronze / Silver / Gold lakehouse, and serving clean data for analytics. I also care a lot about database performance: reading execution plans, fixing slow queries with the right indexes, and proving the improvement with benchmarks.

## ⚡ What I Do Best

| | Skill | What I've built with it |
|---|---|---|
| 🔴 | **Real-Time CDC & Streaming** | Debezium + Kafka + Spark Structured Streaming capturing PostgreSQL changes from the WAL |
| 🏛️ | **Lakehouse Architecture** | Bronze / Silver / Gold on S3 with Delta Lake `MERGE` upserts and Apache Iceberg |
| ⚙️ | **Pipeline Orchestration** | Apache Airflow DAGs running the full pipeline end to end, containerized with Docker Compose |
| ✅ | **Data Quality & Idempotency** | Great Expectations gates between layers, LSN high-water marks for safe re-runs |
| ☁️ | **AWS Data Services** | S3, Glue Crawler, Athena (simulated locally with LocalStack, real-AWS scripts included) |
| 🚀 | **Database Performance Tuning** | `EXPLAIN` analysis, single and composite indexes, before/after benchmarks on 200K+ rows |
| 📊 | **Analytics & BI** | Advanced SQL (CTEs, window functions), Power BI dashboards with DAX |

---

## 🌟 Featured Project

<h3>🏗️ E-commerce CDC Lakehouse Platform</h3>

<p>
  <a href="https://github.com/Hisham11Computer/Ecom-Lakehouse-End-to-End-data-Pipeline"><img src="https://img.shields.io/badge/View%20on-GitHub-181717?style=for-the-badge&logo=github" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/CI-passing-2ea44f?style=for-the-badge" alt="CI passing">
</p>

A fully containerized, end-to-end data platform that streams **change data capture** from PostgreSQL into a **Bronze / Silver / Gold lakehouse** on S3 (LocalStack), with Delta Lake upserts, a Great Expectations quality gate, Apache Iceberg, and Glue / Athena simulations, all orchestrated by Airflow. Everything runs locally with one `docker compose up`.

```mermaid
flowchart LR
    A[(PostgreSQL)] -->|WAL| B[Debezium]
    B --> C{{Kafka}}
    C --> D[Spark Streaming]
    D --> E[Bronze]
    E --> F[Silver]
    F --> G[Gold]
    G --> H[Athena / DuckDB]
    I[Airflow] -.orchestrates.-> D
    J[Great Expectations] -.quality gate.-> F
```

**Skills demonstrated**

![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Debezium](https://img.shields.io/badge/Debezium-CDC-FF6B35?style=flat-square)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-00ADD4?style=flat-square)
![Iceberg](https://img.shields.io/badge/Iceberg-4A90E2?style=flat-square)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Great Expectations](https://img.shields.io/badge/Great%20Expectations-FF6310?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![AWS S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![Glue](https://img.shields.io/badge/Glue-8C4FFF?style=flat-square&logo=awsglue&logoColor=white)
![Athena](https://img.shields.io/badge/Athena-8C4FFF?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Key engineering decisions**

- **Real-time CDC instead of polling:** Debezium reads PostgreSQL WAL changes with minimal load on the source database.
- **Idempotent processing:** LSN high-water marks and Delta Lake `MERGE` handle late-arriving data, updates, and deletes safely.
- **Automated quality gates:** Great Expectations blocks corrupted records before they reach analytical tables.
- **Zero-cost cloud simulation:** S3, Glue, and Athena run locally, and real-AWS scripts are provided.

---

## 📂 More Projects

<h3>🚚 RouteMasterX: Fleet Management & Logistics Database</h3>

<p>
  <a href="https://github.com/Hisham11Computer/fleet-management-db"><img src="https://img.shields.io/badge/View%20on-GitHub-181717?style=for-the-badge&logo=github" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/CI-passing-2ea44f?style=for-the-badge" alt="CI passing">
</p>

A MySQL 8 database for a logistics company where **business rules are enforced inside the database** (constraints, triggers, transactions) and verified by an automated test suite and CI. Covers fleet, drivers, trips, GPS telemetry, speed-violation detection, shipment assignment, and geospatial analytics.

**Skills demonstrated**

![MySQL](https://img.shields.io/badge/MySQL%208-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Triggers](https://img.shields.io/badge/Triggers%20%26%20Constraints-555555?style=flat-square)
![Transactions](https://img.shields.io/badge/Transactions%20%26%20Row%20Locking-555555?style=flat-square)
![Geospatial](https://img.shields.io/badge/Geospatial%20SQL-555555?style=flat-square)
![Window Functions](https://img.shields.io/badge/Window%20Functions-555555?style=flat-square)
![Indexing](https://img.shields.io/badge/Indexing%20Benchmark-555555?style=flat-square)
![Docker](https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Highlights**

- One active trip per vehicle/driver, enforced with generated-column unique keys and `CHECK` constraints.
- Automatic speed-violation detection with per-vehicle-type limits stored as data.
- Nearest-vehicle search, geofence radius search, and speeding hotspots.
- Transactional best-fit shipment assignment with row locking and re-check.

<br>

<h3>⚡ E-Commerce Database Performance Optimization</h3>

<p>
  <a href="https://github.com/Hisham11Computer/E-Commerce-Database-Optimization"><img src="https://img.shields.io/badge/View%20on-GitHub-181717?style=for-the-badge&logo=github" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/CI-passing-2ea44f?style=for-the-badge" alt="CI passing">
</p>

An indexing study on a simulated production-style dataset of **200K+ orders and 400K+ order items** generated with Python (Faker). I found full table scans and inefficient joins in heavy reporting queries, fixed them with targeted indexes, and documented the before/after results.

**Skills demonstrated**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Python](https://img.shields.io/badge/Python%20%7C%20Faker-3776AB?style=flat-square&logo=python&logoColor=white)
![EXPLAIN](https://img.shields.io/badge/EXPLAIN%20%26%20Visual%20Explain-555555?style=flat-square)
![Composite Indexes](https://img.shields.io/badge/Single%20%26%20Composite%20Indexes-555555?style=flat-square)
![Benchmarking](https://img.shields.io/badge/Query%20Benchmarking-555555?style=flat-square)

**Highlights**

- Diagnosed bottleneck queries and cost-heavy joins using execution plans.
- Shifted queries from full table scans to index seeks/lookups (e.g. `idx_orders_status`).
- Documented execution-plan changes and benchmarks, before vs. after.

<br>

<h3>🏋️ Gym Performance Analytics</h3>

<p>
  <a href="https://github.com/Hisham11Computer/Gym-Performance-Analytics"><img src="https://img.shields.io/badge/View%20on-GitHub-181717?style=for-the-badge&logo=github" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/CI-passing-2ea44f?style=for-the-badge" alt="CI passing">
</p>

An end-to-end analytics project: a normalized SQL database of gym members, workouts, and nutrition, analysed with advanced SQL, validated with automated data-quality checks, and presented in an interactive Power BI dashboard. **Business question:** which members are actually getting stronger, and what drives it: goal, calories, or consistency? *(The dataset is simulated; findings demonstrate the method.)*

**Skills demonstrated**

![SQL](https://img.shields.io/badge/SQL%20(ANSI)-4479A1?style=flat-square)
![CTEs](https://img.shields.io/badge/CTEs%20%26%20Window%20Functions-555555?style=flat-square)
![Views](https://img.shields.io/badge/Views-555555?style=flat-square)
![Power BI](https://img.shields.io/badge/Power%20BI%20%7C%20DAX-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Data Quality](https://img.shields.io/badge/Data%20Quality%20Checks-555555?style=flat-square)

**Highlights**

- Data model with Members, Workouts, and Nutrition tables.
- Reproducible seed data generated by a script with a fixed seed.
- Interactive dashboard answering a clear business question.

---

## 🧰 Full Tech Stack

| Area | Tools |
|---|---|
| **Streaming & Ingestion** | Apache Kafka, Debezium (CDC), PySpark Structured Streaming |
| **Lakehouse & Orchestration** | Apache Spark, Delta Lake, Apache Iceberg, Apache Airflow, DuckDB, Parquet |
| **Cloud** | AWS S3, Glue, Athena (LocalStack simulation) |
| **Data Quality** | Great Expectations |
| **Databases** | PostgreSQL, MySQL, SQL Server, SQLite |
| **Analytics & BI** | Advanced SQL, Power Query, Power BI (DAX) |
| **Languages & Tools** | Python, C#, Docker, Git, GitHub, Linux, LaTeX |

---

## 🎓 Education

**B.Sc. in Software Engineering**, Faculty of Computers and Information Technology, New Mansoura University (2024 – 2028)

Coursework: Algorithms & Data Structures (C#), System Analysis & Design (Team Leader of the *Smart University System* project), Computer Architecture (8086 Assembly).

---

## 📫 Let's Connect

I'm looking for opportunities to grow as a data engineer. If you're hiring or want to talk data, reach out:

<p>
  <a href="https://www.linkedin.com/in/hisham-el-rifai-82ba55378/"><img src="https://img.shields.io/badge/LinkedIn-Hisham%20El%20Rifai-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:hishammm77717@gmail.com"><img src="https://img.shields.io/badge/Email-hishammm77717%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2C5364,100:0F2027&height=100&section=footer" alt="footer">
</p>

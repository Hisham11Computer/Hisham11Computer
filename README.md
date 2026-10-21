<h1 align="center">Hi, I'm Hisham Emad 👋</h1>

<p align="center">
  <b>Aspiring Data Engineer · Analytics Engineer</b><br>
  Software Engineering student at New Mansoura University (2024 – 2028) · Egypt 🇪🇬
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hisham-el-rifai-82ba55378/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:hishammm77717@gmail.com"><img src="https://img.shields.io/badge/Email-Contact%20Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Open%20to-Data%20Engineering%20Roles-2ea44f?style=for-the-badge" alt="Open to work">
</p>

---

## 👨‍💻 About Me

I build **data pipelines and data platforms** end to end: capturing changes from transactional databases, streaming them through Kafka, processing them in a Bronze / Silver / Gold lakehouse, and serving clean data for analytics. I also care a lot about **database performance**: reading execution plans, fixing slow queries with the right indexes, and proving the improvement with benchmarks.

- 🔭 Currently focused on: **real-time CDC, lakehouse architecture, and AWS data services** (S3, Glue, Athena, Redshift)
- 🧪 I test what I build: data-quality gates, SQL test suites, and CI pipelines in my projects
- 📫 Open to internships and junior data engineering opportunities

---

## 🛠️ Tech Stack

**Data Engineering**

![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Debezium](https://img.shields.io/badge/Debezium-CDC-FF6B35?style=flat-square)
![Apache Spark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-00ADD4?style=flat-square&logo=delta&logoColor=white)
![Apache Iceberg](https://img.shields.io/badge/Iceberg-4A90E2?style=flat-square)
![Great Expectations](https://img.shields.io/badge/Great%20Expectations-FF6310?style=flat-square)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)

**Cloud (AWS)**

![S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![Glue](https://img.shields.io/badge/Glue-8C4FFF?style=flat-square&logo=awsglue&logoColor=white)
![Athena](https://img.shields.io/badge/Athena-8C4FFF?style=flat-square)
![LocalStack](https://img.shields.io/badge/LocalStack-000000?style=flat-square)

**Databases & Performance Tuning**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

**Analytics & BI**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-F2C811?style=flat-square)
![Power Query](https://img.shields.io/badge/Power%20Query-M-F2C811?style=flat-square)

**Programming & Tools**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)

---

## 🚀 Featured Project

### 🏗️ [E-commerce CDC Lakehouse Platform](https://github.com/Hisham11Computer/Ecom-Lakehouse-End-to-End-data-Pipeline)

A fully containerized, end-to-end data platform: **change data capture** from PostgreSQL into a **Bronze / Silver / Gold lakehouse** on S3 (LocalStack), with Delta Lake upserts, a Great Expectations quality gate, Apache Iceberg, and Glue / Athena simulations, all orchestrated by Airflow. Runs locally with a single `docker compose up`.

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

**Engineering highlights**

- **Real-time CDC instead of polling:** Debezium streams PostgreSQL WAL changes with minimal load on the source database.
- **Idempotent processing:** LSN high-water marks and Delta Lake `MERGE` (upserts) safely handle late-arriving data, updates, and deletes.
- **Automated quality gates:** Great Expectations validates data between layers and blocks bad records from reaching analytics tables.
- **Zero-cost cloud simulation:** S3 (LocalStack), Glue catalog, and Athena run locally; real-AWS scripts are included.

**Stack:** `PostgreSQL` `Debezium` `Kafka` `PySpark` `Delta Lake` `Iceberg` `Airflow` `Great Expectations` `Docker` `GitHub Actions`

---

## 📂 More Projects

| Project | What it shows | Stack |
|---|---|---|
| [🚚 **RouteMasterX**: Fleet Management & Logistics DB](https://github.com/Hisham11Computer/fleet-management-db) | Business rules enforced inside the database (constraints, triggers, transactions): no double-booked vehicles, automatic speeding detection, capacity-aware shipment assignment, geospatial analytics, SQL test suite, and CI. | MySQL 8, Docker, GitHub Actions |
| [⚡ **E-Commerce Database Optimization**](https://github.com/Hisham11Computer/E-Commerce-Database-Optimization) | Indexing study on 200K+ orders and 400K+ order items (generated with Faker). Found full table scans with `EXPLAIN`, fixed them with single-column and composite indexes, and documented before/after plans and benchmarks. | MySQL, Python, Visual Explain |
| [🏋️ **Gym Performance Analytics**](https://github.com/Hisham11Computer/Gym-Performance-Analytics) | Normalized SQL database analysed with CTEs, window functions, and views, validated with data-quality checks and presented in an interactive Power BI dashboard. Business question: *which members are actually getting stronger, and why?* | SQL, Power BI, Python |

---

## 🎓 Education & Coursework

**B.Sc. in Software Engineering**: Faculty of Computers and Information Technology, New Mansoura University (2024 – 2028)

- **Algorithms & Data Structures (C#):** sorting and searching algorithms, linked-list validators, stack-based undo.
- **System Analysis & Design:** Team Leader of the *Smart University System* project (SRS, UML diagrams, project schedule).
- **Low-level architecture:** 8086 Assembly, CPU registers, and 4-bit ALU control logic.

---

## 📫 Let's Connect

I'm looking for opportunities to grow as a data engineer. If you're hiring or want to talk data, reach out:

- 💼 [LinkedIn](https://www.linkedin.com/in/hisham-el-rifai-82ba55378/)
- 📧 hishammm77717@gmail.com

<p align="center">⭐ If you like my projects, a star on the repo means a lot!</p>

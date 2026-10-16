### Hi there, I'm Hisham Emad 👋

🎓 **Undergraduate Software Engineering Student** at the Faculty of Computers and Information Technology, New Mansoura University (Student ID: 224101239).  
🚀 ** Data Engineer & Analyics Engineer** passionate about building scalable, production-grade distributed data architectures, real-time streaming systems, high-performance database optimization, and modern lakehouses.

---

### 🛠️ Core Technical Skills (Ranked by Expertise)

#### 1. Data Engineering & Big Data Systems (Primary Expertise)
- **Streaming & Ingestion:** Apache Kafka, Debezium (Change Data Capture - CDC), PySpark Structured Streaming.
- **Lakehouse & Distributed Processing:** Apache Spark, Multi-hop Lakehouse Architecture (Bronze, Silver, Gold), Delta Lake, Apache Iceberg, Apache Airflow (Workflow Orchestration).
- **Cloud & Storage Ecosystem:** AWS S3 (LocalStack simulation), AWS Glue Crawler, Amazon Athena, DuckDB, Parquet formats.
- **Data Quality & Governance:** Great Expectations (Automated Quality Gates).

#### 2. Advanced Database Architecture & Performance Tuning
- **Query Optimization & Execution Tuning:** Analyzing `EXPLAIN` execution plans, indexing strategies, and database performance tuning.
- **Relational Systems & Development:** PostgreSQL, MySQL, SQL Server, SQLite, Stored Procedures, Transaction Management, Entity-Relationship Modeling, CASCADE Operations.

#### 3. Data Analysis & Business Intelligence
- **Data Transformation & Wrangling:** Exploratory Data Analysis (EDA), advanced SQL aggregations, Power Query (M transformations).
- **Visualization & Reporting:** Power BI (DAX measures, interactive reporting controls, bookmarks, and selection panes).

#### 4. Software Engineering & Backend Core
- **Languages & Paradigms:** Python, C#, Object-Oriented Programming (OOP), Data Structures & Algorithms.
- **DevOps & Tooling:** Docker & Docker Compose, Linux Terminal, Git, GitHub, LaTeX (Overleaf).

---

### 📌 Featured Project

- **[Ecom-Lakehouse-End-to-End-data-Pipeline](https://github.com/Hisham11Computer/Ecom-Lakehouse-End-to-End-data-Pipeline):**
  - **Overview:** A fully containerized, production-grade real-time and batch e-commerce data platform. It captures transactional changes from PostgreSQL via Debezium & Kafka, processes them through a multi-hop Lakehouse (Bronze/Silver/Gold) on S3 using PySpark and Delta Lake, and orchestrates workflows with Apache Airflow.
  - **Advanced Engineering Highlights:**
    1. *Real-Time CDC over Polling:* Utilizes Debezium to stream PostgreSQL WAL logs instantly without database performance overhead.
    2. *Idempotent Processing & State Management:* Implements LSN high-water marks and Delta Lake `MERGE` (upsert) logic to safely handle late-arriving data, updates, and deletes.
    3. *Automated Data Quality Gates:* Integrated Great Expectations between layers to block corrupted records from reaching analytical tables.
    4. *Engine-Neutral Formats & Cloud Simulation:* Simulates AWS S3 (LocalStack), Glue metadata catalogs, and Athena SQL analytics locally with zero cloud cost.

---

### 💻 Other Notable Database & Analysis Projects 

I built RouteMasterX, a MySQL database for fleet tracking and shipment logistics. The database itself enforces the business rules (no double-booked vehicles, automatic speeding detection, capacity-aware shipment assignment) and exposes geospatial analytics such as nearest-vehicle search and speeding hotspots. It ships with Docker Compose, a SQL test suite and a CI pipeline. Code and architecture write-up on GitHub: [https://github.com/Hisham11Computer/fleet-management-db]

I built an E-Commerce Database Optimization project to see how indexing changes query performance at realistic scale. I generated a 200K+ order dataset with Python (Faker), then used EXPLAIN and Visual Explain to find the queries doing full table scans and inefficient joins. I fixed them with single-column and composite indexes and documented before/after execution plans and benchmarks for each change. Code and architecture write-up on GitHub: https://github.com/Hisham11Computer/E-Commerce-Database-Optimization
--- 

### 📚 Academic & Software Engineering Coursework

- **Algorithms & Data Structures (C#):** Implemented efficient array sorting algorithms (Bubble Sort, Binary Search, Interpolation Search), linked-list prerequisite validators, and stack-based undo applications.
- **System Analysis & Design:** Served as Team Leader for a *Smart University System* project, delivering Software Requirements Specifications (SRS), UML diagrams, and project schedules.
- **Low-Level Architecture:** Studied 8086 Assembly language programming, CPU register mechanics, and 4-bit ALU logic control circuits.

---

### 📫 Connect with Me
- **LinkedIn:** [Hisham Emad El Rifai](https://www.linkedin.com/in/hisham-el-rifai-82ba55378/?isSelfProfile=true)
- **Email:** hishammm77717@gmail.com

# Hi, I'm Nicolás Guarín Gaviria

**Software & Cloud Data Engineer · DevOps & Backend** · Medellín, Colombia

I build the systems that take data from a raw source to a decision someone can act on: pipelines, APIs, ML models, and the cloud infrastructure and CI/CD that keep them running. I have 4+ years of experience in banking and energy, and I trained as a mechatronics engineer with a focus on robotics and computer vision.

**Right now:** Full-Stack Software Engineer at **Scotiabank**, contributing to the migration of Spring Boot services from on-premises to **Google Cloud**. My work there covers Microsoft Entra ID sign-in with security groups and API-to-API calls secured with scope-based signed JWTs.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nicolas-guarin-gaviria-08a4091a1)
[![Portfolio](https://img.shields.io/badge/Portfolio-222222?style=flat&logo=googlechrome&logoColor=white)](https://nicolas-guarin-gaviria-my-web-page.pages.dev/)
[![Live demo](https://img.shields.io/badge/Live_demo-Real_Estate_Analyst-FF4B4B?style=flat&logo=streamlit&logoColor=white)](https://realstateanalystcol.streamlit.app)

---

## Experience

| Company | Role | What I worked on |
|---|---|---|
| **Scotiabank** *(Apr 2025 – present)* | Full-Stack Software Engineer | On-prem → Google Cloud migration, Entra ID authentication, scope-based JWTs between Spring Boot APIs, AI-assisted dev tooling (sprint cycle from 7 to 2–4 days) |
| **ISA Interconexión Eléctrica** *(2025)* | Supply Data Analyst (contract) | Sole data engineer: Azure Databricks pipelines over 100+ sources, Azure ML models, CI/CD in Azure DevOps, RPA |
| **Bancolombia** *(2022 – 2024)* | Software Engineer & AI Support | Chatbot microservices on AWS reaching 1M+ customers/month, Azure DevOps CI/CD (deploys from 48 h to 2 h), Serenity + Playwright test automation |
| **Bancolombia** *(2021 – 2022)* | Business Analyst Intern | Impala/SAS data automation (−70% reporting errors), Power BI forecasting tool for VPs |

---

## Featured projects

### [Real Estate Analyst Colombia](https://github.com/Nggerizo97/Real_State_Analyst) · [lakehouse](https://github.com/Nggerizo97/lakehouse-repo) · [live demo](https://realstateanalystcol.streamlit.app)
An end-to-end data platform that flags Colombian properties listed below market value.
- **Ingestion:** GitHub Actions runs a matrix of Playwright scrapers on hosted and self-hosted runners. It has resumable checkpoints and failure alerts, and it triggers the Databricks ETL job automatically.
- **Lakehouse:** a PySpark medallion architecture on S3 and Databricks, with cross-portal deduplication, DIVIPOLA geographic normalization and unit-tested quality rules.
- **ML:** an XGBoost valuation model whose MAPE improved from 30% to 20.8% across 8 versions. Predictions are served through FastAPI and Streamlit.
- **Infrastructure as Code:** Terraform for an ECS Fargate deployment (ECR, autoscaling, CloudWatch, least-privilege IAM, Secrets Manager) with plan/apply pipelines. The deployment is paused to keep cost under US$1/month, and the app is currently served from Streamlit Cloud.

### [PeraBank](https://github.com/Nggerizo97/Perabank)
A credit-risk data platform built on real public data, including 2.9M LendingClub loans.
- A DuckDB medallion pipeline with schema contracts that fail the run, and quality checks at every layer.
- A 12-table snowflake model in Parquet.
- A probability-of-default model with out-of-time validation: **AUC 0.686** vs 0.675 for LendingClub's own sub-grade.
- A serverless AWS design (S3, SQS FIFO + DLQ, DynamoDB, Lambda, API Gateway), verified on a local AWS emulator with a cost model. CI runs Ruff and pytest on GitHub Actions.

### [Colombian Open-Data RAG Agent](https://github.com/Nggerizo97/challenge_epam_llm) · EPAM Challenge
A RAG agent on **AWS Bedrock** (Llama 3 70B) over 144,602 chunks in ChromaDB, ingested from Colombian open-data APIs.
- Usage quotas in DynamoDB, provisioned with Terraform, plus hard token limits.
- **87.5% faithfulness**, measured with Ragas.

### More
- [simulador_impuestos](https://github.com/Nggerizo97/simulador_impuestos): a Colombian income tax estimator built with FastAPI, React, JWT auth and Docker Compose.
- [Car_Assistant_Buyer](https://github.com/Nggerizo97/Car_Assistant_Buyer): Playwright scrapers and a Streamlit comparison app, packaged with Docker.

---

## Tech stack

**Cloud**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Microsoft Entra ID](https://img.shields.io/badge/Entra_ID-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)

**DevOps & Deployment**
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)

**Data**
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

**ML & AI**
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=for-the-badge)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![AWS Bedrock](https://img.shields.io/badge/Bedrock_RAG-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)

---

## GitHub stats

> Part of my work happens in private and company repositories, so these public numbers show only part of it.

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Nggerizo97&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true" height="165" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nggerizo97&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" height="165" alt="Top languages" />
</p>

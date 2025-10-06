# My Software Architecture, Design, and Engineering Projects

A list of projects I've worked on as an architect and software engineer.

- GitHub: byoung
- GitLab: byoung-gl
- Hugging Face: byoung-hf

TBD — expand this section and experiment with how it impacts my [(me)](https://github.com/byoung/me) agentic self [(ai-me)](https://github.com/byoung/ai-me).

## ai-me (2025)

A personal AI agent designed to emulate my communication style, knowledge, and reasoning. [ai-me](https://github.com/byoung/ai-me) leverages retrieval-augmented generation (RAG) to provide contextually relevant and accurate responses by drawing from a curated knowledge base of my writings, code, and professional experience [1](https://github.com/byoung/me) [2](https://github.com/Neosofia/corporate/tree/main/website). The project explores advanced prompt engineering, memory management, MCP tool chaining, and agentic behaviors to create a more authentic and useful digital representation of myself. Built with Python and modern LLM frameworks, ai-me serves as both a personal productivity tool and a demonstration of agentic AI design patterns.

Future versions of the project will include:
- Fine-tuned (FT) models trained on transcripts of educational videos I've watched to better reflect my knowledge
- Additional MCP tools and optimizations for the existing GitHub researcher
- Optimized RAG dataset loading and chunking
- A complete LangGraph implementation with LangSmith and LangPlatform integrations
- MoA on Groq

GitHub repo: https://github.com/byoung/ai-me

## Neosofia Corporate Website and Compliance Tools (2025)

A monorepo containing the source code and infrastructure for Neosofia's corporate website and internal tools. The repository includes:

* Static site generator for the company website and blog, built with React, Vite, Tailwind CSS, and pnpm
* Scripts for generating and managing Quality Management System (QMS) documents, leveraging LaTeX and Git for automated PDF creation, revision history, and compliance features
* Infrastructure-as-code and automation scripts for on-premises hosting, including Proxmox VM management, encrypted disk setup with LUKS, and backup/recovery using REAR
* CI/CD workflows for building, testing, and deploying the website and documentation

The repository is organized to support both public-facing content and internal operational needs, emphasizing automation, compliance, and maintainability.

GitHub Repo: https://github.com/Neosofia/corporate

## Sales Conversion Tool -- Private Neosofia Client (2025)

Architecture and design consultant for a data pipeline and ML model to predict sales conversions for a top-5 car manufacturer in Europe. Used Synapse SQL storage for staging Sales Force source data, Docker for containerization, and Microsoft Azure ML for ETL pipelines, Lead Scoring Random Forest Model management, and CI/CD.

## Vacation Recommendations -- Private Neosofia Client (2024)

Architecture and design consultant for an AI chat agent that makes travel recommendations for a top-5 travel agency in the US. Used OpenAI APIs and models on optimized prompts to provide users with easy access to quickly book recommendations on the site. Internal APIs provided the data needed to customize the agent and to prepare a link to a full itinerary that could be booked in one click.

## Clinical Trial Data Management Platform -- Private Neosofia Client (2023-2024)

Acting CTO for a CRO developing its QMS system, SOPs, and Azure data pipelines to provide services to clinical trial sponsors. Extensive use of Monday.com, GitHub, and DocuSign to establish operational workflows to handle processes relating to onboarding/offboarding, incident management, change management, asset management, employee training, BCDR, and SDLC. Policies and procedures ensured compliance with 21 CFR part 11 and ICH E6 (R2/R3).

## Clinical Trial Fraud Detection -- Medidata (2021-2023)

Architecture, design, and implementation of a machine learning (ML) model, ETL, and visualization/notification system to detect fraud in the clinical trials process. Composed of about 20 subsystems, the product was acquired and required reverse engineering of the architecture and design to scale the system to handle COVID mega trials with 25,000+ patients. My contributions included:
* ARC 42 architecture diagrams of current and future state of the project
* DevOps across the whole stack including:
  * creation of a JSON logging package for R and integration into Sumo Logic
  * operational consistency across the developer, test, and production environments (Docker + package locking) for Ruby/Rails, R, Python, and Clojure stacks
  * CI/CD pipeline automation including complex multi-system orchestration
  * the development of dozens of Sumo Logic dashboards to provide operational insights across 20+ web services
  * integration of SLO review into the sprint lifecycle across 10 engineering teams


## Machine Learning for Medical Coding -- Medidata

Design and implementation of a MLOps framework for managing and predicting MedDRA and WHODrug coding decisions.

## Housing Price Prediction -- Personal Project (2017)

Kaggle competition to predict housing prices in Ames, Iowa using varied ML models Linear, RandomForest, etc. Used traditional ML techniquest such as EDA, normalization, scaling, impute missingness, feature engineering, one-hot-encoding, label encoding, cross-validation, hyperparameter tuning (grid search), model selection and model evaluation.

## Biomarker Analysis Tool -- Personal Project (2017)

Seurat and t-SNE (R) analysis of 10x Genomics datasets to find cancer stem cells in mice tumors.

## Randomization and Trial Supply Management -- Medidata

The world’s first fully configurable randomization and trial supply management system (RTSM). I personally contributed over 3,000 commits to a SIMT Rails application that became the company’s highest revenue-generating product after their flagship product, Rave. Launched in 2009, the product was at the forefront of technology and software development at the time, featuring:
* TDD (RSpec) and BDD (Cucumber/Selenium) for fully automated testing
* CI/CD pipeline automation to run tests and create a validation portal automatically with every merged pull request, ensuring the system was always in a "deployable" state
* Rapid Application Development (RAD) despite regulatory requirements for independent peer review of 20,000+ pull requests
* Full traceability between requirements (JIRA), design (RSpec), implementation (Ruby/Rails), and tests, all programmatically updated through multiple system integrations

This is one of the projects I’m most proud of. An RTSM system can have life-or-death consequences if it ships with defects, as it determines which double-blind experimental drugs patients receive in clinical trials. We transformed an industry that was decades behind by focusing relentlessly on automation, effective testing, and challenging outdated norms.

This system was among the first clinical trial data management solutions to be hosted in the cloud (AWS), use SIMT (shared DB), and maintain a constant state of deployability. This approach defied the prevailing belief among sponsors and CROs that systems had to be on-premises, segmented at the database level by client and environment, and required at least six weeks of rigorous testing and validation before deployment.


## NYSERNet Grant Management Application

A greenfield project including architecture, design, and implementation of a LAMP stack to manage grants and internet provisioning for the New York State Education and Research Network. Work included
 * Database (MySQL) ERD design
 * System implementation in PHP + MySQL + Linux + Apache 
 * System operation including firewall (ipchains/iptables) management, database monitoring and optimizations, and software updates (OS and application-level)

## Survey Studio SaaS Application -- ReQuest Technologies

Originally implemented in Perl, I converted the entire LAMPerl stack to PHP.

## Clinical Trial Data Management Systems -- ReQuest Technologies / etrials

My first assignment fresh out of college was to install Oracle 7.5 onto SCO Unix via one of the most convoluted TUIs I've ever seen in my life. This first project always makes me think of the expression "what doesn't kill you makes you stronger".

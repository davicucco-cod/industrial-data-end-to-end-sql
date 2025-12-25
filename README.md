# Industrial Data Engineering & AI Integration

## Sobre o Projeto
Este projeto demonstra um pipeline completo de Engenharia de Dados (**End-to-End**), simulando o ambiente real de uma fábrica inteligente (Indústria 4.0).

O objetivo não é apenas treinar um modelo, mas construir toda a infraestrutura de dados que permite que a IA funcione em produção.

## Arquitetura do Pipeline
1.  **Ingestão (SQL):** Criação de banco de dados relacional (SQLite) e ingestão de dados brutos de sensores IoT.
2.  **Data Quality (ETL):** Implementação de regras de sanitização via SQL para tratar falhas de sensores (valores nulos e outliers) diretamente na fonte.
3.  **Analytics:** Geração de KPIs de chão de fábrica usando agregações (`GROUP BY`, `HAVING`).
4.  **Integração com AI:** Conexão do Banco de Dados com um modelo de Machine Learning (*Random Forest*) para prever falhas em tempo real.

## Resultados Alcançados
* **Single Source of Truth:** Unificação de dados dispersos em um banco estruturado.
* **Previsão de RUL:** O sistema lê o estado atual da máquina no banco e classifica a necessidade de manutenção (Ex: "ATENÇÃO - PLANEJAR" para máquinas com < 200h de vida útil).
* **Automação:** Eliminação de planilhas manuais para tomada de decisão.

## Tech Stack
* **Linguagem:** Python & SQL.
* **Bibliotecas:** Pandas, SQLite3, Scikit-Learn.
* **Conceitos:** ETL, Data Cleaning, Database Modeling, Predictive Maintenance.

---
*Desenvolvido por Davi Cucco | [LinkedIn](https://www.linkedin.com/in/davi-duarte-cucco-8b272a238/)*

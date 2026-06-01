# 🌐 Trabalho Final de Redes de Computadores: Apache Kafka

<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Kafka-000000?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka Badge">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5 Badge">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3 Badge">
</p>

---

## 🎯 Objetivo do Trabalho
Este repositório armazena o desenvolvimento do trabalho final da disciplina de **Redes de Computadores**. O objetivo principal é analisar a arquitetura e o funcionamento do **Apache Kafka** sob a ótica de redes, compreendendo como ele lida com streaming de dados distribuído, mensageria de alta performance, topologias de rede e tolerância a falhas.

O projeto conta com:
* **Estudo Teórico:** Análise aprofundada dos conceitos de Brokers, Clusters, Zookeeper/KRaft, Tópicos, Partições, Producers e Consumers.
* **Apresentação Prática:** Interface HTML explicativa e interativa para ilustrar o fluxo dos dados na rede.
* **Material de Apoio:** Código-fonte e roteiro para a apresentação em sala de aula.

---

## 🏢 Arquitetura do Apache Kafka (Foco em Redes)
No contexto de Redes de Computadores, o Kafka se destaca pela eficiência na camada de transporte e armazenamento de logs. O fluxo principal baseia-se no modelo Publish-Subscribe (Pub/Sub):

```mermaid
graph LR
    P[Producers] -->|Publish| B[Kafka Cluster / Brokers]
    B -->|Subscribe| C[Consumers]
    
    style B fill:#f9f,stroke:#333,stroke-width:2px
# 🧠 Blockchain-Based Recommender Systems – Comparative Study

This repository contains the implementation and experimental results of a **comparative analysis of blockchain-based recommender systems**. The project evaluates two main architectures:
- **Web3Recommend**: A decentralized, smart contract-driven collaborative filtering system.
- **Federated Blockchain Recommender System**: A privacy-preserving, federated learning approach secured by blockchain coordination.

> 📄 This project forms the basis of an academic research paper written in IEEE format, comparing real-world performance, scalability, and privacy trade-offs between the two systems.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Algorithms Implemented](#algorithms-implemented)
- [Results](#results)
- [Why Blockchain-Based RS?](#why-blockchain-based-rs)

---

## 🧾 Overview

The project focuses on answering:
- How do Web3-based RSs compare to federated blockchain RSs in accuracy and scalability?
- What are the trade-offs in terms of decentralization, privacy, and performance?
- Can these systems be implemented on real-world blockchain frameworks?

Three algorithms were implemented:
- `Web3 Cosine Similarity`
- `Web3 GraphJet-style Recommender`
- `Federated Matrix Factorization`

A subset of the **Last.fm dataset** (50,000 rows) was used for training and evaluation.

---

## 🛠 Technologies Used

| Tool              | Purpose |
|-------------------|---------|
| **Python 3.10**   | Core implementation, evaluation, and analysis |
| **Solidity**      | Smart contract development |
| **Hardhat**       | Local Ethereum environment for testing and deploying contracts |
| **Jupyter Notebooks** | Interactive implementation and visualization |
| **web3.py**       | Ethereum-Python integration |
| **Scikit-learn**  | Cosine similarity computation |
| **NetworkX**      | Graph-based recommendation (GraphJet) |
| **NumPy**         | Vectorized operations for matrix factorization |

---

## 🤖 Algorithms Implemented

### 🔹 Web3 Cosine Similarity
A user-based collaborative filtering model that uses smart contracts to record interactions and log recommendation scores. Similarities are computed off-chain and verified on-chain.

### 🔹 Web3 GraphJet
A real-time, graph-based recommender using co-visitation signals on a bipartite graph. Smart contracts store event logs and maintain traceability.

### 🔹 Federated Matrix Factorization
A privacy-preserving recommender where local models are trained on-device and encrypted updates are coordinated via blockchain smart contracts.

---

## Results

| Algorithm           | Precision | Recall | F1 Score | Hit Rate |
| ------------------- | --------- | ------ | -------- | -------- |
| Web3 Cosine         | 0.8545    | 0.0378 | 0.0692   | 1.0000   |
| Web3 GraphJet       | 0.8909    | 0.0395 | 0.0722   | 1.0000   |
| Federated MF (sim.) | 0.8650    | 0.0430 | 0.0794   | 0.9750   |


## 🔐 Why Blockchain-Based RS?

Blockchain-based recommenders solve key issues:

Privacy: No centralized data collection.
Transparency: Smart contracts make logic verifiable.
Decentralization: Removes platform control and promotes open ecosystems.
Auditability: Every interaction is traceable on-chain.
Cross-platform Portability: User profiles and preferences are wallet-based.


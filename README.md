# TP1 — Detecção de Anomalias Visuais

Repositório destinado ao Trabalho Prático I (TP1) da disciplina **BCC406 - Redes Neurais e Aprendizagem em Profundidade** (DECOM/UFOP).

## 📌 O Problema
O objetivo deste trabalho é desenvolver um modelo de **detecção de anomalias não supervisionada (one-class)** para imagens industriais. Em um cenário real de inspeção em linha de produção, defeitos são raros e imprevisíveis. Portanto, o modelo deve aprender uma representação do que é "normal" utilizando **apenas imagens sem defeitos** durante o treinamento. 

Durante o teste, o modelo deve ser capaz de receber imagens normais e defeituosas e produzir:
1. **Escore de Anomalia (Detecção):** Um valor que indica o quão anômala a imagem é.
2. **Mapa de Anomalia (Localização - Bônus/Pós-graduação):** Um mapa de calor destacando os pixels defeituosos.

## 🛠️ Restrições e Regras
- **Apenas CNNs:** O uso de arquiteturas baseadas em atenção (como Vision Transformers - ViT) é estritamente proibido.
- **Protocolo One-Class:** O conjunto de treinamento e validação contém *apenas* imagens normais.
- **Treinamento Próprio:** Pelo menos um componente da solução deve ser treinado usando retropropagação (fine-tuning, autoencoders, destilação, etc.).
- **Framework:** Desenvolvido em PyTorch.

## 📂 Conjunto de Dados
O trabalho utiliza o dataset **VisA (Visual Anomaly)**, composto por 12 categorias de objetos, abrangendo estruturas complexas, múltiplas instâncias e objetos únicos com pose variável.

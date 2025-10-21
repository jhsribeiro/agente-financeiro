# Agente de Análise Financeira com RAG e Gemini

Este projeto implementa um agente de conversação especializado em análise de relatórios financeiros, utilizando a arquitetura RAG (Retrieval-Augmented Generation). O agente é construído com Python, LangChain e os modelos de IA Generativa do Google (Gemini), sendo capaz de responder a perguntas complexas com base no conteúdo de documentos PDF.

## 📜 Funcionalidades

- **Carregamento e Processamento de Documentos:** Ingestão de relatórios financeiros em formato PDF.
- **Criação de Base de Conhecimento:** O texto é dividido em trechos (chunks) e vetorizado usando modelos de embedding do Gemini.
- **Busca Vetorial:** Utilização do FAISS para criar um Vector Store que permite buscas rápidas por similaridade semântica.
- **Geração Aumentada por Recuperação (RAG):** Uma cadeia LangChain recupera os trechos mais relevantes do documento e os fornece como contexto para o modelo Gemini gerar uma resposta precisa.
- **Agente Inteligente:** Um fluxo de conversação (grafo) é construído com LangGraph para gerenciar a lógica, decidir os próximos passos e fornecer respostas coerentes.

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Ambiente:** Google Colab
- **Orquestração de LLM:** LangChain & LangGraph
- **Modelos de IA:** Google Generative AI (Gemini Flash e Gemini Embedding)
- **Busca Vetorial:** FAISS (Facebook AI Similarity Search)
- **Processamento de PDF:** PyMuPDF

## 🚀 Como Executar

Siga os passos abaixo para configurar e executar o projeto no Google Colab.

**1. Clone o Repositório (Opcional, se quiser rodar localmente):**
```bash
git clone https://github.com/jhsribeiro/agente-analise-financeira-rag.git

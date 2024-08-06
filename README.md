# Trabalho Final de NLP - UFAM
### Trabalho final de NLP com aplicação da técnica de fine-tuning (LoRA) e implementação de um RAG com BM25

**Aluno**: Lennon Chaves

**Discplina**: Tópicos Especiais em Recuperação de Informação (TERI)

**Breve Resumo:** O principal objetivo deste trabalho foi desenvolver uma LLM capaz de responder perguntas sobre a legislação e normas acadêmicas da graduação da Universidade Federal do Amazonas (UFAM). Todas as informações sobre normas e legislações estão disponíveis no site da UFAM: https://proeg.ufam.edu.br/normas-academicas/57-proeg/146-legislacao-e-normas.html

### Etapas do Trabalho

**1. Download e Pré-Processamento da Legislação:** ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Pré-Pocessamento.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Etapa_Parte1_Parte2.ipynb)
- Download de todas as normas e legislações;
- Extração de documentos PDFs escaneados;
- Processamento dos textos dos documentos.
  
**2. Geração de Base de Dados Sintética de Instruções:** ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Geração Base Sintética.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Etapa_Parte1_Parte2.ipynb)
- Utilização de técnicas de geração de texto automatizado para criação de uma base de 1000 perguntas e respostas sobre a legilsção da UFAM.

**3. Fine Tuning com LoRA:** ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Fine-Tuning-LoRA.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Etapa_Parte3.ipynb)
- Aplicação da técnica LoRA (Low-Rank Adaptation) para fazer o tuning de instruções treinando com o modelo Gemma-7b;
- O modelo Gemma foi treinado com a base de dados sintética.
- Modelo com Fine Tuning: https://huggingface.co/lennonssss/gemma-7b-tuned 

**4. Implementação de RAG (Retrieval-Augmented Generation):** ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Implementação-RAG.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Etapa_Parte4.ipynb)
- Desenvolvimento de um RAG em chromaDB com aplicação de Rank do algoritmo BM25. 

### Entregáveis:
- Relatório Técnico:
- Base de Dados Sintética: [database_sintetica.csv](https://github.com/lennonchaves/llm-fine-tuning-rag/blob/main/database_sintetica.csv)
- Modelo com Fine Tuning: https://huggingface.co/lennonssss/gemma-7b-tuned
- Implementação RAG: ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Implementação-RAG.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Etapa_Parte4.ipynb)




#### Consideração Final:
O trabalho completo com todas as etapas em um único notebook podem ser acessadas em: ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg) [Trabalho-Final-Completo.ipnyb](https://colab.research.google.com/github/lennonchaves/llm-fine-tuning-rag/blob/main/TPFinal_Lennon_Chaves_Completo.ipynb)


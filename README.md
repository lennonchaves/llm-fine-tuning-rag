# Trabalho Final de NLP - UFAM
### Trabalho final de NLP com aplicação da técnica de fine-tuning (LoRA) e implementação de um RAG com BM25

**Aluno**: Lennon Chaves

**Discplina**: Tópicos Especiais em Recuperação de Informação (TERI)

**Breve Resumo:** O principal objetivo deste trabalho foi desenvolver uma LLM capaz de responder perguntas sobre a legislação e normas acadêmicas da graduação da Universidade Federal do Amazonas (UFAM). Todas as informações sobre normas e legislações estão disponíveis no site da UFAM: https://proeg.ufam.edu.br/normas-academicas/57-proeg/146-legislacao-e-normas.html

### Etapas do Trabalho

**1. Download e Pré-Processamento da Legislação:**
- Download de todas as normas e legislações;
- Extração de documentos PDFs escaneados;
- Processamento dos textos dos documentos.
  
**2. Geração de Base de Dados Sintética de Instruções:**
- Utilização de técnicas de geração de texto automatizado para criação de uma base de 1000 perguntas e respostas sobre a legilsção da UFAM.

**3. Fine Tuning com LoRA:**
- Aplicação da técnica LoRA (Low-Rank Adaptation) para fazer o tuning de instruções treinando com o modelo Gemma-7b;
- O modelo Gemma foi treinado com a base de dados sintética.

**4. Implementação de RAG (Retrieval-Augmented Generation):**
- Desenvolvimento de um RAG em chromaDB com aplicação do algoritmo BM25;

### Download e Pré-Processamento

### Geração de Base de Dados Sintética

### Fine Tuning com LoRA

- Modelo com Fine Tuning: https://huggingface.co/lennonssss/gemma-7b-tuned

### Implementação do RAG com Algoritmo BM25

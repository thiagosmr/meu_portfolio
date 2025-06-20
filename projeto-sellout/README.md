# Projeto X — Identificação Inteligente de Produtos em Notas Fiscais

## 💡 Sobre o projeto

O Projeto X foi desenvolvido para resolver um desafio crítico enfrentado por empresas da indústria farmacêutica:

**Como identificar automaticamente produtos em notas fiscais, mesmo com variações extremas de nomenclatura, abreviações e erros de grafia — e sem depender exclusivamente de correspondência textual.**

A solução implementa um pipeline inteligente que combina:

✅ Fuzzy Matching com `pg_trgm` (primeira camada de comparação textual)  
✅ Embeddings semânticos para validação contextual (segunda camada)  
✅ **Filtro final com LLM (ChatGPT)** para interpretação semântica completa e tomada de decisão em casos duvidosos (terceira camada)  
✅ Estrutura híbrida com fallback dinâmico  
✅ Interface REST simples (API) para integração com sistemas de ETL

O sistema é capaz de realizar curadoria em alto volume, com forte capacidade de interpretação contextual, reduzindo drasticamente o número de falsos positivos.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Python** (FastAPI)
- **PostgreSQL** com `pg_trgm` e `pgvector`
- **Sentence Transformers — MiniLM (384)**
- **Embeddings semânticos locais**
- **OpenAI ChatGPT (LLM contextual filtering)**
- **N8N** (orquestração com o ETL do cliente)
- **Docker Swarm** (deploy em VPS auto-hospedada)
- **Supabase** (painel de controle e dados auxiliares)

---

## 🚀 Resultados alcançados

- Precisão superior a 95% na identificação de produtos em NFs, mesmo com grafias inconsistentes
- Falso positivo reduzido com pipeline híbrido (regras + embeddings + LLM contextual)
- Processamento de grandes volumes (> 500 mil registros por lote)
- Curadoria e enriquecimento progressivo da base de variações
- Integração transparente com ETL corporativo, sem impacto nos fluxos atuais

---

## 📸 Prints do projeto


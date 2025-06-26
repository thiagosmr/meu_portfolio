# Projeto: Lia — Assistente Comercial Multi-Agente com IA

## 💡 Sobre o projeto

A Lia é uma assistente virtual multi-agente projetada para automatizar e otimizar o processo comercial de empresas.

Sua arquitetura é composta por:

✅ **Agente SDR** — captação e qualificação de leads via WhatsApp  
✅ **Agente de Agendamento** — integração com Google Calendar para marcar reuniões com controle de agenda e regras personalizadas  
✅ **Agente Pesquisador** — consulta em base vetorial (embeddings) para responder dúvidas frequentes (FAQ) com alta precisão  
✅ **Pipeline de Follow-up** — envio automático de relatórios para o closer   
✅ **Memória conversacional** — armazenamento de contexto (Postgres + Redis)

O projeto foi desenvolvido com foco em automação avançada, permitindo um atendimento comercial 24/7 altamente personalizado e eficiente.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **N8N** (orquestração e automação)
- **LangChain** (orquestração de LLM + memória + agentes)
- **Evolution API** (integração com WhatsApp)
- **Supabase** (armazenamento, base vetorial e contexto)
- **Redis** (cache e memória temporária)
- **PostgreSQL** (memória conversacional)
- **OpenAI GPT-4-mini** (modelo LLM principal)
- **Google Calendar API** (controle de agendamento)

---

## 🚀 Resultados alcançados

- Qualificação de leads em tempo real via WhatsApp
- Redução de 70% do tempo gasto no atendimento inicial
- Integração completa com agenda real da empresa, respeitando disponibilidade e regras de agendamento
- Base de conhecimento vetorial 100% atualizável e pesquisável
- Geração automática de relatórios para o closer com contexto da conversa
- Atendimento 24/7 com retenção de contexto entre sessões

---

## 📸 Prints do projeto

### Fluxo no N8N
![Fluxo N8N](images/n8n)

### Memória Conversacional no Postgres
![Memória Conversacional](images/memoria-postgres)

### Base FAQ Vetorizada (Supabase)
![FAQ Vetorizada](images/faq-vetorizada)

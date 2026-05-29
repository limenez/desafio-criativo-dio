# 🎯 Desafio Criativo — Prompt Final
## Extraindo Insights do Feedback de Clientes Bancários

---

## 🧱 Passo 1 — Definição da Intenção

Quero que a IA analise **comentários e avaliações de clientes** sobre os canais digitais de um banco (aplicativo móvel, internet banking, Pix e atendimento por chatbot) para identificar **reclamações recorrentes, pontos de satisfação e oportunidades de melhoria na experiência do usuário**.

O resultado será usado pela **equipe de Experiência do Cliente (CX) e pelo time de Produtos Digitais** para apoiar a **priorização do roadmap de melhorias no aplicativo e a redução de atrito nos canais de atendimento**.

A entrega deve conter:
- Um resumo executivo com os principais achados
- Uma tabela com temas, sentimento, evidência e ação sugerida
- Uma lista com as 3 prioridades mais críticas para ação imediata

O resultado será considerado bom se for **claro, baseado exclusivamente nos comentários fornecidos, organizado por prioridade e diretamente útil para tomada de decisão** — sem termos técnicos desnecessários.

---

## 🧱 Passo 2 — Contexto e Restrições

**Contexto:** Estou trabalhando com feedbacks de clientes bancários relacionados ao aplicativo móvel, Internet Banking, Pix, cartão de crédito e atendimento por chatbot.

**Dados disponíveis:** A base contém as seguintes colunas:
- `data_feedback` — data e hora do registro
- `canal` — canal de origem (app, internet banking, chatbot, agência)
- `produto` — produto mencionado (Pix, cartão, conta, investimentos)
- `texto_feedback` — comentário livre do cliente
- `nota_satisfacao` — nota de 1 a 5 (NPS simplificado)
- `segmento_cliente` — perfil do cliente (pessoa física, pessoa jurídica, premium)

**Critérios de análise:** A IA deve classificar os feedbacks por:
- **Tema** (autenticação, transferências, atendimento, interface, segurança)
- **Sentimento** (positivo, negativo, neutro)
- **Urgência** (alta, média, baixa — baseada na frequência e no impacto relatado)
- **Canal e produto** mencionados

**Cuidados e restrições:**
- Use apenas os dados fornecidos. Não invente números, causas ou conclusões
- Não exponha dados pessoais ou sensíveis (nomes, CPFs, números de conta)
- Se houver informação insuficiente, indique a limitação claramente
- Não tire conclusões que não tenham evidência direta nos comentários
- Use linguagem simples, direta e orientada à tomada de decisão

---

## 🧱 Passo 3 — Prompt Final Consolidado

---

> **Atue como analista sênior de Experiência do Cliente e Dados em um banco digital.**
>
> Sua tarefa é analisar feedbacks de clientes sobre o **aplicativo móvel, Internet Banking, Pix, cartão de crédito e atendimento por chatbot**, com o objetivo de **identificar temas recorrentes, sentimento predominante, urgências e oportunidades de melhoria**.
>
> ---
>
> **Contexto:**
> A análise será usada pela equipe de CX e pelo time de Produtos Digitais para priorizar melhorias no roadmap do aplicativo e reduzir atritos no atendimento digital. O foco é transformar comentários dispersos em insights claros, acionáveis e organizados por prioridade.
>
> ---
>
> **Dados disponíveis:**
> Os feedbacks fornecidos contêm os seguintes campos:
> - `data_feedback` — data e hora do registro
> - `canal` — canal de origem (app, internet banking, chatbot, agência)
> - `produto` — produto mencionado (Pix, cartão, conta, investimentos)
> - `texto_feedback` — comentário livre do cliente
> - `nota_satisfacao` — nota de 1 a 5
> - `segmento_cliente` — perfil do cliente (PF, PJ, premium)
>
> ---
>
> **Instruções de análise:**
> 1. Classifique os feedbacks por **tema** (ex: autenticação, falhas em transferências, interface confusa, demora no atendimento, elogios a funcionalidades), **sentimento** (positivo, negativo, neutro), **urgência** (alta, média, baixa) e **canal/produto** citado.
> 2. Identifique os principais padrões, problemas recorrentes, elogios e oportunidades de melhoria.
> 3. Para cada tema relevante, **aponte evidências diretamente nos dados** usando trechos curtos e representativos dos comentários (sem expor dados pessoais).
> 4. Sugira **ações práticas e concretas** para a equipe de CX e para o time de Produtos Digitais, com indicação de responsável sugerido.
>
> ---
>
> **Formato da resposta:**
> Entregue a análise em três blocos:
>
> **Bloco 1 — Resumo Executivo** (máximo 5 linhas):
> Síntese dos principais achados, com destaque para o sentimento geral, os temas mais críticos e o volume de feedbacks negativos vs. positivos.
>
> **Bloco 2 — Tabela de Insights:**
> | Tema | Sentimento | Urgência | Canal/Produto | Evidência (trecho do feedback) | Ação Sugerida | Responsável |
> |------|-----------|----------|---------------|-------------------------------|---------------|-------------|
>
> **Bloco 3 — Top 3 Prioridades:**
> Liste as 3 ações mais críticas com justificativa baseada na frequência e no impacto relatado pelos clientes.
>
> ---
>
> **Restrições obrigatórias:**
> - Use **apenas** os dados fornecidos. Não invente números, causas ou conclusões.
> - **Não exponha** dados pessoais ou sensíveis (nomes, CPFs, números de conta ou agência).
> - Se os dados forem insuficientes para uma conclusão, **indique a limitação** explicitamente.
> - Use linguagem **simples, direta e orientada à tomada de decisão** — sem jargões técnicos desnecessários.
> - Não ignore comentários negativos nem suavize críticas: reporte o que os dados mostram.

---

## ✅ Checklist de Revisão do Prompt

- [x] A tarefa está claramente definida?
- [x] O papel da IA foi especificado?
- [x] O contexto e o público-alvo foram descritos?
- [x] Os dados disponíveis foram detalhados?
- [x] O formato da resposta foi definido?
- [x] A IA sabe o que deve evitar?
- [x] Os critérios de qualidade foram estabelecidos?

---

*Desafio Criativo — DIO | Extraindo Insights do Feedback de Clientes Bancários*

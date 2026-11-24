# 🚀 PlanAI: Assistente Inteligente de Planejamento & Execução com Notion & ChatGPT

> Um ecossistema de produtividade modular que transforma objetivos abstratos em planos de ação estruturados, integrados à rotina real e blindados contra imprevistos.

---

## 🔗 Acesse o Planner no Notion

O template funcional e estruturado do projeto pode ser acessado diretamente através do link público abaixo:

👉 **[CLIQUE AQUI PARA ACESSAR O PLANNER NO NOTION](https://app.notion.com/p/PlanAI-Assistente-de-Planejamento-422abbfe864280d5a49ddec04ab15592?source=copy_link)**

---

## 📌 1. Problema e Diferencial

### O Problema
Planos de estudo, carreira e negócios frequentemente falham não por falta de vontade, mas por atrito operacional e falta de método na execução diária:
1. **Metas Abstratas:** Objetivos genéricos ou vagos como *"estudar inteligência artificial"* geram paralisia de decisão por falta de clareza do próximo passo.
2. **Desconexão com a Rotina:** Criação de cronogramas ideais que ignoram a capacidade real de tempo e energia do dia a dia, gerando cansaço e frustração.
3. **Vulnerabilidade a Imprevistos:** A ausência de planos de contingência estruturados faz com que o primeiro obstáculo desmonte todo o planejamento semanal.

### O Diferencial do PlanAI
O **PlanAI** combina inteligência generativa estratégica com persistência de dados relacional:
* **Divisão de Responsabilidades:** O **ChatGPT** atua como o *Estrategista e Arquiteto* (decompondo metas e formulando contingências), enquanto o **Notion** serve como a *Central do Motor de Execução* (rastreável e visual).
* **Metodologia em Habilidades Reutilizáveis:** Instruções sistêmicas padronizadas (prompts) que transformam a IA em etapas de planejamento modulares que servem para qualquer objetivo.
* **Integração Bidirecional Relacional:** As bases de dados do Notion são integradas por meio de relações nativas, garantindo que o progresso das tarefas retroalimente os objetivos principais de forma coordenada.

---

## 🛠️ 2. Tecnologias e Recursos Utilizados

| Ferramenta | Recurso Utilizado | Motivo da Escolha |
| :--- | :--- | :--- |
| **Notion** | Bases de Dados Relacionais | Conectar tarefas diárias do plano de ação às metas macros e riscos em visualizações coordenadas. |
| **Notion** | Propriedades Inteligentes | Uso de propriedades tipadas de forma rigorosa (`Date`, `Select`, `Multi-select`, `Status` e `Relation`) para estruturação limpa dos dados. |
| **Notion** | Tabelas em Linha (*Inline*) | Manter todo o painel de comando unificado em uma única tela principal e visualizável de forma prática. |
| **ChatGPT** | Prompts de Sistema Estruturados | Padronizar as habilidades metodológicas do assistente para responderem exatamente o esperado sem reexplicar o contexto. |
| **ChatGPT** | Saída Tabular em Markdown | Permitir a cópia limpa do cronograma da IA e colagem instantânea nas colunas estruturadas do Notion. |

---

## 🏗️ 3. Estrutura do Planner no Notion

O ecossistema é formado por **4 bases de dados centrais e interconectadas** que trabalham de forma coordenada:

```
 [🎯 DB: Objetivos & Metas]
        ▲
        │ (Relação Bidirecional 1:N)
        ▼
 [📋 DB: Plano de Ação] ───────► [🛡️ DB: Obstáculos & Riscos]
        │                             (Relação N:1)
        ▼
 [⏰ DB: Rotina & Blocos de Tempo]
```

### Dicionário de Dados do Notion

#### 1. `🎯 DB: Objetivos & Metas` (Visão Estratégica)
* **Objetivo** (coluna principal `Nome/Title`): Nome do objetivo refinado de forma SMART.
* **Área** (tipo `Seleção/Select`): Segmentação (Estudos, Carreira, Negócio, Saúde).
* **Status** (tipo `Status`): Não iniciado, Em andamento, Concluído.
* **Prazo Final** (tipo `Data/Date`): Data-limite para atingir a meta macro.
* **↗ DB: Plano de Ação** (tipo `Relação/Relation`): Conexão para as tarefas do plano de ação.

#### 2. `📋 DB: Plano de Ação` (Visão Operacional)
* **Tarefa** (coluna principal `Nome/Title`): Entregável granular iniciado por verbo.
* **Fase** (tipo `Seleção/Select`): Fase correspondente (Fase 1: Fundamentos, Fase 2: MVP, Fase 3: Portfólio).
* **Prioridade** (tipo `Seleção/Select`): Nível de criticidade (P1 - Essencial, P2 - Importante, P3 - Desejável).
* **Esforço Estimado** (tipo `Seleção/Select`): Tempo necessário (Baixo <1h, Médio 1h-3h, Alto >3h).
* **Status** (tipo `Status`): A fazer, Em progresso, Concluído.
* **Data Programada** (tipo `Data/Date`): Dia específico planejado para a execução.
* **↗ DB: Objetivos & Metas** (tipo `Relação/Relation`): Vínculo com a meta macro correspondente.

#### 3. `⏰ DB: Rotina & Blocos de Tempo` (Visão de Capacidade)
* **Bloco / Hábito** (coluna principal `Nome/Title`): Nome da janela de dedicação (ex: Deep Work Sábado).
* **Dias da Semana** (tipo `Seleção múltipla/Multi-select`): Dias em que o bloco ocorre (Segunda a Domingo).
* **Horário** (tipo `Texto/Text`): Faixa horária de foco (ex: 08:30 - 11:30).
* **Nível de Energia** (tipo `Seleção/Select`): Disposição física/mental requerida (Alto, Médio, Baixo).

#### 4. `🛡️ DB: Obstáculos & Riscos` (Visão de Blindagem)
* **Gatilho / Risco** (coluna principal `Nome/Title`): Evento gerador de atrito ou potencial atraso.
* **Probabilidade** (tipo `Seleção/Select`): Chance de ocorrer (Alta, Média, Baixa).
* **Impacto** (tipo `Seleção/Select`): Gravidade do impacto no plano (Alto, Médio, Baixo).
* **Regra Se-Então (Contingência)** (tipo `Texto/Text`): Ação alternativa clara a ser ativada imediatamente (ex: Se [Gatilho], Então [Ação]).

---

## 🧠 4. Habilidades (Skills) do Assistente

As Habilidades são instruções estruturadas de prompt que ensinam a IA a atuar em cada etapa do planejamento, formatando as saídas no padrão exato consumido pelo Notion.

### Habilidade 1: Esclarecer e Registrar o Objetivo (`Clarify & Lock`)
* **Descrição:** Transforma vontades vagas em um objetivo SMART rigoroso com escopo negativo delimitado.
* **Instruções de Sistema:**
```text
Você é a Habilidade 1 do PlanAI. Sua missão é entrevistar o usuário para refinar seu objetivo:
1. Garanta que o objetivo seja SMART: Específico, Mensurável, Atingível, Relevante e com Prazo definido.
2. Defina expressamente o Escopo Negativo (Não-Objetivos) para blindar o foco contra dispersões.
3. Entregue um resumo estruturado para copiar na base do Notion:
   - Nome do Objetivo: [Verbo no Infinitivo + Indicador + Prazo]
   - Indicador de Sucesso: [Critério numérico de entrega claro]
   - Prazo Final: [Data exata]
   - Não-Objetivos: [O que NÃO será feito]
```

### Habilidade 2: Desdobrar em Plano de Ação (`WBS Breakdown`)
* **Descrição:** Decompõe a meta em fases lógicas e tarefas atômicas executáveis que podem ser coladas diretamente na base do Notion.
* **Instruções de Sistema:**
```text
Você é a Habilidade 2 do PlanAI. Sua missão é quebrar o objetivo SMART definido em entregáveis práticos e atômicos (máximo de 3 horas de esforço por tarefa).
1. Divida o plano em 3 fases estruturais de evolução.
2. Defina para cada tarefa a Prioridade (P1, P2, P3) e o Esforço Estimado.
3. Retorne OBRIGATORIAMENTE em formato de tabela Markdown compatível com as colunas do Notion:
   | Tarefa | Fase | Prioridade | Esforço Estimado | Status | Data Programada |
```

### Habilidade 3: Adaptar o Plano à Rotina (`Routine Sync`)
* **Descrição:** Cruza os blocos de tempo livres e a energia declarada com as tarefas prioritárias (P1), aplicando uma margem de segurança.
* **Instruções de Sistema:**
```text
Você é a Habilidade 3 do PlanAI. Sua missão é conectar as tarefas P1 prioritárias à rotina real do usuário:
1. Mapeie a disponibilidade horária semanal, aplicando um Buffer de Segurança de 25% (planeje apenas 75% da capacidade útil).
2. Aloque tarefas de alta demanda cognitiva em blocos de alta energia e tarefas mecânicas em blocos de baixa energia.
3. Retorne um mapa de distribuição semanal claro separando os blocos e horários sugeridos para foco.
```

### Habilidade 4: Antecipar Obstáculos & Contingências (`Risk Shield`)
* **Descrição:** Realiza análise pré-morte operacional, antecipando falhas e gerando protocolos comportamentais imediatos.
* **Instruções de Sistema:**
```text
Você é a Habilidade 4 do PlanAI. Realize uma análise pré-morte do planejamento semanal:
1. Identifique os 3 a 4 riscos reais que podem ameaçar as entregas (ex: cansaço, reuniões extras, falta de internet).
2. Formule para cada risco uma regra condicional pragmática de mitigação no formato: "Se [Gatilho de Risco], Então [Ação Alternativa]".
3. Forneça o resultado formatado em tabela Markdown para colagem direta na base "DB: Obstáculos & Riscos".
```

### Habilidade 5: Revisar o Progresso (`Weekly Pulse`)
* **Descrição:** Avalia o status das entregas, calcula a taxa de conclusão e repactua o cronograma protegendo o prazo macro.
* **Instruções de Sistema:**
```text
Você é a Habilidade 5 do PlanAI. Conduza o ritual de check-in semanal de progresso:
1. Compare o realizado com o planejado para calcular a taxa de conclusão semanal.
2. Se a taxa for menor que 70%, ative a repactuação dinâmica: remova tarefas P3 (desejáveis) ou P2 para garantir a entrega das tarefas P1 dentro do prazo final.
3. Gere o resumo consolidado com: Vitórias, Aprendizados, Gargalos, Repactuações e Foco do próximo ciclo.
```

---

## 🧪 5. Demonstração Prática (Estudo de Caso)

### Caso Selecionado: Transição de Carreira para IA
* **Perfil:** Lucas Andrade, Analista de Suporte de TI.
* **Objetivo:** Migrar para Engenharia de IA Aplicada desenvolvendo portfólio prático em 90 dias.
* **Capacidade Semanal:** 8 horas disponíveis.

### Resultados Obtidos via Assistente e Registrados no Notion:
* **Objetivo SMART Refinado:** *"Construir e publicar 2 aplicações completas com IA Generativa (RAG + Agente) em repositórios públicos, documentados no GitHub, até 28 de Fevereiro de 2027."*
* **Plano de Ação Desdobrado:** Tarefas granulares organizadas por fases com prazos estipulados e prioridades definidas.
* **Rotina e Blocos de Tempo:** Mapeamento inteligente de blocos focados de "Deep Work" de 3 horas aos sábados e blocos "Foco Noturno" durante a semana.
* **Mitigação de Riscos:** Matriz com riscos mapeados (ex: horas extras no trabalho) associados à regra Se-Então correspondente.

---

## 📋 6. Checklist de Validação do Desafio

- [x] **Planner Estruturado:** O painel contém Plano de Ação, Rotinas, Riscos e Metas integrados de forma relacional.
- [x] **Habilidades de IA:** 5 instruções de sistema desenhadas de forma modular e reutilizável para qualquer objetivo.
- [x] **Demonstração de Sucesso:** Testado de ponta a ponta com dados reais simulados.
- [x] **Entrega Segura:** Sem dados pessoais sensíveis e com link público do Notion configurado corretamente para visualização.

---

## ⚖️ 7. Licença e Autoria
Projeto desenvolvido por Maurício Paim como desafio prático da Trilha de Assistentes de Planejamento com IA.  
Distribuído sob a licença MIT. Livre para uso e adaptações.

# Personas

> Produto de referência: dashboard web que compara provedores de nuvem (AWS, Azure, Google Cloud, Oracle) com métricas de **custo**, **desempenho** e **impacto ambiental** (PUE/energia/CO₂e), para apoiar decisões de migração e otimização (FinOps/GreenOps).

## 📌 Persona 1 — Bruna Almeida (Primária)
<img src="/docs/imagens/persona1.jpeg" width="200">

**Cargo:** Gestora de FinOps  
**Setor:** TI/Financeiro  
**Idade:** 33  
**Experiência:** 8+ anos em controle de custos de TI  

### Sobre
Responsável por prever gastos, criar budgets, negociar reservas (RI/SP) e reportar economia. Atua com múltiplos provedores e precisa traduzir custos técnicos em métricas de negócio (custo por cliente/feature/produto).

### Objetivos
- Reduzir o **custo por unidade de negócio** sem impactar a disponibilidade.
- Identificar **anomalias** rapidamente (spikes, drift).
- Gerar **relatórios mensais** claros para diretoria e áreas parceiras.
- Medir e acompanhar **emissões (CO₂e)** nos projetos críticos.

### Comportamentos
- Trabalha com planilhas e painéis; compartilha relatórios no fim do mês.
- Usa tags/labels e showback/chargeback.
- Valoriza **templates prontos**, filtros simples e export para PDF/CSV.

### Dores
- Dificuldade em **comparar multi-cloud** de forma unificada.
- **Curva de aprendizado** alta em ferramentas enterprise.
- Dados defasados (atraso no refresh) prejudicam decisões.

### Tarefas recorrentes
- [ ] Ver custo dia/mês por provedor/serviço/região.  
- [ ] Checar **top N** projetos que mais cresceram.  
- [ ] Simular economia com **RI/SP/rightsizing**.  
- [ ] Relatar **CO₂e por projeto** e tendência mensal.

### Como o produto ajuda
- Painéis **multi-cloud** unificados (custo × CO₂e).  
- **KPIs** e **rankings** com filtros rápidos por serviço/região.  
- **Export** (PDF/CSV) e **templates por persona**.  
- Índice composto configurável (**custo × carbono × desempenho**).

> **Citação representativa:** “Preciso mostrar, em 1 slide, onde o dinheiro está indo e quanto podemos economizar — sem abrir 5 ferramentas diferentes.”

---

## 📌 Persona 2 — Matheus Rocha (Secundária)

<img src="/docs/imagens/persona2.jpeg" width="200">

**Cargo:** Arquiteto/Engenheiro de Nuvem  
**Setor:** Engenharia/Plataforma  
**Idade:** 28  
**Experiência:** 5+ anos (infra como código, Kubernetes, observabilidade)  

### Sobre
Projeta e mantém workloads em múltiplas nuvens. Precisa balancear **SLA/performance** com **custo** e **padrões de arquitetura**. Quer dados operacionais acionáveis.

### Objetivos
- Encontrar **gargalos de desempenho** que elevam custo.  
- Validar impacto de mudanças (ex.: tipo de instância, região).  
- Automatizar recomendações (rightsizing/idle/auto-scaling).  

### Comportamentos
- Vive no terminal/CI/CD, consome dados via **APIs** e **dashboards técnicos**.
- Curte **drill-down** até recurso/namespace/pod (quando possível).

### Dores
- Métricas de custo **descoladas** das métricas técnicas.  
- Falta de **contexto** (quem/qual time gerou o gasto?).  
- Visão de **emissões** inexistente ou muito superficial.

### Tarefas recorrentes
- [ ] Investigar **spikes** por serviço/recurso.  
- [ ] Revisar **recomendações** (CPU/memória/storage/rede).  
- [ ] Comparar **regiões** e **tipos de instância**.  

### Como o produto ajuda
- **Drill-down** do custo até o nível necessário (ex.: projeto/serviço).  
- Relatório de **recomendações acionáveis** (prioridade × economia estimada).  
- Tabelas comparativas por **região/tipo** + projeção de impacto.

> **Citação representativa:** “Quero ver, em 5 minutos, o que mudar para reduzir 20% do custo sem mexer no SLA.”

---

## 📌 Persona 3 — Ana Ribeiro (Complementar)

<img src="/docs/imagens/persona3.jpeg" width="200">

**Cargo:** Especialista ESG / Sustentabilidade  
**Setor:** Estratégia/ESG  
**Idade:** 37  
**Experiência:** 10+ anos em relatórios GRI/ISSB/CSRD  


### Sobre
Responde por **inventário de emissões** (escopo 2/3 operacional do provedor), metas de redução e prestação de contas a stakeholders. Precisa cruzar custo com **CO₂e** e **energia renovável**.

### Objetivos
- Monitorar **emissões** por projeto/produto/região.  
- Evidenciar **tendência** e **projeção** anual.  
- Priorizar iniciativas com **maior redução de CO₂e por real investido**.

### Comportamentos
- Trabalha com painéis executivos e **exports** para relatórios corporativos.
- Revisa **metodologia** (fontes/fatores/assunções) e pede rastreabilidade.

### Dores
- Ferramentas de custo sem **módulo de carbono** consolidado multi-cloud.  
- **Metodologias** pouco transparentes (fatores de emissão, PUE, mix elétrico).  

### Tarefas recorrentes
- [ ] Acompanhar **CO₂e mensal** por programa.  
- [ ] Comparar **regiões** pelo **mix de energia**.  
- [ ] Selecionar projetos-piloto para redução de emissões.  

### Como o produto ajuda
- Painel de **CO₂e** com fonte/metodologia documentadas.  
- **Comparador de regiões** (custo × CO₂e × PUE).  
- **Export** para planilhas e relatórios (BigQuery/CSV/PDF).

> **Citação representativa:** “Se não consigo explicar a metodologia do número, não posso publicar.”

---

## Contexto de uso (comum às personas)
- **Cenários:** planejamento de migração, otimização de custos, revisão mensal, roadmap de sustentabilidade.  
- **Ambiente:** desktop/notebook (dashboard web); uso pontual em tablet/meeting room.  
- **Acessibilidade:** contraste adequado, tabelas com ordenação, export dos dados brutos, navegação por teclado.  
- **Dados:** conectores para AWS/Azure/GCP/Oracle; refresh diário (≥ 1×/dia) e possibilidade de forçar atualização.

## Critérios de sucesso por persona
- **Bruna (FinOps):** redução do **custo/MRR** e **tempo** para gerar o relatório mensal.  
- **Matheus (Engenharia):** número de **recomendações aplicadas** e **economia** associada.  
- **Ana (ESG):** **cobertura** e **qualidade** do inventário de emissões (rastreável), além da **tendência** de redução.

## Anti-personas (fora do escopo imediato)
- **Usuário sem qualquer vínculo com cloud/finanças/ESG** buscando “dashboard genérico”.  
- **Operações puramente on-prem** sem intenção de comparar com cloud.

---


## Análise de Concorrência

> Escopo: soluções usadas por gestores/FinOps/engenharia para **comparar custos e eficiência em nuvem** e, quando possível, **avaliar impacto ambiental** (GreenOps).  


---

### 1) Concorrentes 

| Concorrente | Link oficial | Descrição |
|---|---|---
| IBM **Apptio Cloudability** | https://www.apptio.com/products/cloudability/ | Plataforma FinOps multi-cloud com painéis de custo, alocação/chargeback, forecasting, rightsizing e módulos de sustentabilidade. | 
| VMware **Tanzu CloudHealth** | https://tanzu.vmware.com/cloudhealth | Gestão de custos multi-cloud com relatórios, políticas e governança; foco em visibilidade e otimização. |
| **CloudZero** | https://www.cloudzero.com/ | “Cost intelligence” com custo por cliente/feature/unidade de negócio; dashboards custom e usuários ilimitados. | 
| **Flexera One – Cloud Cost Optimization** | https://www.flexera.com/products/cloud-cost-optimization | Suíte corporativa de FinOps para visibilidade, governança e otimização multi-cloud. | 
| **AWS Cost Explorer** | https://aws.amazon.com/aws-cost-management/aws-cost-explorer/ | Ferramenta nativa para explorar custo/uso e previsões na AWS. |
| **Azure Cost Management + Billing** | https://azure.microsoft.com/services/cost-management/ | Relatórios, budgets, alertas e recomendações diretamente no Azure (sem custo adicional para recursos Azure). | 
| **Google Cloud Carbon Footprint** | https://cloud.google.com/carbon-footprint | Painel gratuito de emissões (escopos 1/2/3 operacionais da nuvem Google), com export para BigQuery. | 
| **Cloud Carbon Footprint (OSS)** | https://www.cloudcarbonfootprint.org/ | Ferramenta open-source para estimar energia/CO₂e em múltiplas nuvens, com painéis e API. | 


---

### 2) Características e Funcionalidades (resumo)

- **Cloudability:** alocação/chargeback, business mapping, budgets/forecast, rightsizing, scorecards, módulo de sustentabilidade.  
- **CloudHealth:** relatórios interativos multi-cloud, políticas/alertas de governança, otimização, visão híbrida.  
- **CloudZero:** custo por unidade de negócio/cliente/feature, painéis custom, bom suporte a Kubernetes/etiquetas.  
- **Flexera One:** visibilidade fim-a-fim, otimização em escala corporativa, governança e integração com inventário/licenças.  
- **AWS Cost Explorer:** relatórios pré-configurados, filtros/agrupamentos salvos, previsão, recomendações RI/SP.  
- **Azure Cost Management:** tagging, budgets/alerts, recomendações de rightsizing/occiosidade, integração nativa.  
- **GCP Carbon Footprint:** emissões por projeto/produto/região, visualizações e export para BigQuery.  
- **Cloud Carbon Footprint (OSS):** estimativa de kWh e CO₂e via APIs dos hypers, gráficos de tendência e API.

---

### 3) Opiniões sobre UX (colete e anexe prints)

- **Pontos relatados em reviews públicos (G2/Capterra/marketplaces):**
  - Cloudability/Flexera: muito poder, **curva de aprendizado** maior e **setup** mais denso em ambientes enterprise.
  - CloudHealth: interface geralmente vista como **clara**; dashboards e políticas bem avaliados.
  - CloudZero: elogiado por **facilidade de uso** e por traduzir custo em **métricas de negócio** (custo por cliente/feature).

---

### 4) Preços e Modelos de Negócio (alto nível)

- **Enterprise (Cloudability, CloudHealth, Flexera):** contratos anuais, normalmente atrelados ao **gasto em nuvem** (tiers/percentuais mínimos).  
- **CloudZero:** camadas com **usuários ilimitados** e ofertas via marketplaces (contrato/consumo).  
- **Nativos (AWS/Azure/GCP):** baixo custo ou **gratuitos** (podem cobrar por granularidade de uso/export); ótimos para baseline.  
- **OSS (Cloud Carbon Footprint):** gratuito; custos só de infraestrutura/execução e esforço de integração.


---

### 5) Padrões e Tendências do Mercado

- **FinOps integrado** (custo + governança + segurança) e **multi-cloud** como padrão.  
- Ascensão de **GreenOps**: módulos nativos de emissões e ferramentas OSS para CO₂e/energia.  
- **Democratização do acesso** (usuários ilimitados / métricas de negócio) para engajar stakeholders não-técnicos.  
- **Export/ETL first-class** (ex.: BigQuery, APIs) e conectores para manter dados frescos.

---

### 6) Relatório e Sumário dos Resultados

**Visão geral:**  
- Plataformas enterprise entregam **amplitude** e **governança forte**, mas pedem investimento e tempo de onboarding.  
- Soluções nativas dos hypers são **excelentes pontos de partida** (custo baixo), porém limitam **comparação multi-cloud**.  
- Para **sustentabilidade**, o GCP oferece painel oficial gratuito; o **Cloud Carbon Footprint (OSS)** cobre várias nuvens e pode embasar índices compostos custo×carbono.

---

### 7) Pontos Positivos/Negativos & Recomendações

**Pontos positivos do mercado atual**
- Ecossistema maduro de **painéis** e **recomendações de economia**.  
- Foco crescente em **métricas de negócio** (custo por cliente/feature) e **sustentabilidade**.

**Gaps/oportunidades para o nosso produto**
- **Multi-cloud custo+carbono lado a lado** com **pesos/índices** configuráveis.  
- **Onboarding guiado** com templates por persona (FinOps, Engenharia, Diretoria).  
- **Preço transparente** com **camada acadêmica/gratuita** e **usuários ilimitados**.  
- **Conectores + refresh confiável** (AWS/Azure/GCP/Oracle) e **export** (BigQuery/ATP).

**Recomendações práticas**
1. Implementar **Índice Composto** (custo × CO₂e × desempenho) com pesos ajustáveis.  
2. Oferecer **templates de dashboard** por persona/cenário (ex.: “FinOps mensal”, “Planejamento RI/SP”, “Sustentabilidade”).  
3. Publicar **roadmap de integrações** (connectors + SLAs de atualização).  
4. Incluir **modo demo** com dataset sintético para onboarding em < 5 minutos.

---


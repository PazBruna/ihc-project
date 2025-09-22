# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](http://lattes.cnpq.br/6747210702910392) e Prof. Dr. [Plino Thomaz Aquino Junior](http://lattes.cnpq.br/6186413528999908).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Título do TCC** sob orientação do Professor **Nome do Orientador** e desenvolvido pelos seguintes alunos:

- Bruna Pereira Paz
- Matheus Miranda Vieira

## Conhecendo o problema

### Descrição breve
Aplicação web (dashboard) que compara provedores de computação em nuvem (AWS, Azure, Google Cloud e Oracle) a partir de dados coletados e normalizados, evidenciando impactos técnicos, econômicos e ambientais da migração.

### Objetivo
Consolidar indicadores (custo, desempenho e sustentabilidade) em um painel interativo que auxilie decisões estratégicas de migração para nuvem.

### Usuário final
- Gestores e times de TI envolvidos em planejamento/avaliação de migração.
- Pesquisadores e estudantes de computação em nuvem, eficiência operacional e sustentabilidade.

### Principais benefícios
- Comparação transparente entre provedores por serviço/região.
- Apoio prático à decisão (custo × desempenho × impacto ambiental).
- Exploração interativa com filtros e relatórios exportáveis.
- Base reutilizável para estudos, apresentações e auditorias.

### Funcionalidades
- Gráficos comparativos de custos e indicadores ambientais.
- KPIs em cartões (ex.: custo médio/h, estimativa de emissões).
- Filtros por provedor, serviço e região; geração de relatórios.
- Ranqueamento com índices compostos (ponderação de critérios).

### Tecnologias e ferramentas
- Coleta de dados: APIs dos provedores e scripts em **Python**.
- Armazenamento: **Oracle Autonomous Transaction Processing (ATP)**.
- Front-end/visualização: **Oracle APEX** (dashboard interativo).
- Tratamento/normalização e estatística básica (médias ponderadas/índices).

### Contexto de uso
- Planejamento e avaliação de migração de workloads para nuvem.
- Estudos comparativos institucionais e atividades acadêmicas com métricas objetivas.

### Interface prevista
**Sim.** O projeto inclui um **dashboard interativo em Oracle APEX**.

## Desenvolvimento
- [Análise de Concorência](docs/2_concorencia.md)
- [Personas](docs/3_personas.md)
- [Cenário de Análise/Problema](docs/4_cenarios.md)
- [Análide de Tarefas](docs/5_analise_tarefas.md)
- [Prototipação em Papel](docs/6_prototipacao.md)
- [Coleta de Dados](docs/7_coleta_dados.md)
- [Ciclo de vida da engenharia de usabilidade](docs/8_ciclo_vida.md)
- [Modelo Conceitual](docs/9_modelo_conceitual.md) 
- [MOLIC](docs/10_molic.md)
- [FIGMA](docs/11_figma.md)
- [Planejamento da Avaliação](docs/12_planejamento_avaliacao.md)
- [Avaliação de IHC através de Inspeção Heurística](docs/13_heuristica.md)
- [Avaliação de Usabilidade baseado em Observação do Usuário](docs/14_observacao_usuario.md)

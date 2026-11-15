# Princípios arquiteturais do Oráculo BDP — 2026-11-14

Status: diretrizes aprovadas pelo responsável de produto; implementação e homologação pendentes.

## Núcleo
BDP é núcleo de discernimento organizacional independente de LLMs, agentes, RAG, MCP e Skills. Esses recursos são adaptadores ou executores auxiliares; regras, evidências, governança e memória de domínio permanecem próprias.

## Modelo de domínio
Os 11 componentes do BT Model são aplicados integralmente em organização, departamentos e funções: Propósito; Problema/Oportunidade; Proposta de Valor; Processos; Ativos; Canais; Ecossistema; Clientes/Pessoas; Jornada; Custos/Externalidades; Receitas/Impactos Positivos.
Cada unidade possui propósito específico que deve convergir, por contribuição verificável, ao propósito do nível superior. Os componentes são dimensões transversais, não departamentos. Começar pelo entendimento da cadeia de valor real e dos clientes.

## Evidências, estados e navegação
Fatos e evidências originam-se preferencialmente no nível funcional; estado departamental deriva de evidências funcionais, e organizacional dos níveis inferiores, com linhagem navegável e permissões. O CEO pode perguntar pelo estado atual e navegar do semáforo dos 11 componentes organizacionais para departamentos e funções, até fatos de origem. Cada componente pode ter evidência qualitativa/quantitativa. Distinguir verde verificado, desconhecido/insuficiência de dados, amarelo e vermelho. Estados não são meras médias.

## Sinapses e impactos
Representar relações verticais (mesmo componente entre níveis) e transversais (entre componentes, funções e departamentos), com tipo, direção, fonte, validade, confiança e evidência. Não inferir causalidade automaticamente de correlação. Explicar como uma ocorrência funcional pode contribuir para estados superiores e afetar outros componentes.

## Presente e futuro
Separar AS-IS observado de análises prospectivas de riscos E oportunidades. Prospectivas devem ser hipóteses/cenários com premissas, grau de confiança e horizonte temporal, não fatos consumados. Impactos diretos no cliente recebem prioridade de análise, sem suplantar automaticamente riscos legais, segurança, ambientais ou outros críticos.

## Propósito e Board
Identificar casos em que metas locais verdes coexistem com impactos adversos no propósito maior, clientes ou cadeia de valor. Escalonar desalinhamentos estratégicos materiais ao Board com evidências, impactos observados, hipóteses, alternativas e responsáveis humanos. Não automatizar decisões do Board.

## Agregação e matemática
Pesos, limiares e propagação de cores AINDA NÃO DEFINIDOS. Desenvolver a partir de casos reais, criticidade, cadeia de valor, alcance das sinapses e qualidade de evidências. Não mascarar um crítico por muitos verdes; testar sensibilidade, explicabilidade e exceções. Evitar falsa precisão.

## Governança
Segurança desde o início, segregação multi-tenant, controle de acesso por nível, proveniência, finalidade, auditoria, memória histórica, retenção e responsabilidade humana. BDK-QS01 é a primeira aplicação, com foco em ISO 9001 e análise crítica pela direção, sem pressupor substituição de SGQ.

## Critérios mínimos de aceitação
1. Instanciar 11 componentes nos três níveis e consultar convergência de propósito.
2. Navegar do estado organizacional até a evidência funcional com permissões.
3. Explicar a contribuição de cada ocorrência aos estados agregados.
4. Não converter ausência de dados em verde; preservar alertas críticos.
5. Exibir sinapses transversais com fonte e status de validação.
6. Separar fatos presentes de riscos e oportunidades futuros.
7. Sinalizar ao Board desalinhamento material entre metas locais e propósito organizacional.
8. Operar regras e trilha de evidências sem dependência obrigatória de um LLM.
9. Preservar decisão humana e trilha auditável.
10. Executar testes de regressão e casos adversariais antes de alegar homologação.

## Próximos passos
Inventariar ADRs e código existente, mapear lacunas, definir esquema de dados, protótipo navegável e casos de teste; validar matemática e semântica com casos reais antes de produção.

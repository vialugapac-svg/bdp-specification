# Ontologia de domínio do BT Model e do BDP

Versão: 0.1  
Data: 2026-11-16  
Status: especificação conceitual inicial; definições e relações propostas para validação semântica. Princípios já aprovados permanecem identificados como tais. Este documento não declara implementação ou homologação.

## 1. Objetivo

Definir, com linguagem comum e rastreável, os conceitos do domínio BT Model/BDP, as relações entre eles e as regras que limitam sua interpretação. A ontologia deve permitir que pessoas, aplicações e mecanismos de IA falem do mesmo domínio sem depender de significados implícitos.

Este documento complementa os princípios arquiteturais existentes. É referência conceitual para o BT Engine, o BDK-QS01, o Oráculo e futuras aplicações do BDP. Não prescreve uma tecnologia de representação nem um esquema de banco de dados.

## 2. Como ler o status das definições

- **Aprovado**: princípio já registrado como decisão ou diretriz do projeto.
- **Proposto nesta versão**: definição de domínio criada para tornar explícitos conceitos e relações; requer validação semântica do responsável do projeto.
- **Pendente**: decisão que depende de casos reais, validação ou definição posterior. Não tratar como regra implementada.

As relações, definições e exemplos desta versão não transformam hipóteses em fatos. O estado de implementação deve ser acompanhado separadamente.

## 3. Princípios de modelagem

1. Os 11 componentes do BT Model são dimensões transversais para interpretar o negócio; não são departamentos. **Aprovado.**
2. Os componentes aplicam-se nos níveis funcional, departamental e organizacional. Os fatos têm origem preferencial no nível funcional; as leituras superiores derivam de vínculos rastreáveis. **Aprovado.**
3. A cadeia de valor real, os clientes e as entregas de valor dão contexto à interpretação das relações. O Propósito orienta o discernimento. **Aprovado.**
4. Impactos diretos no cliente recebem prioridade de investigação, sem sobrepor automaticamente riscos legais, de segurança, ambientais ou outros riscos críticos. **Aprovado.**
5. Fato, evidência, hipótese, inferência, impacto potencial e decisão humana são tipos distintos de informação. **Aprovado.**
6. Relação, correlação ou sequência temporal, por si só, não comprova causalidade. Causalidade exige evidência suficiente e validação segundo critérios a definir. **Aprovado quanto à vedação de inferência automática; critérios de validação pendentes.**
7. Estado da situação e estado do tratamento são independentes. Resposta, ação ou mudança de prazo, isoladamente, não torna o estado factual verde. **Aprovado.**
8. Pesos, limiares, agregação e propagação matemática de estados permanecem pendentes; evitar falsa precisão.

## 4. Conceitos centrais

| Conceito | Definição de trabalho | Status |
|---|---|---|
| Organização | Entidade cujo propósito, cadeia de valor, unidades, componentes e evidências são analisados. | Proposto |
| Unidade organizacional | Elemento de uma estrutura de três níveis: função, departamento ou organização. | Aprovado |
| Componente BT Model | Dimensão transversal usada para interpretar aspectos do negócio em cada unidade organizacional. | Aprovado |
| Instância de componente | Aplicação de um componente a uma unidade, com contexto, estado, evidências e relações próprios. | Proposto |
| Propósito | Direção e razão de contribuição de uma unidade ou organização, usada como referência para discernimento e alinhamento. | Aprovado em princípio; redação operacional proposta |
| Cadeia de valor | Sequência e rede contextualizada de atividades, interfaces e entregas pelas quais a organização cria e entrega valor. | Aprovado em princípio; representação proposta |
| Cliente/pessoa | Pessoa ou grupo que recebe, participa, executa ou é afetado por uma entrega, processo ou impacto. Os papéis devem ser especificados no contexto. | Proposto |
| Processo | Conjunto de atividades relacionadas que transforma entradas em saídas e participa da cadeia de valor. | Proposto |
| Ocorrência | Evento ou condição identificada no trabalho, com origem, tempo, contexto e evidência disponível. | Proposto |
| Situação | Item submetido a discernimento e acompanhamento; pode ser ocorrência, não conformidade, risco ou oportunidade. A taxonomia completa requer validação. | Proposto |
| Evidência | Registro ou fonte identificável que sustenta, limita ou contradiz uma afirmação. Deve preservar origem, tempo, qualidade, finalidade e permissão. | Aprovado em princípio; atributos operacionais propostos |
| Fato | Afirmação sobre algo observado ou confirmado, sustentada por evidência e delimitada por contexto e tempo. | Proposto |
| Hipótese | Explicação ou possibilidade ainda não confirmada, com premissas e incerteza explícitas. | Aprovado em princípio |
| Inferência | Conclusão derivada de fatos, evidências e regras declaradas; deve expor o caminho de derivação e limites. | Aprovado em princípio |
| Impacto | Efeito observado ou potencial de uma situação ou relação sobre um componente, unidade, cliente, pessoa ou propósito. | Proposto |
| Sinapse | Relação relevante entre componentes, unidades, eventos ou partes da cadeia de valor, cuja origem e contribuição podem ser explicadas. | Aprovado em princípio; tipos definidos abaixo são proposta |
| Decisão | Determinação feita por pessoa com alçada, incluindo autoria, justificativa, data, contexto e elementos considerados. | Aprovado em princípio |
| Tratamento | Fluxo de atribuição, análise, ação, acompanhamento, verificação de eficácia e escalonamento de uma situação. | Aprovado em princípio |

## 5. Os 11 componentes e suas definições de trabalho

As definições abaixo são propostas semânticas iniciais. Devem ser validadas com casos de diferentes segmentos antes de serem tratadas como definições finais.

| Componente | Definição de trabalho |
|---|---|
| Propósito | Razão de existir e direção que orienta escolhas e contribuições da unidade ou organização. |
| Problema/Oportunidade | Necessidade, condição adversa ou possibilidade de melhoria que merece discernimento. |
| Proposta de Valor | Benefício ou valor que a organização pretende entregar a um cliente ou pessoa identificada. |
| Processos | Atividades relacionadas que convertem entradas em entregas e resultados. |
| Ativos | Recursos, conhecimentos, capacidades, infraestrutura, dados ou direitos necessários à operação e à entrega de valor. |
| Canais | Meios pelos quais a organização comunica, acessa, atende ou entrega valor a clientes e pessoas. |
| Ecossistema | Atores e entidades externos ou parceiros que influenciam ou participam da criação e entrega de valor. |
| Clientes/Pessoas | Clientes e demais pessoas relevantes como destinatários, participantes, executores ou afetados. |
| Jornada | Etapas, interações e experiências vividas por um cliente ou pessoa em relação à organização e sua entrega. |
| Custos/Externalidades | Recursos consumidos e efeitos externos, positivos ou adversos, associados à atividade da organização. |
| Receitas/Impactos Positivos | Entradas financeiras e demais resultados benéficos gerados pela organização, com evidência e contexto. |

**Regra de leitura:** a mesma evidência pode ser relevante para mais de um componente. Isso não significa que os componentes sejam equivalentes; cada vínculo deve explicar o aspecto observado.

## 6. Relações do domínio

As relações abaixo formam o vocabulário inicial. “Origem” e “destino” indicam os tipos de entidades que podem se conectar; regras de cardinalidade permanecem pendentes.

| Relação | Origem → destino | Significado e condição |
|---|---|---|
| possui_instância | Unidade → Instância de componente | A unidade é analisada por aquela instância de componente. |
| possui_propósito | Unidade → Propósito | O propósito declarado ou validado para a unidade. |
| contribui_para | Propósito/atividade → Propósito superior | Contribuição alegada ou demonstrada; exige explicação e evidência compatível. |
| participa_de | Unidade/Processo/Ator → Cadeia de valor | Indica participação contextualizada numa cadeia de valor. |
| entrega_valor_a | Proposta de valor/Processo → Cliente/Pessoa | Relaciona uma entrega pretendida ou observada ao destinatário. |
| executa | Unidade/Ator → Processo/Atividade | Indica responsabilidade ou participação operacional. O papel precisa ser identificado. |
| origina | Ocorrência → Unidade/Processo | Registra onde a ocorrência foi observada ou identificada. |
| sustentada_por | Fato/Inferência/Impacto → Evidência | Aponta a evidência que sustenta ou limita a afirmação. |
| envolve | Ocorrência/Situação → Instância de componente | Identifica os componentes diretamente envolvidos, sem presumir impacto causal. |
| relaciona | Sinapse → Entidade de origem e entidade de destino | Registra uma relação vertical ou transversal com tipo, direção, contexto e status de validação. |
| afeta | Ocorrência/Sinapse → Instância/Cliente/Pessoa/Propósito | Expressa impacto observado ou potencial, que deve ser tipado e fundamentado. |
| atribuída_a | Situação → Papel/Responsável | Define quem responde pelo tratamento em uma alçada e período. |
| tratada_por | Situação → Ação | Relaciona uma situação a ação proposta, aprovada ou executada. |
| verificada_por | Ação/Resultado → Evidência/Critério | Registra a verificação da execução e da eficácia. |
| decidida_por | Decisão → Pessoa/Papel com alçada | Preserva autoridade humana, autoria e justificativa. |
| deriva_de | Estado superior → Estado/evidência inferior | Permite navegar da leitura organizacional até a origem funcional. |
| escalada_para | Situação → Papel/Alçada superior | Registra escalonamento por regra, prazo, criticidade ou ineficácia. |

### 6.1 Tipos de sinapse

- **Vertical**: relação entre instâncias do mesmo componente em níveis organizacionais diferentes.
- **Transversal**: relação entre componentes, funções, departamentos ou partes da cadeia de valor.
- **Observada**: relação constatada e sustentada por evidência.
- **Hipotética**: relação proposta para investigação, ainda sem confirmação.
- **Causal**: relação de causa e efeito validada segundo critérios que ainda precisam ser definidos.

Uma sinapse deve expor, no mínimo, tipo, direção quando aplicável, origem, destino, contexto, fonte, período de validade, evidência, nível de confiança e estado de validação. Os campos específicos e suas escalas são pendentes.

## 7. Regras e restrições de interpretação

1. **Componentes não equivalem a estrutura hierárquica.** Uma função ou departamento não é, por si, um componente BT Model.
2. **A origem funcional deve permanecer rastreável.** Leituras departamentais e organizacionais são projeções fundamentadas em evidências inferiores; não devem aparecer como fatos independentes sem proveniência.
3. **Falta de evidência é desconhecido, não verde.** Exibir insuficiência, desatualização ou indisponibilidade da fonte quando aplicável.
4. **Não inferir causalidade automaticamente.** Correlação, coexistência ou sequência temporal podem iniciar investigação, não confirmar causa.
5. **Separar observado de prospectivo.** Estado atual (AS-IS), risco futuro, oportunidade, cenário e hipótese devem ser identificáveis e não confundidos.
6. **Separar situação de tratamento.** A resposta do responsável e o progresso da ação não determinam por si o estado factual do componente.
7. **A eficácia precisa de verificação.** Fechamento administrativo não equivale a eficácia comprovada; critérios e autoridades de validação dependem da política organizacional.
8. **Prioridade é contextual.** Impacto direto no cliente merece atenção prioritária de investigação; riscos críticos legais, de segurança, ambientais ou outros não podem ser automaticamente subordinados.
9. **Propósito e metas locais.** Uma meta local favorável não elimina a necessidade de expor evidências de desalinhamento material com propósito, cliente ou cadeia de valor.
10. **Decisão humana e alçada.** O sistema pode organizar evidências, propor interpretações e sugerir ações; decisões materiais permanecem com autoridade humana competente.
11. **Sem falsa precisão.** Não apresentar pesos, percentuais, confiança ou agregações sem método, dados e limites conhecidos.

## 8. Estado da situação e estado do tratamento

Representar separadamente:

- **Estado factual do componente/situação**: leitura baseada em evidências, impactos, critérios e atualidade da informação. O vocabulário visual pode incluir verde verificado, amarelo, vermelho e desconhecido/insuficiência de dados; critérios de cor permanecem pendentes.
- **Estado do tratamento**: acompanhamento do responsável, prazo, análise, plano, ação, verificação, eficácia, atraso e escalonamento. A taxonomia de estados é inicial e deve ser validada.

O BDP pode sugerir responsável, prioridade e prazo inicial com base em criticidade, impactos, cadeia de valor, cliente, políticas e evidências. Pessoa com alçada pode confirmar ou ajustar com justificativa auditável. Algoritmos, calendários, SLAs, limites e limiares não estão homologados.

## 9. Exemplo de leitura, sem afirmar causalidade

1. Uma ocorrência é registrada numa função, com data, contexto e evidências.
2. A ocorrência é vinculada aos processos e instâncias de componentes que a evidência sustenta.
3. Uma possível sinapse com outra função, componente ou etapa da cadeia de valor é registrada como hipótese se ainda não estiver validada.
4. O BDP apresenta efeitos observados separados de impactos potenciais e informa o nível de confiança e as lacunas de evidência.
5. A situação é atribuída ao responsável competente, com prazo proposto e regra de escalonamento aplicável.
6. O tratamento acompanha resposta e ação. O estado factual só muda mediante evidência e critério de avaliação; a eficácia é registrada separadamente.
7. Se houver reflexo departamental ou organizacional, a projeção mantém ligação navegável à evidência funcional.
8. Uma decisão humana, inclusive ajuste de prazo, prioridade ou interpretação, conserva autoria, justificativa e histórico.

Este fluxo é um exemplo de aplicação das relações e princípios; não certifica que os contratos de software já existem.

## 10. Decisões ainda pendentes

- Definições finais e limites semânticos de cada componente, validados em segmentos reais.
- Subtipos e taxonomia de ocorrências, não conformidades, riscos, oportunidades, causas, impactos e decisões.
- Cardinalidades e regras para unidades, propósitos, processos, clientes e componentes.
- Critérios de qualidade, suficiência, atualização e conflito entre evidências.
- Critérios para validar causalidade, eficácia e níveis de confiança.
- Matriz de criticidade, pesos, limiares, agregação e propagação de estados.
- Semântica e escalas para severidade, prioridade, confiança, temporalidade e materialidade.
- Regras de acesso, visibilidade e retenção para cada tipo de entidade e relação.
- Formato técnico canônico e contratos de serialização, depois da validação semântica.
- Mapeamento para ISO 9001 e outros referenciais sem confundir norma, processo, componente BT Model e estrutura organizacional.

## 11. Próxima evolução

1. Validar as definições propostas dos 11 componentes com exemplos concretos do BDK-QS01 e de outros contextos.
2. Registrar contraexemplos e ambiguidades antes de fechar vocabulário.
3. Revisar compatibilidade desta ontologia com ADRs, Shared Runtime, memória organizacional e contratos existentes.
4. Só então derivar esquema técnico e casos de validação, mantendo versionamento, proveniência e revisão humana.
5. Atualizar esta especificação quando decisões forem aprovadas; registrar pendências sem preencher lacunas por inferência.

## Referências internas

- [Princípios arquiteturais do Oráculo BDP — três níveis](./PRINCIPIOS-ORACULO-BDP-TRES-NIVEIS-2026-11-14.md)
- [Princípio: responsabilidade primária, prazo, escalonamento e semáforo contínuo](./PRINCIPIO-ESCALONAMENTO-E-SEMAFORO-CONTINUO-2026-11-14.md)
- [Princípio: prazos propostos pelo BDP e validados por autoridade humana](./PRINCIPIO-PRAZOS-PROPOSTOS-PELO-BDP-2026-11-14.md)
- [BDP como núcleo independente de discernimento](../../ADR/PRINCIPIO-BDP-NUCLEO-INDEPENDENTE-DISCERNIMENTO-2026-11-14.md)

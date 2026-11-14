# EXP-001 — BDK-QS01 como laboratório multiagente do BDP

Status: PROPOSTA PARA TESTE (não implementado)
Data: 2026-11-14
Escopo: experimento offline, com dados sintéticos, sem integração com clientes.

## Objetivo
Validar se agentes especializados podem apoiar o BDK-QS01 sem substituir o BT Engine como núcleo de interpretação sistêmica, sinapses e discernimento. Não presumir ganhos de desempenho antes da medição.

## Princípios invariantes
1. Propósito no centro; entender primeiro a cadeia de valor real da organização e de seus clientes.
2. Os 11 componentes do BT Model são dimensões transversais, não departamentos.
3. Priorizar investigação de impactos diretos ao cliente, sem precedência automática sobre riscos legais, segurança, ambientais ou outros críticos.
4. Fatos e evidências nascem no nível funcional; os níveis departamental e organizacional são projeções rastreáveis, não fatos independentes.
5. Separar fato, hipótese, inferência, impacto potencial e decisão humana. Não fabricar causalidade, percentual, ROI ou evidência.
6. A base cristocêntrica do discernimento é aplicável a qualquer perfil de cliente e não impõe religião.
7. Segurança desde a origem: menor privilégio, segregação por tenant, autorização, origem/finalidade/permissão de dados, segredos protegidos, auditoria, retenção e backups adequados ao estágio.
8. Sem decisões executivas autônomas. O responsável humano aprova conclusões e ações.

## Papéis experimentais (interfaces, não necessariamente LLMs distintos)
- Coletor de evidências: recebe eventos funcionais e aponta origem, integridade, lacunas e permissões.
- Analista de NC: classifica a não conformidade, responsável pelo processo, requisito e status; não transfere automaticamente a execução à Qualidade.
- Analista de impactos: propõe relações com cadeia de valor, cliente e componentes BT Model; identifica hipóteses e incertezas.
- Preparador de análise crítica: organiza insumos para ISO 9001 9.3 e questões à direção; não homologa decisões.
- BT Engine: reconcilia evidências, avalia sinapses transversais e apresenta caminhos explicáveis para discernimento.
- Governança: aplica autorização, trilha de auditoria, isolamento e revisão humana a todos os papéis.

## Contrato mínimo de entrada
event_id, tenant_id sintético, timestamp, nível funcional, processo, descrição, fonte, evidências/referências, classificação de acesso, responsável humano, cadeia de valor contextualizada.

## Contrato mínimo de saída
finding_id, event_id, componentes BT Model relacionados, elo na cadeia de valor, tipo (fato/hipótese/inferência), evidências citadas, confiança justificada sem percentual inventado, impactos diretos/indiretos, criticidade e fundamento, lacunas, agente/versão, timestamp, status de revisão humana.

## Cenário piloto sintético
Uma NC funcional registra atraso de liberação de lote por falha de calibração de equipamento. O experimento deve distinguir efeitos comprovados de efeitos apenas possíveis sobre entrega, cliente, custo, conformidade e demais componentes. Não atribuir perda financeira sem base.

## Procedimento
1. Inventariar runtime, ADRs, testes e contratos existentes; não alterar arquitetura antes do diagnóstico.
2. Registrar baseline de testes e segurança.
3. Executar caso piloto com um fluxo sequencial e determinístico; agentes inicialmente simulados quando apropriado.
4. Comparar saída individual e consolidada com gabarito revisado por humano.
5. Testar ausência de evidência, dados contraditórios, acesso indevido e tentativa de induzir decisão automática.
6. Executar regressões e documentar resultados, limitações e custo/latência.
7. Decisão humana: adotar, ajustar ou descartar arquitetura multiagente.

## Critérios de aceite (propostos)
- 100% das afirmações factuais do relatório vinculadas a evidências rastreáveis no conjunto de teste.
- Nenhuma inferência apresentada como causalidade demonstrada.
- Nenhum acesso entre tenants ou vazamento de informação restrita nos testes negativos.
- Nenhuma ação executiva sem aprovação humana.
- Nenhuma regressão na suíte previamente aprovada.
- Toda saída relevante identifica lacunas, versão e responsável por revisão.

## Não objetivos
Produção SaaS, integrações externas, coleta de dados reais, automação de decisões, substituição do SGQ, criação de múltiplos agentes apenas por conveniência.

## Próxima decisão
Aprovar o desenho do experimento e conferir a compatibilidade com Shared Runtime v0.1, ADR-005 e contratos reais antes de implementar. O prompt Grokbot é referência de planejamento, não dependência técnica aprovada.

# Princípio: máxima agilidade operacional sob autoridade humana

Status: diretriz de produto aprovada em 2026-11-14; implementação pendente.

O BDP/BT Engine/Oráculo deve detectar, explicar e antecipar riscos e oportunidades, mas também agilizar o tratamento, fazendo o máximo permitido pelas regras e delegações humanas. Não deve se limitar a responder perguntas ou emitir alertas.

## Autonomia graduada
1. Automação de baixo impacto, previamente autorizada: ingestão, análise, registro, consolidação de evidências, preparação de recomendações.
2. Delegação operacional explícita: abertura de tarefas e ocorrências, notificações, solicitações de dados, acompanhamento de prazos e cobranças proporcionais, respeitando papéis e permissões.
3. Aprovação humana específica: mudanças materiais, irreversíveis ou com efeitos relevantes em contratos, clientes, recursos financeiros, processos críticos, riscos legais e estratégia.

## Fluxo
Evento/evidência -> avaliação das sinapses e consequências -> classificação do risco/oportunidade e confiança -> sugestão de ações -> execução permitida ou pedido de aprovação -> acompanhamento -> verificação de eficácia -> memória organizacional. Separar fatos de cenários e nunca inventar causalidade.

## Controles
Autorização por papel/tenant, escopo, limites de impacto, segregação de funções, confirmação de decisões materiais, idempotência, logs auditáveis, responsável humano, revogação, escalonamento ao Board quando material e possibilidade de suspensão da automação. Integrações devem ser explicitamente habilitadas; ausência de conexão não implica execução.

## Aceitação
- Detectar evento e abrir registro rastreável.
- Executar apenas ações autorizadas e demonstrar quem delegou.
- Bloquear e solicitar aprovação para ação fora do escopo.
- Informar responsáveis e acompanhar prazos sem assumir decisões humanas.
- Mostrar evidência, estado, hipótese e histórico de cada ação.
- Verificar eficácia após tratamento e retroalimentar análise.
- Testar revogação, permissões cruzadas, duplicação e falha de integração.

Referência complementar: docs/architecture/PRINCIPIOS-ORACULO-BDP-TRES-NIVEIS-2026-11-14.md

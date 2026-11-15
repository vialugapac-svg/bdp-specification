# Princípio: responsabilidade primária, prazo, escalonamento e semáforo contínuo
Data: 2026-11-14
Status: decisão conceitual aprovada; implementação pendente.

## Regra principal
Cada situação identificada pelo BDP deve ser atribuída primeiro ao responsável competente da função de origem, com prazo explícito conforme criticidade e regras da organização. O responsável pode registrar resposta, plano, ações e evidências. Se não responder dentro do prazo, o Oráculo escala automaticamente ao gestor departamental e, se persistir, à direção/Board conforme alçadas, criticidade e matriz de escalonamento. Situações críticas podem exigir aviso simultâneo ou imediato à autoridade competente, sem aguardar prazos incompatíveis com o risco.

## Dois estados independentes
1. Estado da situação (semáforo BT Model): reflete evidências e impactos reais nos componentes funcionais, departamentais e organizacionais. Atualização contínua orientada a eventos e disponibilidade das fontes; exibir data/hora da última evidência, origem, qualidade, latência e estado desconhecido quando apropriado. Não prometer tempo real sem fontes integradas.
2. Estado do tratamento: novo, atribuído, ciência, em análise, plano aprovado, em execução, aguardando verificação, eficaz, ineficaz, vencido, escalado, encerrado (taxonomia inicial a validar). Ação ou resposta não tornam componente verde; somente evidência de melhoria e critério de eficácia validado.

## Autonomia e governança
Automatizar registro, atribuição, notificações, lembretes, abertura de tarefas e escalonamento apenas dentro de políticas e permissões. Ações materiais e decisões estratégicas requerem aprovação humana; manter logs de autorizações, responsáveis, tempos e justificativas. Preservar segregação de funções, trilha de auditoria, acesso por alçada, proteção contra alertas duplicados e tratamento de ausência/férias/substituição de responsáveis.

## Regras de negócio a detalhar
- Matriz de criticidade e SLA por categoria, função e risco; relógio, calendário e fuso horário.
- O que constitui resposta válida, ação adequada, evidência suficiente e eficácia confirmada.
- Escalonamento por ausência de resposta, atraso de ação, deterioração do risco ou evidência de ineficácia.
- Sinapses propagam impactos entre os 11 componentes e os três níveis com explicabilidade, sem mascarar críticos por média.
- Riscos e oportunidades prospectivos separados do AS-IS; metas locais verdes podem coexistir com desalinhamento material a expor ao Board.

## Critérios de aceitação
1. Situação com responsável primário, prazo, justificativa e evidência.
2. Resposta dentro do prazo não gera escalonamento por silêncio, mas mantém acompanhamento de eficácia.
3. Falta de resposta provoca escalonamento na alçada prevista e registro auditável.
4. Não resposta reiterada avança na cadeia de escalonamento; exceções críticas são imediatas.
5. Semáforo muda por evidência validada, independentemente de notificações e respostas.
6. Fonte indisponível ou evidência desatualizada não é tratada como verde.
7. CEO pode navegar de estado organizacional à evidência funcional e histórico de tratamento.
8. Ações automatizadas respeitam permissões, limites e decisões humanas.

## Pendências
Definir SLA e limiares com casos reais, critérios de eficácia, arquitetura de eventos, políticas de acesso e testes de regressão antes de alegar implementação.

# Princípio — prazos propostos pelo BDP e validados por autoridade humana

Data: 2026-11-14
Status: decisão conceitual aprovada; implementação e parâmetros pendentes.

O BDP/Oráculo deve sugerir automaticamente responsável, prioridade e prazo inicial de tratamento de situações, riscos e oportunidades com base em criticidade, impactos observados e potenciais, cadeia de valor, efeitos no cliente, políticas e evidências disponíveis.

Uma pessoa com alçada adequada deve poder confirmar ou ajustar a proposta, com justificativa, autoria, data e trilha de auditoria. Alterações não podem permitir prorrogações indefinidas ou contornar limites críticos e escalonamentos; exceções exigem aprovação em alçada superior.

O acompanhamento distingue: (a) estado factual dos componentes BT Model e semáforos nos três níveis, atualizado conforme evidências; (b) estado do fluxo de tratamento, prazo e escalonamento. Resposta, aceite, mudança de prazo ou início de ação não transformam automaticamente o estado factual em verde.

Requisitos de desenvolvimento:
- Configurar matriz de criticidade, SLA, horários/calendários, limites de prorrogação, papéis e substitutos.
- Explicar a base de cada prazo proposto e registrar qualidade das evidências e incertezas.
- Notificar responsável primário, monitorar prazo, alertar e escalar por silêncio, atraso, agravamento ou ineficácia.
- Proteger riscos urgentes com escalonamento imediato quando a gravidade impedir espera.
- Testar alterações de prazo sem justificativa, falta de alçada, repetidas prorrogações, indisponibilidade de fonte e atualização do semáforo independentemente do workflow.

Não há algoritmo de prazos, pesos ou limites numéricos homologados neste documento.

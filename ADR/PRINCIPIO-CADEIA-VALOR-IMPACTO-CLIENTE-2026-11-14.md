# Princípio arquitetural — Cadeia de valor, propósito e impacto no cliente

Data: 2026-11-14
Status: princípio aprovado conceitualmente; implementação pendente de especificação e validação
Aplicação: BDP, BT Engine, BDK-QS01 e Oráculo

## Enunciado normativo

O BDP DEVE identificar e contextualizar a cadeia de valor real da organização, seus clientes e as entregas de valor antes de interpretar e priorizar sinapses e impactos entre os 11 componentes do BT Model. O Propósito permanece como referência central do discernimento. Impactos diretos no cliente DEVEM receber atenção prioritária na análise, sem determinar automaticamente a maior criticidade nem suplantar obrigações legais e riscos graves de segurança, ambientais ou outros.

## Regras

1. Identificar segmento, contexto, clientes, entregas, processos e interfaces relevantes da cadeia de valor, registrando fontes, versão e responsável pela validação humana.
2. Mapas de sinapses por segmento são hipóteses de referência, ajustáveis e sujeitas a validação; não são diagnóstico nem causalidade comprovada.
3. Registrar fatos e evidências no nível funcional; representar reflexos departamentais e organizacionais somente com vínculos fundamentados, temporalidade e permissões.
4. Diferenciar impacto observado, impacto potencial e hipótese; não propagar automaticamente cor, prioridade, criticidade ou percentuais entre níveis ou componentes.
5. Avaliar alcance sobre cliente, gravidade, probabilidade quando estimável, urgência, reversibilidade, obrigações e riscos críticos; não criar pontuação ou peso universal sem calibração e validação.
6. Toda prioridade apresentada deve ser explicável: fato de origem, cadeia de relações, evidências, lacunas, critérios e decisão/responsável humano.
7. Sem cadeia de valor validada, permitir diagnóstico preliminar sinalizado como tal; impedir afirmações categóricas de causalidade ou prioridade baseada no cliente.
8. Respeitar segregação por tenant, controle de acesso, minimização de dados, auditoria e segurança desde a concepção.

## Aplicação inicial no BDK-QS01

Para cada não conformidade, auditoria, indicador, risco ou entrada de análise crítica da direção (ISO 9001, cláusula 9.3), registrar vínculo com processo/função, evidência e eventual consequência na cadeia de valor e no cliente. O relatório deve separar evidências de hipóteses e mostrar a justificativa da priorização; não substituir a decisão da direção.

## Critérios mínimos de aceitação futuros

- Caso A: falha interna sem efeito demonstrado no cliente não recebe automaticamente prioridade máxima.
- Caso B: atraso de entrega com evidência de efeito no cliente apresenta cadeia rastreável e destaque na análise.
- Caso C: risco grave legal, ambiental ou de segurança pode superar impacto direto no cliente, com justificativa.
- Caso D: ausência de evidência é explicitada; não há causalidade ou percentuais inventados.
- Caso E: dados de outro tenant ou fora da permissão nunca são exibidos na explicação.
- Caso F: mudança na cadeia de valor exige versionamento e reavaliação, sem reescrever o histórico.

## Limite da decisão

Este documento define princípio e requisitos de desenho. Não homologa algoritmo, pesos, testes, implantação nem diagnóstico organizacional. Mudanças de motor e priorização requerem proposta, testes de regressão e validação humana.

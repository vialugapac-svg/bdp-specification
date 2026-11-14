# EXP-001 — Diagnóstico inicial de compatibilidade

Data: 2026-11-14
Status: REVISÃO DOCUMENTAL PARCIAL; sem execução de testes, sem alteração de código do BDP.

## Repositórios consultados
- vialugapac-svg/bdp-specification: README e ADR/PRINCIPIO-CADEIA-VALOR-IMPACTO-CLIENTE-2026-11-14.md
- vialugapac-svg/bdp (privado): AGENTS.md; docs/PROTOCOLO-TRANSVERSAL-ARQUITETURA-GOVERNANCA-BDP.md; busca pontual por ADR-005, SharedRuntime e QS01.

## Achados confirmados
1. O protocolo transversal já separa Observar, Interpretar, Recomendar e Executar; requer evidências, AS-IS/TO-BE, governança de dados/agentes, memória reavaliável, alçadas e auditoria.
2. AGENTS.md exige consulta seletiva ao RADAR, decisão humana antes de adotar tecnologia e prioridade à homologação BDK-QS01/I2.B.
3. A norma de cadeia de valor exige contexto real antes da priorização de sinapses e destaque explicável para impactos diretos no cliente sem sobrepor riscos críticos.
4. A documentação encontrada menciona ADR-005 e Shared Runtime, mas esta revisão ainda não localizou nem examinou seus contratos de implementação.
5. O protocolo indica explicitamente corrigir e homologar a reavaliação das sinapses/supports I2.B antes de ampliar o MVP.

## Avaliação de compatibilidade
- Conceitual: COMPATÍVEL, condicionada a agentes como papéis delimitados e BT Engine como núcleo.
- Contratos de runtime, persistência e memória: NÃO VERIFICADOS.
- Segurança multi-tenant efetiva: NÃO TESTADA.
- Baseline e regressões: NÃO EXECUTADOS nesta revisão; não inferir aprovação de relatos históricos.
- Homologação funcional I2.B: NÃO VERIFICADA nesta revisão.

## Decisão operacional recomendada
Não implementar agora uma camada multiagente nova. Primeiro concluir diagnóstico do código, contratos e testes, e preservar a prioridade de I2.B. Preparar um teste offline sintético e reversível que não altere o produto nem repositório privado até autorização de mudança específica.

## Checklist de próxima inspeção
- Identificar paths e versões reais do Shared Runtime e da ADR-005.
- Localizar implementação do fluxo BDK-QS01/I2.B, testes, fixtures e comandos de execução.
- Reproduzir baseline em ambiente isolado; registrar totais, falhas, duração e commit.
- Mapear contratos de evidência, tenant, autorização, sinapse e reavaliação histórica.
- Só então especificar adaptadores de agentes sem duplicar memória nem lógica de discernimento.

Referências:
- https://github.com/vialugapac-svg/bdp/blob/main/AGENTS.md
- https://github.com/vialugapac-svg/bdp/blob/main/docs/PROTOCOLO-TRANSVERSAL-ARQUITETURA-GOVERNANCA-BDP.md
- https://github.com/vialugapac-svg/bdp-specification/blob/main/ADR/PRINCIPIO-CADEIA-VALOR-IMPACTO-CLIENTE-2026-11-14.md

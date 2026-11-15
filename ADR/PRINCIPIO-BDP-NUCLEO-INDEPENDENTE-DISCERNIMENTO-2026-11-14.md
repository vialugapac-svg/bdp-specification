# Princípio arquitetural — BDP como núcleo independente de discernimento

Data: 2026-11-14
Status: diretriz aprovada pelo responsável do projeto; implementação sujeita a validação técnica.

## Decisão
O BDP não é um agente de IA. É o sistema de inteligência organizacional e governança que contextualiza, orienta e integra capacidades especializadas. O BT Engine preserva a lógica reutilizável de interpretação sistêmica, relações e sinapses dos 11 componentes do BT Model, sem dependência obrigatória de um LLM, provedor ou framework de agentes.

## Requisitos normativos
1. Separar o núcleo de domínio e discernimento dos adaptadores tecnológicos (LLM, RAG, MCP, Skills, agentes e orquestradores).
2. Modelar explicitamente Propósito, cadeia de valor real, clientes, componentes do BT Model, sinapses, evidências, impactos, criticidade e hipóteses, com rastreabilidade e versões.
3. Priorizar a investigação de impactos diretos ao cliente sem sobrepor automaticamente riscos legais, segurança, ambientais ou outros críticos.
4. Manter regras determinísticas e contratos verificáveis para aquilo que não exige geração probabilística. LLMs apoiam interpretação, não constituem fonte de verdade nem autoridade decisória.
5. Exigir origem, finalidade, permissão, segregação de tenant, auditoria, revisão humana e controle de execução de ações externas.
6. Permitir substituir modelos, conectores e agentes sem perda de memória organizacional, evidências, contratos de domínio ou princípios.
7. O BDK-QS01 e o Oráculo são aplicações/experiências que consomem essas capacidades; agentes executam tarefas delimitadas sob autorização, sem assumir o discernimento como autoridade autônoma.
8. Preservar a base cristocêntrica como fundamento de discernimento não confessional, aplicável a clientes de qualquer perfil, sem imposição religiosa.

## Critérios de verificação
- Um caso de NC do BDK-QS01 deve ser interpretável com evidências e regras de domínio mesmo com LLM indisponível, identificando explicitamente o que requer avaliação humana.
- Trocar adaptador de LLM/agente não deve alterar o modelo canônico nem apagar histórico.
- Toda recomendação deve distinguir fato, inferência, hipótese, impacto potencial e decisão humana.
- Validar compatibilidade com ADRs, Shared Runtime, ADR-005, protocolo transversal e regressões antes de alterar código.

## Escopo
Decisão conceitual e arquitetural; não afirma implementação ou homologação concluída.

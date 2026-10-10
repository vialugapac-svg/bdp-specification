# ADR-001 — Avaliação do Paperclip para Orquestração de Agentes

Data: 10/10/2026
Status: PROPOSTO — NÃO IMPLEMENTADO
Projeto: BDP / BT Engine
Referência: https://github.com/PaperclipAI/paperclip

## 1. Contexto

O BDP e o BT Engine poderão mobilizar agentes, ferramentas e competências especializadas para investigar problemas e produzir evidências verificáveis.

O Paperclip é uma tecnologia open source candidata à coordenação operacional desses agentes.

## 2. Hipótese arquitetural

Avaliar o Paperclip como camada opcional de orquestração, preservando a independência do BDP e do BT Engine.

O Paperclip não substitui o discernimento, a interpretação contextual nem a decisão humana.

## 3. Responsabilidades

- BDP: contextualização, investigação e discernimento.
- BT Engine: capacidades reutilizáveis de interpretação.
- BDKs: competências especializadas homologadas.
- Connectors: acesso governado a sistemas e ferramentas.
- Evidence Layer: proveniência, validação e rastreabilidade das evidências.
- CLAREZA: experiência de investigação e decisão humana.
- Paperclip (candidato): coordenação de tarefas, agentes, custos e aprovações.

## 4. Experimento proposto

Realizar prova de conceito isolada com dois agentes em um caso sintético de análise de taxas de adquirência, sem dados reais de clientes.

Comparar com execução direta sem Paperclip, avaliando tempo, custo, segurança, qualidade, rastreabilidade e esforço de integração.

## 5. Critérios de aprovação

- Benefício mensurável sobre a execução direta.
- Compatibilidade com contratos do BT Engine.
- Segurança, isolamento e controle de permissões.
- Rastreabilidade das evidências.
- Recuperação de falhas e observabilidade.
- Baixo acoplamento e possibilidade de substituição.
- Licença e manutenção verificadas.

## 6. Decisão atual

Manter o Paperclip como tecnologia candidata, sem adoção ou integração imediata.

Não alterar os MVPs do CLAREZA, BT Engine, PNE ou Desafio R$ 1.

A adoção dependerá de avaliação técnica e prova de conceito documentada.

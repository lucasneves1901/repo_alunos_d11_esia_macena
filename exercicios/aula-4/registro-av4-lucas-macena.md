# Registro individual — AV1.4

**Estudante:** Lucas Macena | **Data:** 03/10/2026  
**Critério de aceite por R2:** incluir `aberto` e `em_andamento`, excluir `fechado` e preservar a ordem de entrada.

| Entrada | IDs esperados por R2 | IDs do candidato | Status: inferido/observado | Mecanismo/trecho essencial |
|---|---|---|---|---|
| TR-41, TR-42, TR-43, TR-44 | TR-41, TR-42, TR-44 | TR-42, TR-44, TR-41 | Inferido por leitura; não executado | O filtro seleciona TR-41, TR-42 e TR-44.<br>`sorted(..., key=lambda c: c["impacto"] + c["urgencia"], reverse=True)` ordena pelos escores 6, 4 e 2, alterando a ordem de entrada. |

**Teste entregue — o que verifica e o que não consegue distinguir:**  
verifica a inclusão dos ativos e exclusão do fechado nesta entrada, mas não distingue R2 do candidato: a ordem dos ativos já coincide com a ordem decrescente dos escores.

**Trecho do teste (entrada e comparação de IDs) que sustenta minha análise:**  
entrada TR-42, TR-44, TR-41, TR-43; asserção: IDs retornados iguais a `["TR-42", "TR-44", "TR-41"]`. Candidato e ajuste passam nesta entrada.

**Decisão (aceitar, aceitar com condições ou rejeitar) e motivo:**  
rejeitar a proposta atual; a ordenação por pontuação viola a ordem exigida por R2.

**Comparação entre manter e ajustar / responsável pelo aceite:**  
manter preserva a divergência; ajustar remove a ordenação e conserva o filtro. A aprovação cabe à pessoa responsável pela revisão técnica do código.

**Ajuste proposto (texto ou código):**  
`return [c for c in chamados if c["estado"] in ("aberto", "em_andamento")]`

| Caso para conferir o ajuste: entrada e ordem | IDs esperados | Resultado previsto ou observado / status |
|---|---|---|
| TR-41 (`em_andamento`, escore 2), TR-42 (`aberto`, 6),<br>TR-43 (`fechado`, 4), TR-44 (`aberto`, 4), nesta ordem | TR-41, TR-42, TR-44 | TR-41, TR-42, TR-44 — previsto por inspeção do ajuste; não executado.<br>Distingue o ajuste do candidato, que ordena os ativos por escore. |

**Limite remanescente e condição para rever o parecer:**  
R2 não define fronteiras numéricas; o caso verifica a fronteira relevante entre preservar entrada e ordenar por escore. A validação foi por inspeção, não pela execução do Python. Rever após executar testes em Python para lista vazia, cada estado, lista só de fechados e ativos em ordens diferentes da pontuação.

**Origem dos dados e da análise:**  
candidato, teste e entrada simulados no enunciado; método próprio: inspeção; comando e trecho de saída, se executado: não realizado.

**Uso de IA neste registro:**  
utilizada — ferramenta-modelo: Copilot no VS Code - GPT-6 Luna; tarefa/contexto: organizar a comparação com R2 e formular ajuste e conferência; trecho aproveitado e minha verificação: análise e código do ajuste, conferidos contra R2 e os artefatos do enunciado.

**Revisão:** [x] comparação com R2; [x] alcance do teste; [x] ajuste/revalidação; [x] status; [x] uma página.

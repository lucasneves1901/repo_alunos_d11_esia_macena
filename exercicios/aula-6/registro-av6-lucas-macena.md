# Registro individual — AV1.6

**Estudante**: Lucas Macena · **Data**: 03/10/2026

**Objeto do diagnóstico e estágio escolhido:** uso de IA para apoiar a manutenção de Fila Clara na proposta de testes e documentação; estágio escolhido: protótipo.

**Critério/definição adotada:** Protótipo = “tem artefato demonstrável em ambiente controlado”. Piloto = “tem execução limitada no fluxo com participantes e resultados acompanhados”. Uso sustentado = “tem operação recorrente com governança e evidências ao longo do tempo”.

| Fato identificado | Trecho essencial | O que sustenta / o que não sustenta |
|---|---|---|
| M1 | “Há um artefato demonstrável com três exemplos sintéticos de propostas de testes e documentação.” | Sustenta protótipo: existe um artefato concreto em ambiente controlado. Não prova uso real, produtividade nem qualidade em operação. |
| M3 | “Foi definida revisão humana de todas as propostas antes de qualquer uso.” | Sustenta controle e governança inicial. Não substitui execução observada nem evidencia de desempenho. |
| M5 | “Até hoje ocorreram zero execuções com usuários; o plano de duas semanas ainda não começou.” | Refuta piloto: a definição exige execução limitada com participantes e acompanhamento de resultados. O alcance permanece em preparação, sem evidência operacional. |
| M6 | “Não há série de resultados de qualidade, retrabalho, tempo total ou incidentes; metas ainda serão definidas.” | Refuta uso sustentado e também impede afirmar que o protótipo foi validado em contexto operacional. Faltam dados para decidir avanço ou interrupção com base em evidência. |

**Resposta ao argumento de que responsável, revisão e plano já caracterizam o estágio seguinte:** Não. Esses elementos atendem a governança e preparação, mas não à definição de piloto: execução limitada no fluxo com participantes e resultados acompanhados. O fato M5 mostra zero execuções com usuários e M6 mostra ausência de resultados; por isso a iniciativa continua em protótipo. O que existe é um artefato demonstrável e uma preparação planejada, não uma execução validada.

**Evidência que falta para justificar outra classificação:** registros de execução com participantes, qualidade das propostas, retrabalho, tempo por proposta, incidentes e metas comparáveis. Sem isso, não há base para classificar como piloto ou uso sustentado.

**Próximo passo proposto — tarefa, participantes, duração, dados e responsável:** executar um piloto de duas semanas com duas pessoas da manutenção usando dados sintéticos e registro de resultados; responsável pela iniciativa, com revisão humana de todas as propostas e decisão da gestora sobre avanço. Tarefa: produzir propostas de testes e documentação para chamados sintéticos e registrar qualidade, retrabalho, tempo e ajustes.

| Métrica (fórmula/unidade) | Como coletar e referência para comparar | Limite da medida |
|---|---|---|
| Taxa de aprovação sem retrabalho (%) = propostas aprovadas na primeira revisão / total de propostas | Registrar cada proposta e classificar se precisou de ajuste; comparar com meta inicial de 80% e com uma linha de base manual equivalente | Não mede qualidade em uso real nem risco operacional; ajuda a decidir avanço do protótipo, não a afirmar uso sustentado |
| Tempo médio por proposta (minutos) | Medir tempo de geração + revisão por proposta; comparar com esforço manual esperado para o mesmo conjunto de itens | Não mostra impacto total da equipe nem erros não detectados em cenários mais complexos |
| Retrabalho por proposta (minutos ou % com ajuste) | Registrar ajustes e tempo de revisão extra; comparar com limiar de 25% de propostas com retrabalho significativo | Não captura problemas que apareçam em maior volume ou em fluxo real |
| Incidentes relevantes (quantidade) | Registrar erros materiais em testes/documentação; comparar com meta de zero | Pode subestimar falhas que surgem em uso mais amplo |

**Condição proposta de avanço / quem decide:** avançar se a taxa de aprovação sem retrabalho for ≥ 80%, o tempo médio por proposta não ultrapassar a referência manual em mais de 20% e não houver incidentes relevantes. Quem decide: gestora + responsável da iniciativa.

**Condição proposta de interrupção / quem age:** interromper ou replanejar se mais de 25% das propostas exigirem retrabalho significativo, se o tempo médio for claramente superior ao manual, ou se houver erro material em itens críticos. Quem age: responsável da iniciativa e gestora.

**Como os resultados mudariam meu diagnóstico:** se o piloto mostrar execução observada, qualidade aceitável e metas atendidas, a classificação passaria para piloto; se o resultado for fraco, inconclusivo ou inconsistente, o diagnóstico permaneceria em protótipo, e a lacuna não seria convertida em evidência favorável por omissão.

**Origem dos dados e da análise:** fatos M1–M6 simulados; diagnóstico inferido; passo, metas e condições propostos, ainda não executados.

**Uso de IA neste registro:** Copilot no VS Code — GPT-6 Luna; tarefa/contexto: apoio à revisão do diagnóstico e à checagem em Node.js dos limites dos critérios propostos para estágio, avanço e interrupção; trecho aproveitado: análise dos limites e da relação entre aprovação sem retrabalho e retrabalho significativo; verificação: assertivas executadas com Node.js passaram nos casos definidos, mas não testaram o sistema Fila Clara nem executaram um piloto.

**Revisão:** [x] diagnóstico/fatos; [x] contraponto; [x] métrica/comparação; [x] avanço/interrupção; [x] uma página.

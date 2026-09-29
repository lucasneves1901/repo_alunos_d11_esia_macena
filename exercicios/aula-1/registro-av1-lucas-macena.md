# Registro individual — AV1.1

**Estudante:** Lucas Macena — **Data:** 29/09/2026  
Origem: cartões C1–C3 fictícios do enunciado.

| Cartão | Processo sem IA / entrada → saída | Modalidade e justificativa | Verificação de aceite | Responsável humano |
|---|---|---|---|---|
| C1 | Ler R2 e separar inclusão, exclusão e ordem. Entrada: `[FC-003, FC-001, FC-002, FC-004]`. Saída: `[FC-001, FC-002, FC-004]`, pois `FC-003` está `fechado` e os demais estão ativos, na ordem original. | **Com assistência:** delegaria apenas o rascunho dos critérios. O contrato aprovado continuaria sendo a referência da decisão. | Conferir se `aberto` e `em_andamento` foram incluídos, se `fechado` foi excluído e se a ordem original foi preservada. | Pessoa responsável pela manutenção, com aceite técnico da equipe. |
| C2 | Montar casos de departamentos e estados diferentes. Para demonstrar a independência da prioridade, usar também `FC-007` (Oficina, `aberto`, impacto 1, urgência 1, prioridade `baixa`) e `FC-008` (Oficina, `aberto`, impacto 3, urgência 3, prioridade `alta`). Saídas: `pode_visualizar(FC-007, "Oficina") → True`; `pode_visualizar(FC-007, "Laboratório") → False`; `pode_visualizar(FC-008, "Oficina") → True`; `pode_visualizar(FC-008, "Laboratório") → False`. | **Com assistência:** delegaria a sugestão da estrutura do teste, mas confrontaria cada caso com R3. A assistência não decidiria os resultados esperados nem o aceite. | Aceitar somente se o acesso for permitido quando o departamento da pessoa for igual ao do chamado e negado quando for diferente, independentemente do estado ou da prioridade. | Equipe responsável por testes, com aceite humano do responsável técnico. |
| C3 | Ler o pedido e registrar as informações ausentes: regra nova, dados afetados, verificações, riscos e aprovador. Entrada: resumo “facilitar acesso entre áreas”. Saída: não autorizar a implantação nas condições atuais. | **Sem delegar a decisão:** não há informação suficiente para avaliar escopo, risco ou autoridade. Uma ferramenta poderia organizar perguntas, mas não autorizar a mudança. | Confirmar a regra aprovada, os dados afetados, os testes, os resultados e o responsável formal pela aprovação antes de decidir. | Responsável técnico e aprovador formal da mudança, ainda não identificados. |

**Trecho essencial de evidência:**  
Em C1, a entrada `[FC-003, FC-001, FC-002, FC-004]` deve produzir `[FC-001, FC-002, FC-004]`. Isso demonstra a inclusão dos estados ativos, a exclusão de `fechado` e a preservação da ordem. Em C2, `FC-007` e `FC-008` têm o mesmo departamento e estado, mas prioridades diferentes; ambos devem ter o mesmo resultado de visibilidade. Isso demonstra que R3 depende do departamento, não da prioridade.

**Alternativa para o cartão C2:** fazer o teste sem IA, escrevendo manualmente os casos, as saídas booleanas e a justificativa.

**Comparação com minha escolha:** a assistência pode acelerar a organização dos casos, mas pode sugerir entradas ou interpretações incorretas. Eu escolheria “sem IA” se a ferramenta ou o modelo não tivesse procedência visível ou se não fosse possível revisar cada resultado contra R3.

**Limite da delegação e condição para rever a escolha:** delego somente sugestões e rascunhos, nunca o aceite técnico nem a autorização de produção. No C3, só reavalio a autorização depois de confirmadas a regra, os dados, as verificações e a autoridade aprovadora.

**Procedência/IA:** utilizada a ferramenta GitHub Copilot, no Visual Studio Code; modelo: GPT-5.6 Luna. A tarefa delegada foi revisar a clareza do registro e sugerir evidências para C1 e C2. Eu conferi as sugestões com o contrato de R2 e R3, mantive as decisões e defini o aceite final. O raciocínio e a decisão registrados são meus.

**Revisão:** [x] três decisões; [x] evidência localizada; [x] alternativa e limite; [x] até uma página.
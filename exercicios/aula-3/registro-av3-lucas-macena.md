# Registro individual — AV1.3

**Limite: uma página.** Estudante: Lucas Macena — Data: 01/10/2026
**O que a listagem e a documentação precisam cumprir, conforme R2/R4:** incluir `aberto` e `em_andamento`, excluir `fechado` e manter a ordem de entrada; a documentação deve descrever a mesma regra.

| Caso / estado a verificar | Entrada (IDs e ordem) | IDs esperados na ordem | Obrigação de R2 e como verificar |
|---|---|---|---|
| 1 / aberto | [TR-33] | [TR-33] | Incluir `aberto`; confirmar que o ID permanece. |
| 2 / em_andamento | [TR-31] | [TR-31] | Incluir `em_andamento`; confirmar que o ID permanece. |
| 3 / fechado | [TR-32] | [] | Excluir `fechado`; confirmar que TR-32 não aparece. |

**Entrada combinada TR-31, TR-32, TR-33 → IDs esperados:** [TR-31, TR-33]
**Como conferiria a ordem (compare a posição dos IDs na entrada e na saída esperada):** TR-31 aparece antes de TR-33 na entrada e continua antes dele na saída; TR-32 é excluído.
**Documentação proposta (até três frases):** A listagem inclui chamados `aberto` e `em_andamento`, exclui `fechado` e preserva a ordem de entrada.

**Etapa em que admitiria IA / tarefa que ela faria / pessoa responsável por conferir:** Na elaboração dos casos e do texto, a IA pode sugerir um rascunho; eu confiro os resultados e decido o aceite.
**O que essa pessoa deve verificar antes de aprovar:** Confrontar os três estados, as saídas e a ordem com R2; confirmar que a documentação expressa a mesma regra.
**Alternativa sem IA e comparação:** Eu faria os casos e o texto diretamente pelo contrato; com IA, o rascunho pode acelerar a redação, mas ainda precisa de conferência.
**O que os casos não verificam e o que me faria rever a aprovação:** Não cobrem listas maiores ou vazias nem a execução do programa. Eu reveria o aceite se uma execução divergisse das saídas esperadas ou se o contrato mudasse.

**Origem dos dados e como fiz a análise:** entrada fictícia do enunciado; saídas esperadas calculadas por R2; comparei estados e ordem com a entrada e a documentação proposta com R4; execução não realizada.
**Uso de IA neste registro:** GitHub Copilot; modelo não informado; contexto/tarefa: completar o registro conforme o enunciado e R2/R4; aproveitei o rascunho das respostas, conferi as saídas com R2 e a documentação com R4.

**Revisão:** [x] três estados; [x] ordem; [x] texto; [x] aceite/limite; [x] uma página.

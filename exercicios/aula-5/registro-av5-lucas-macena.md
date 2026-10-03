# Registro individual — AV1.5

**Estudante:** Lucas Macena · **Data:** 03/10/2026  
**Critério de decisão:** Envio externo somente após confirmação de ferramenta, permissões e condições de tratamento.  
**Encaminhamento e justificativa:** Não enviar chamados ou logs reais agora. Avançar manualmente com dados sintéticos e R1–R4; isso não autoriza envio externo.  
**Alternativa viável:** Aguardar esclarecimentos de segurança e da gestão antes de considerar uso externo. Reduz risco de envio não autorizado, mas atrasa a resposta. A análise manual sintética permite avançar já, com maior esforço.

| Regra | Trecho do enunciado que justifica a regra | Risco e consequência | Ação para tratar o risco | Responsável | Registro proposto para conferir o cumprimento |
|---|---|---|---|---|---|
| **1 — dados** | O chamado pode conter identificação, relato de incidente e informações de acesso; permissões não foram confirmadas. | Envio real sem autorização pode expor dados a serviço de condições desconhecidas. | Não enviar dados reais; usar apenas cópia sintética. | Manutenção não envia; segurança e gestora avaliam eventual exceção. | Checklist de origem dos dados e envio; eventual decisão e escopo, sem conteúdo real. |
| **2 — resultado** | A manutenção pode revisar explicações/testes. A verificação técnica achou divergências da lógica inicial com R1–R3. | Resposta pode repetir defeitos do código ou contrariar o contrato; produção está fora do escopo. | Conferir com R1–R4: limiar 5 em R1; `em_andamento` em R2; acesso somente ao mesmo departamento em R3, qualquer estado/prioridade. | Pessoa da manutenção revisora. | Registrar regras, método, casos, esperado/observado, divergências e decisão; só dados sintéticos. |

**Informação ausente:** Ferramenta autorizada, permissões e condições de tratamento (retenção e treinamento). Sem confirmação, não recomendo envio real.

**Exceção:** Segurança e gestora avaliam eventual pedido; não está aprovada. Registrar decisão, responsáveis, escopo, condições e justificativa, sem reproduzir chamado/log.

**O que mudaria a decisão:** Confirmação documentada de ferramenta, permissões e tratamento permitiria reavaliar uso externo no escopo autorizado. Testes aprovados aumentam confiança funcional, mas não substituem autorização nem liberam produção.

**Origem/evidência:** Enunciado hipotético e R1–R4. Espelhei em Node.js a lógica Python conferida: 144 casos válidos, 39 divergências (R1: 2; R2: 19; R3: 18); não executei Python. Transcrição anterior: 6/9 testes passaram, com 3 falhas nas mesmas regras. Nenhum dado real.

**Uso de IA:** Copilot no VS Code - GPT-6 Luna apoiou a revisão e a checagem em Node.js. A checagem refere-se à lógica do código didático, não avalia a decisão de governança nem equivale a executar Python; confronto feito com R1–R4.

**Revisão:** [x] decisão/alternativa; [x] duas regras completas; [x] exceção/limite; [x] uma página.
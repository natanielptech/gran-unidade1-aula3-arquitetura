# 4. Máquina de estados × atividades

Os dois diagramas podem descrever o mesmo sistema, mas respondem a perguntas diferentes: estados explicam o ciclo de vida de uma entidade; atividades explicam o fluxo de um processo.

| Aspecto | Máquina de estados | Atividades |
|---|---|---|
| Foco | Ciclo de vida de **um objeto** | Fluxo de um **processo ou algoritmo** |
| Elemento central | Estado e transição disparada por evento | Ação e fluxo de controle |
| Paralelismo | Não representado diretamente | Nativo, com fork/join |
| Orientação | Aos estados | Às ações |
| Uso típico | Status de `Pedido`, `Conta` ou `Assinatura` | Aprovação, checkout ou processamento de pedido |

## Como podem trabalhar juntos

Em um sistema de pedidos, a máquina de estados documenta quando o pedido pode ser criado, pago, enviado, entregue ou cancelado. O diagrama de atividades detalha o processo executado para processá-lo. Uma ação específica desse processo pode, por sua vez, ser refinada com uma sequência para mostrar a colaboração entre serviços.

## Quando usar

Se a questão é “em que condição está esta entidade?”, escolha estados. Se é “quais etapas executam este processo e em que ordem?”, escolha atividades. Se é “quais participantes trocam mensagens neste cenário?”, escolha sequência.

## Checklist de revisão

- [ ] Identifico se o objetivo é documentar um objeto ou um processo.
- [ ] Não uso estados para sugerir paralelismo que o diagrama não representa diretamente.
- [ ] Uso atividades para mostrar fork/join e sincronização.
- [ ] Considero sequência para detalhar uma colaboração pontual.

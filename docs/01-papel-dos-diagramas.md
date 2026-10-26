# 1. O papel dos diagramas

Diagramas UML diferentes respondem a perguntas diferentes. A escolha começa pelo aspecto do sistema que se quer explicar.

## A lacuna que cada diagrama preenche

- **Classes** mostram o que os objetos são: sua estrutura e relações.
- **Sequência** mostra uma interação pontual entre objetos ao longo de um cenário.
- **Máquina de estados** mostra o ciclo de vida de um objeto e as mudanças permitidas nesse ciclo.
- **Atividades** mostram o fluxo de um processo, incluindo decisões e atividades paralelas.

Um diagrama de sequência pode detalhar a colaboração que realiza uma ação de um processo. Já a máquina de estados descreve como eventos mudam a condição de uma entidade. Assim, diagramas de estados e atividades complementam — não substituem — classes e sequência.

## Um exemplo em duas perspectivas

Considere um pedido. A máquina de estados explica como ele passa de criado a pago, enviado e entregue, ou como pode ser cancelado. O diagrama de atividades explica o processamento: verificar estoque, decidir se é possível prosseguir, processar o pagamento e executar notificações.

| Pergunta | Diagrama mais adequado |
|---|---|
| Quais são os estados válidos de um pedido? | Máquina de estados |
| Quais etapas compõem o processamento? | Atividades |
| Quais objetos colaboram para reservar itens? | Sequência |
| Quais classes e relações existem no domínio? | Classes |

## Quando usar

Use estados para comunicar as condições estáveis de uma entidade ao longo do tempo; atividades para comunicar o fluxo de trabalho; sequência para detalhar mensagens entre participantes em um cenário.

## Checklist de revisão

- [ ] Diferencio a estrutura de objetos do ciclo de vida de um objeto.
- [ ] Diferencio uma interação pontual de um processo ponta a ponta.
- [ ] Consigo relacionar estados, atividades e sequência sem tratá-los como alternativas excludentes.

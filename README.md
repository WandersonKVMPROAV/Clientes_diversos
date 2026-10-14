# KVM Pro AV | Clientes Diversos

App de acompanhamento do cronograma de Clientes Diversos, com barra lateral, mapa, salas, calendário, pendências e tarefas. Funciona em computador, tablet e celular, e não precisa de internet depois de aberto.

## Arquivos

- `index.html`: o app completo. Abre na apresentação rotativa e tem menu lateral para as demais seções.
- `tv.html`: só a apresentação rotativa, em tela cheia, pensada para TVs e para o Admooh.

Os dois arquivos precisam ficar na mesma pasta do repositório.

## Como usar

- **Menu lateral:** o botão de três linhas no topo oculta e mostra o menu. No celular e no tablet o menu abre sobre a tela e fecha ao escolher uma seção.
- **Apresentação:** passa as telas sozinha, com botões para voltar, pausar, avançar e abrir em tela cheia.
- **Filtros:** mês, tipo e local valem para visão geral, mapa, calendário, pendências e tarefas.
- **Tema:** o botão no topo alterna entre claro e escuro e lembra a escolha.
- **Links diretos:** `index.html#mapa`, `#salas`, `#calendario`, `#pendencias`, `#tarefas` e `#visao` abrem cada seção.

## Admooh

Use o endereço de `tv.html` no player:

- `tv.html?tempo=20` define quantos segundos cada tela fica visível (padrão: 15).
- `tv.html?tela=mapa` fixa uma tela. Opções: `visao`, `mapa`, `agenda`, `pendencias`, `salas`.

Endereços antigos com `?tela=` ou `?tempo=` em `index.html` continuam funcionando: o app redireciona para a tela de TV.


## Dados

- Fonte: cards de tarefa exportados do Bitrix e controle de salas dos clientes.
- Cronograma até 13/10/2026. O status das tarefas pendentes foi conferido no Bitrix em 14/10/2026.
- Tarefas marcadas como "a confirmar" são as que não puderam ser abertas na conferência.
- Os dados ficam dentro dos arquivos. Para atualizar, é preciso gerar novos `index.html` e `tv.html` a partir de uma nova exportação.

# Trello to Kaneo Converter

Página web estática que converte o JSON exportado de um quadro do Trello para o formato de importação de tarefas do Kaneo.

## Como usar

1. Abra `index.html` no navegador.
2. Exporte o quadro no Trello em JSON.
3. Arraste o arquivo para a página.
4. Revise o mapeamento de cada lista do Trello para o slug da coluna correspondente no Kaneo.
5. Clique em **Converter para Kaneo**.
6. Baixe o JSON gerado e importe-o no projeto do Kaneo.

## Conversão

- `card.name` -> `title`
- `card.desc` -> `description`
- lista do Trello -> `status`
- labels de prioridade -> `priority` (opcional)
- `card.start` -> `startDate`
- `card.due` -> `dueDate`
- `userId` padrão -> `userId` (opcional)

A opção de preservação de dados extras adiciona labels, checklists, links de anexos e a URL original do cartão à descrição, já que esses dados não fazem parte do formato básico de importação de tarefas usado pela página.

## Privacidade

O processamento é 100% local no navegador. O arquivo JSON não é enviado a nenhum servidor.

# Trello to Kaneo Converter

Página HTML única para converter o JSON exportado de um quadro do Trello para o formato aceito pelo importador de tarefas do Kaneo.

## Como usar

1. Abra `index.html` no navegador.
2. Selecione o JSON exportado do Trello.
3. Para cada lista do Trello, digite o **Nome exato da Coluna no Kaneo** ou marque **Ignorar esta lista**.
4. Clique em **Converter para Kaneo**.
5. Revise o preview e baixe o JSON final.

O conversor transforma automaticamente o nome visível da coluna no slug interno usado pelo Kaneo. Exemplo: `In Progress` vira `in-progress`.

A transformação segue a mesma regra usada pelo Kaneo ao criar colunas. Colunas que foram renomeadas depois de criadas podem manter o slug antigo no Kaneo.

Todo o processamento acontece localmente no navegador.

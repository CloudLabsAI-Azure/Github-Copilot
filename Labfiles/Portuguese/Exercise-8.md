# Exercício 8: Utilização do GitHub Copilot para código T-SQL e YAML [opcional]

### Duração estimada: 15 minutos

Neste exercício, o principal objetivo é aproveitar as capacidades do GitHub Copilot, uma poderosa ferramenta de escrita de código assistida por IA, para o ajudar a gerar código para duas linguagens de programação distintas: T-SQL e YAML. Pode aproveitar os comentários para gerar sugestões do Copilot!

>**Nota**: O GitHub Copilot irá sugerir automaticamente um corpo de função completo ou código em texto cinzento. Exemplos do que provavelmente verá neste exercício, mas a sugestão exata pode variar.

>**Nota**: Se não conseguir ver nenhuma sugestão do GitHub Copilot no VS Code, reinicie o VS Code uma vez e tente novamente.

## Objetivos do laboratório

Poderá completar as seguintes tarefas:

- Tarefa 1: Gerar uma consulta SQL com o GitHub Copilot utilizando comentários
- Tarefa 2: Gerar YAML com o GitHub Copilot utilizando comentários
- Tarefa 3: Enviar código para o seu repositório a partir do Codespace


### Tarefa 1: Gerar uma consulta SQL com o GitHub Copilot utilizando comentários

1. Navegue de volta para o Visual Studio Code e, a partir do Codespace na janela Explorer do VS Code, crie um novo ficheiro.

   ![](../../media/chat-code-new.png)

1. Nomeie o ficheiro `demo.sql` e digite o comentário abaixo:

    ```
    -- Create a table for 5 products with product names and prices
    ```

1. Para abrir um novo separador com múltiplas soluções sintetizadas, prima `Ctrl+Enter`. O GitHub Copilot irá sintetizar cerca de 10 sugestões de código diferentes num novo separador. Pode visualizar as soluções e, para aceitar uma sugestão, clique em **Accept suggestion** abaixo da solução e guarde o ficheiro.

   ![](../../media/ex7-t1-s3.png)

1. Após aceitar a sugestão, reveja-a cuidadosamente antes de a aplicar.

   ![](../../media/demo-sql-1.png)

 >**Nota**: Poderá não ver as mesmas sugestões mostradas na captura de ecrã; sugestões exatas podem variar.

### Tarefa 2: Gerar YAML com o GitHub Copilot utilizando comentários

1. A partir do codespace na janela do VS Code Explorer, crie um novo ficheiro.

   ![](../../media/chat-code-new.png)

1. Nomeie o ficheiro como `deploy-app.yml` e digite o comentário abaixo:

    ```
    # Create a GitHub action to email a report from a file at 6 a.m. daily
    ```

1. Para abrir um novo separador com múltiplas soluções sintetizadas, prima `Ctrl+Enter`. O GitHub Copilot irá sintetizar cerca de 10 sugestões de código diferentes num novo separador. Pode visualizar as soluções e, para aceitar uma sugestão, clique em **Accept suggestion** abaixo da solução e guarde o ficheiro.

   ![](../../media/ex7-t2-s3.png)

1. Após aceitar a sugestão, reveja-a cuidadosamente antes de a aplicar.

   ![](../../media/demo-yaml-1.png)

 >**Nota**: Poderá não ver as mesmas sugestões mostradas na captura de ecrã; sugestões exatas podem variar.

### Tarefa 3: Enviar código para o seu repositório a partir do Codespace

1. Utilize o terminal VS Code para adicionar ficheiros ao repositório. Abra o VS Code Terminal se ainda não estiver aberto.

1. Execute o comando abaixo para adicionar todos os ficheiros ao repositório:

    ```
    git add --all
    ```

1. De seguida, na fase terminal do VS Code, envie as alterações para o repositório:

    ```
    git commit -m "Copilot fourth commit"
    ```

1. Por fim, a partir do terminal VS Code, envie o código para o repositório:

    ```
    git push
    ```

   ![](../../media/ex-6-push.png)

   >**Nota**: Aguarde cerca de 60 segundos e atualize a página inicial do repositório para o passo seguinte.

1. Pode verificar os ficheiros recém-adicionados disponíveis no seu repositório GitHub.

   ![](../../media/ex-6-github.png)

### Resumo

Neste exercício, gerou código para SQL e YAML utilizando comentários com a ajuda do GitHub Copilot.

### Concluiu o laboratório com sucesso

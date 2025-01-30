# Exercício 8: Utilização do GitHub Copilot para código T-SQL e YAML [opcional]

### Duração estimada: 15 minutos

Neste exercício, o principal objetivo é aproveitar as capacidades do GitHub Copilot, uma poderosa ferramenta de escrita de código assistida por IA, para o ajudar a gerar código para duas linguagens de programação distintas: T-SQL e YAML. Pode aproveitar os comentários para gerar sugestões do Copilot!

>**Aviso**: O GitHub Copilot irá sugerir automaticamente um corpo de função completo ou código em texto cinzento. Exemplos do que provavelmente verá neste exercício, mas a sugestão exata pode variar.

>**Nota**: Se não conseguir ver nenhuma sugestão do GitHub Copilot no VS Code, reinicie o VS Code uma vez e tente novamente.

## Objetivos do laboratório

Poderá completar as seguintes tarefas:

- Tarefa 1: Gerar uma consulta SQL com o GitHub Copilot utilizando comentários
- Tarefa 2: Gerar YAML com o GitHub Copilot utilizando comentários


### Tarefa 1: Gerar uma consulta SQL com o GitHub Copilot utilizando comentários

1. Navegue de volta para a janel do codespace no Visual Studio Code e, crie um novo ficheiro.

   >**Nota:** No exercício anterior, você realizou as tarefas em uma nova janela, então volte para a janela do codespace.

   ![](../../media/chat-code-new.png)

1. Nomeie o ficheiro `demo.sql`, digite o comentário abaixo e pressione **Enter**:

    ```
    -- create a table with 5 columns customer_id, customer_fname, customer_lname, customer_phone, customer_address
    ```

    ![](../media/c34.png)   

1. Observe como o Copilot consegue gerar as próximas linhas de código.

1. Clique em `Tab` e pressione **Enter**.

1. Em seguida, digite o comentário abaixo e pressione **Enter**.

   ```
   -- fill in 5 rows in customers table
   ```

    ![](../media/c35.png)   

1. Clique em `Tab` e pressione **Enter**.

1. Vamos executar a consulta para exibir a tabela. Digite o comentário abaixo e pressione **Enter**.

   ```
   -- show the data in customers table
   ```

    ![](../media/c36.png)   

1. Clique em Enter e depois clique em `Tab` para selecionar a sugestão.

1. Pressione `Ctrl+S` para salvar o arquivo.

1. Clique no ícone Iniciar do Windows, expanda a pasta **Microsoft SQL Server Tools 20 (1)** e selecione **SQL Server Management Studio 20 (2)**.

   ![](../media/hub106.png)

1. Certifique-se de que os seguintes detalhes sejam adicionados:

   - Server name: **labvm-<inject key="Deployment-id" enableCopy="false"/>\SQLEXPRESS (1)**
   - Authetication: **Windows Authentication (2)**
   - Encryption: Check the box for **Trust server certificate (3)**
   - Clique em **Connect (4)**

       ![](../media/hub115.png)
     
1. Uma vez conectado ao servidor, clique em **New Query** na parte superior.

   ![](../media/hub110.png)

1. Navegue até ao **Visual Studio Code** e copie todo o conteúdo que buscamos no arquivo `demo.sql`.

1. Cole-o na nova página de consulta.

1. Selecione cada **bloco de código (1)** e clique em **Execute (2)**. Observe como cada bloco de código é executado com sucesso, gerando a saída esperada no terminal.

   ![](../media/hub111.png)

   ![](../media/hub112.png)

   ![](../media/hub113.png)
   
1. Você pode observar como ele processa cada bloco de código e exibe a tabela de Customers..

   ![](../media/hub40.png)   


### Tarefa 2: Gerar YAML com o GitHub Copilot utilizando comentários

1. Dentro do codespace, na janela do VS Code Explorer, crie um novo arquivo e nomeie-o como `report.yml`

    ![](../media/chat-code-new.png)

1. Pressione `Ctrl + I` , digite o comentário abaixo e clique em Enviar:

   ```
   # Create a GitHub action to email a report from a file at 6 a.m. daily
   ```
   ![](../media/hub9.png)

1. Clique em **Accept**.

   ![](../media/hub8.png)

      > **Nota**: Pode ser que você não veja as mesmas sugestões mostradas na captura de tela; as sugestões exatas podem variar.

1. Abra o GitHub Copilot Chat na parte superior, digite `Explian the cron syntax in this code` e clique em **send**.

      ![](../media/hub10.png)
   
1. Verifique a resposta e entenda como utilizar e criar expressões Cron.

      ![](../media/hub11.png)

1. Ofereça outra consulta: `How should a GitHub Actions YAML file be structured?` e avalie a resposta fornecida.

   ![](../media/c41.png)



### Resumo

Neste exercício, gerou código para SQL e YAML utilizando comentários com a ajuda do GitHub Copilot.

### Concluiu o laboratório com sucesso
